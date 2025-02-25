# Steganography Image Encryption

This project is a simple Python script that performs steganography by encoding a secret message within an image and decoding it using a passcode.

## Features
- Encodes a secret message into an image.
- Requires a passcode for decryption.
- Saves the encrypted image as `encryptedImage.jpg`.
- Works with `cv2` for image processing.

## Prerequisites
Ensure you have the following installed before running the script:
- Python 3.x
- OpenCV (`cv2`)

You can install OpenCV using pip:
```sh
pip install opencv-python
```

## Usage

### Encryption
1. Place the image you want to use in the same directory as the script and rename it to `mypic.jpg` (or modify the script to use your preferred image name).
2. Run the script:
   ```sh
   python stego.py
   ```
3. Enter the secret message when prompted.
4. Enter a passcode for encryption.
5. The encrypted image will be saved as `encryptedImage.jpg`.

### Decryption
1. Run the script again.
2. Enter the passcode used for encryption.
3. If the passcode is correct, the hidden message will be displayed.
4. If the passcode is incorrect, an authentication failure message will be shown.

## Notes
- The encryption method modifies pixel values in the image, which may slightly change its appearance.
- Ensure the passcode is stored securely as decryption requires an exact match.

## License
This project is open-source and available under the MIT License.

