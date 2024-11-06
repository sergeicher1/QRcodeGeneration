---

# QR Code Generator 📱🎉

A simple yet powerful Python tool for generating QR codes from text or URLs! This QR Code Generator is perfect for anyone who wants to quickly create and save QR codes for their projects, websites, or social media profiles. With easy-to-use parameters and robust error handling, this tool is beginner-friendly yet highly effective.

---

## 📝 Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Examples](#examples)
- [Parameters](#parameters)
- [Error Handling](#error-handling)
- [License](#license)

---

## ✨ Features
- Generate QR codes from any text or URL
- Save QR codes as `.png` images with customizable file names
- Adjustable QR code properties (size, error correction level, box size, border width)
- Built-in error handling for invalid input and file issues
- Lightweight and easy to integrate into other Python projects

---

## 🚀 Installation

To use this tool, make sure you have Python installed. Then, install the required libraries:

```bash
pip install --upgrade 'qrcode[pil]'

pip install qrcode pillow
```

The `qrcode` library is essential for QR code generation, and `Pillow` (Python Imaging Library) is required for saving the QR code as an image file.

---

## 💻 Usage

Simply clone the repository, or copy the code file to your local machine, and run it in any Python environment.

### Running the Script
```bash
python qr_code_generator.py
```

### Example Interaction

1. The program will prompt you to enter the text or URL you want to encode in the QR code.
2. The generated QR code will be saved in the same directory with the default name `qrcode.png`.

---

## 🛠 Parameters

The `generate_qr_code` function includes several customizable parameters to give you control over the QR code's appearance.

- **text** (str): Text or URL to encode in the QR code.
- **filename** (str, optional): The name of the file where the QR code image will be saved. Default is `qrcode.png`.

#### QR Code Properties
These properties are set within the function but can be modified directly in the code:
- **version**: Controls the size of the QR code (1 is the smallest).
- **error_correction**: Defines the error correction level (default is `ERROR_CORRECT_L`).
- **box_size**: Size of each box in the QR code.
- **border**: Width of the border around the QR code.

---

## 🧩 Examples

Here are a few examples of how you can use this QR Code Generator:

```python
# Basic usage
generate_qr_code("https://www.zero-to-hero.dev")

# Save with custom filename
generate_qr_code("Hello Hero!", filename="hello_hero_qr.png")
```

These examples will generate QR codes for the provided text or URL and save them as images.

---

## ⚠️ Error Handling

This script includes error handling for:
- Invalid text input: Raises a `ValueError` if the input text is empty or not a string.
- File permission errors: Catches `IOError` if there’s an issue saving the file.
- Unexpected errors: Catches any other exceptions, providing an error message.

---

## 📄 License
This project is licensed under the MIT License, so feel free to use and modify it for your own projects!

---

### 🤝 Contributions
Contributions, issues, and feature requests are welcome! Feel free to check out the [issues page](https://github.com/your-username/qr-code-generator/issues) if you'd like to contribute.

---

Happy QR Coding! 🎉
