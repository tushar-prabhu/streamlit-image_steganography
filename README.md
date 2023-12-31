# Image Steganography

This Python script uses the Streamlit library to create a web-based application for image steganography. Steganography is the practice of concealing a file, message, image, or video within another file, message, image, or video.

## Dependencies

- Streamlit
- PIL
- base64
- io

## How to Run

You can run this script by using the following command:

```bash
streamlit run main.py
```

## Features

The script provides two main functionalities:

1. **Encode**: This feature allows you to hide a message within an image. You can enter your message and upload an image, and the script will encode the message into the image.

2. **Decode**: This feature allows you to extract a hidden message from an image. You can upload an image, and the script will decode and display any hidden message.

The script uses the least significant bit of the red channel of each pixel to encode the binary representation of the message. A special character (`$`) is added at the end of the message as a delimiter.

## User Interface

The user interface is divided into two sections: Encode and Decode. Each section has its own input fields and displays the output image.

In the Encode section, you can enter a message and upload an image. After encoding, the script displays the encoded image and provides a download link.

In the Decode section, you can upload an encoded image. After decoding, the script displays the hidden message and the original image.

## Note

This script only works with PNG, JPG, and JPEG images. The quality of the encoded image may be slightly reduced due to the encoding process. The hidden message is not encrypted, so anyone with the same script can decode it. For better security, consider encrypting the message before encoding it into the image. 

## Disclaimer

This script is for educational purposes only. Please do not use it for illegal activities. The author is not responsible for any misuse of this script. Always respect privacy and the law.