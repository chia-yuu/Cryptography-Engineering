# NYCU 2023 Cryptography-Engineering final project -- steganography tool
112 下 謝致仁 密碼工程 final project

## Abstract
This project focuses on developing a steganography tool that can embed secret messages within digital media (images, audio, video). We uilized advanced steganographic techniques, the tool embeds encrypted messages into media files. The system architecture involves encoding and decoding. The tool demonstrates the potential for secure communication, making it a valuable asset in fields requiring confidential information transfer.

## Introduction -- What is Steganography
- Definition
    - Concealing info within message or object, unnoticed by humans.
    - In computing/electronic contexts, a computer file is concealed within another file.
- How it Works?
    - Concealment Medium : text, image, audio, video
    - Carrier Medium : where message is hidden, e.g. image file
    - Techniques : altering pixels, modifying text spacing, manipulating audio signals

## System Architecture
- Encryption
    - Input : concealment medium and carrier medium
    - Output : the encrypted file containing the hidden message
- Decryption
    - Input : the encrypted file
    - Output : the hidden message

## Usage
Type `main.py` to run the code, then you can choose what kind of stego way you want (text to text, text to audio, image to image...). The result file (either encoded or decoded file) will be in `files/`.

The algorithm we use in this project is LSB insertion. The input file will first translare into binary, then use LSB insertion to hide or get the secret message, and convert back to its original format.

## Contribution and Future Enhancement
- Contribution
    - Integrate steganography across different file types
    - User-friendly interface
- Future Enhancement
    - Unknown hidden file format
    - Size restrictions