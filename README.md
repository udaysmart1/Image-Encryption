# Img-encrypt




## examples

Command

### For encrypting an image myImage.png to encryptedImage.png and saving the key to key.txt

```sh
imcrypt -e myImage.png -i encryptedImageName.png -p keyFile.txt
```

output

```sh
 imcrypt  v0.0.1 by theninza
An image encryption node-js cli

✔ Image read successfully
✔ Output image file name is valid
✔ Output key file name is valid
✔ Image data read successfully
✔ Key generated successfully
✔ Image encrypted successfully
✔ Image saved successfully
✔ Key saved successfully

✔  Image encrypted successfully  Image encrypted successfully:
                                  Encrypted image: encryptedImageName.png
                                  Key: keyFile.txt

 Give it a star on github:  https://github.com/theninza/imcrypt
```

### For decrypting an image encryptedImage.png with its key key.txt to decryptedImage.png

```sh
imcrypt -d encryptedImage.png -k key.txt -i decryptedImage.png
```

output

```sh
 imcrypt  v0.0.1 by theninza
An image encryption node-js cli

✔ Image read successfully
✔ Key read successfully
✔ Decryption successful
✔ Image saved successfully

✔  Success  Image decrypted successfully

                        Decrypted Image: decryptedImage.png

## Limitation

While encryption and decryption is perfect on the png images. On jpg and jpeg, the operation is not perfect. Jpg and jpeg images are lossy and while encryption and decryption, a few pixels values are changed. The decrypted image is however, very similar to the original image but with a few pixels changed.
