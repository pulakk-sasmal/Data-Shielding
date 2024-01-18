# Steganopy - Python Image Steganography

## Overview

Steganopy is a simple Python program that allows users to embed and extract messages within images using the Least Significant Bit (LSB) technique. This technique involves breaking down bytes into bit sets and embedding them in specific pixel bands of an image, ensuring minimal visual distortion.

## Features

- Embeds and extracts messages securely within images.
- Uses the LSB technique to hide information without causing noticeable changes in the image.
- Supports various image formats (e.g., PNG, JPEG, BMP).
- Provides options for users to specify input and output files.

## Installation

Steganopy requires the following dependencies:

- Python 3.x
- Pillow (PIL Fork): `pip install pillow`

To install Steganopy, clone the repository or download the source code from [GitHub](https://github.com/example/steganopy).

```bash
git clone https://github.com/example/steganopy.git
cd steganopy
```

## Usage

### Embedding a Message

To embed a message in an image, use the following command:

```bash
python steganopy.py embed -i input_image.png -m secret_message.txt -o output_image.png
```

- `-i` or `--input`: Path to the input image.
- `-m` or `--message`: Path to the text file containing the message to be embedded.
- `-o` or `--output`: Path to the output image with the embedded message.

### Extracting a Message

To extract a message from an image, use the following command:

```bash
python steganopy.py extract -i image_with_message.png -o extracted_message.txt
```

- `-i` or `--input`: Path to the image containing the embedded message.
- `-o` or `--output`: Path to the file where the extracted message will be saved.

## Example

### Embedding

```bash
python steganopy.py embed -i input_image.png -m secret_message.txt -o output_image.png
```

### Extracting

```bash
python steganopy.py extract -i output_image.png -o extracted_message.txt
```

## Note

- Steganopy works best with high-resolution images to minimize the impact on visual quality.
- Always keep a backup of the original image, as embedding data may result in irreversible changes.

## Acknowledgments

Special thanks to the Pillow development team for providing a powerful image processing library.

If you have any issues or suggestions, please feel free to open an [issue](https://github.com/example/steganopy/issues).

Happy Steganography!
