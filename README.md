# Steganography-Tool

This project implements a secure messaging application that utilizes steganography techniques to hide messages within images. By embedding secret messages in image files, the application ensures both data confidentiality and subtlety, making it ideal for secure communication.

---

## Features

- **Message Embedding:** Hide sensitive messages within image files using advanced steganographic techniques.
- **Message Extraction:** Retrieve hidden messages from steganographic images.
- **Encryption:** Ensure the confidentiality of embedded messages using a user-defined key.
- **Cross-Platform Support:** Built with Python and Tkinter, the application runs seamlessly on Windows, macOS, and Linux.
- **User-Friendly Interface:** Intuitive graphical interface for both embedding and extracting messages.

---

## How It Works

1. **Message Embedding:**
   - The user selects an image file (JPEG or PNG).
   - A message and a key are provided by the user.
   - The message is encrypted using the provided key.
   - The encrypted message is embedded into the image using Least Significant Bit (LSB) steganography.

2. **Message Extraction:**
   - The user provides a steganographic image and the key.
   - The application extracts the embedded message.
   - The message is decrypted using the provided key to reveal the original text.

---

## Technologies Used

- **Programming Language:** Python
- **Graphical Interface:** Tkinter
- **Image Processing:** PIL (Python Imaging Library)
- **Encryption:** Python Cryptography Toolkit (cryptography module)

---

## Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/yourusername/steganography-messaging-app.git
   cd steganography-messaging-app
   ```

2. **Install Dependencies:**

   Ensure you have Python 3.7 or higher installed. Then, run:

   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Application:**

   ```bash
   python app.py
   ```

---

## Usage

1. **Embedding a Message:**
   - Open the application.
   - Select an image file.
   - Enter the message and encryption key.
   - Click the "Encode and Download Image" button to save the steganographic image.

2. **Extracting a Message:**
   - Open the application.
   - Select a steganographic image file.
   - Enter the encryption key.
   - Click the "Decode Image" button to retrieve the original text.

---

## Sample Output

### Before Embedding:
![Original Image](images/original_image_example.jpg)

### After Embedding:
![Steganographic Image](images/steganographic_image_example.jpg)

---

## Limitations

- Supports only JPEG and PNG formats.
- The image must have sufficient space to embed the message.
- Incorrect keys will result in decryption failures or garbled text.

---
