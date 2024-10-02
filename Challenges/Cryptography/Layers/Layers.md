## Layers
- Challenge Description: "I found this on my flash drive, any idea what these could mean?"

#### Provided Items
challenge has a downloadable .txt file containing the following:
```
108 120 111 108 123 106 97 110 104 120 100 117 114 116 114 119 112 108 114 121 113 110 97 98 125 10
```

#### Process
- This challenge is cryptography, so we can assume the provided text is some sort of cipher text that needs to be decoded
- Using a website like cipheridentifier, we can figure out what cipher was used


- From the cipher identifier, we know that ASCII encoding was used


- Decoding from ASCII results in the following:
```
	lxol{janhxdurtrwplryqnab}
```

- If we repeat putting this new cipher text into the cipher identifier, we can use one of the most likely ones (i tried affline, vigenere, and ROT and all could decrypt it)


#### Result:
```
cofc{areyoulikingciphers}
```