## Clyde The Cougar
Challenge Description: "Clyde sent me this photo, but there should be a flag in it somewhere. All I know is that it was hidden using LBS."

#### Provided Items
challenge has a downloadable .png file that is a picture of Clyde the Cougar.

#### Process
- After a quick google search, we know that LBS is Least Significant Bits, a technique used to hide information in photos.

- LBS can be used to hide text in an image (one character in every pixel), or it can be used to hide an image within another. We can try to use a tool like [StegOnline](https://georgeom.net/StegOnline/image) or [aperisolve]https://www.aperisolve.com/6440293d3f6d2cdec4d1161aac4e6b85 or something else.

- Attempting to extract files/data on StegOnline returns no data:

- We can browse the bit planes to see if an image was hidden in the clyde.png:


#### Result:
```
cofc{reg_green_blue}
```
