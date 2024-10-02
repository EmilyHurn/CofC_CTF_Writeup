## Check The Hex
Challenge Description: "I found this corrupted file, hopefully it has the flag in it. Maybe you should try and figure out what sort of file it is and how to fix it?"

#### Provided Items
challenge has a downloadable .zip file containing a png. When the user attempts to view the png, an error such as 'It may be damaged or use a file format that Preview doesn’t recognize' will appear

#### Process
- This file is likely an actual .png, and the title is check the hex, indicating we can fix the file by editing the hex.

- verifing the file format using an exif viewer or file command results in unknown file format / data, so we are left to trial and error different file types.

- If we open the file using a hex editor such as https://hexed.it/, we see the following:



- Notably, the file header is ``` 00 00 00 00 0D 0A 1A 0A```
- If we compare this to a list of command hex headers (https://en.wikipedia.org/wiki/List_of_file_signatures), we notice that the last 4 bits are the same as png, h5, and hdf5, 

- Returning to the hex editor, we can replace the first 4 bytes with those of png, h5, or hdf5 to attempt to restore our file.
- If we replace the first four with ```89 50 4E 47``` for PNG, we get the following:



#### Result:
```
cofc{hex_hero}
```
