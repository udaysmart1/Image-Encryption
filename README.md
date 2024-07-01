# Img-encrypt




## examples

Command

### For encrypting an image myImage.png to encryptedImage.png and saving the key to key.txt

```sh
imcrypt -e myImage.png -i encryptedImageName.png -p keyFile.txt
```



### For decrypting an image encryptedImage.png with its key key.txt to decryptedImage.png

```sh
imcrypt -d encryptedImage.png -k key.txt -i decryptedImage.png
```



### Limitation
While encryption and decryption is perfect on the png images. On jpg and jpeg, the operation is not perfect. Jpg and jpeg images are lossy and while encryption and decryption, a few pixels values are changed. The decrypted image is however, very similar to the original image but with a few pixels changed.
