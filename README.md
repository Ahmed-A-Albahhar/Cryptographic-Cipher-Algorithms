# Cryptographic-Cipher-Algorithms
An interactive desktop application demonstrating Shift, Caesar, and Vigenère cryptographic encryption algorithms.
# Cryptographic Cipher Algorithms: Information Security Application

## 📌 Project Overview
This project involves the development of an interactive desktop application designed to demonstrate foundational information security principles. The application programmatically executes classical cryptographic algorithms to encrypt and decrypt plaintext, showcasing a practical understanding of data protection, secure communication logic, and algorithmic key manipulation.

## 💡 Core Competencies Demonstrated
* **Algorithmic Logic:** Engineered dynamic encryption and decryption pathways that manipulate string characters based on user-defined integer and string keys.
* **Information Security:** Demonstrated a fundamental understanding of cipher mechanics, a critical prerequisite for grasping modern data encryption standards (DES/AES) and secure system architecture.
* **GUI Development:** Built an intuitive user interface that allows users to seamlessly switch between different cryptographic methods, input dynamic keys, and visualize the immediate cipher output.

## 🔐 Implemented Cryptographic Algorithms

### 1. Shift Cipher
* **Mechanism:** Shifts every letter in the plaintext by a fixed, user-defined integer key.
* **Example Execution:** Encrypting the word `APPLE` with a shift key of `4` successfully outputs the cipher text `ETTPI`.

### 2. Caesar Cipher
* **Mechanism:** A historical substitution cipher utilizing a fixed shift (traditionally 3) to obscure data.
* **Example Execution:** Encrypting the plaintext `HELLO` outputs `KHOOR`. The application also successfully reverses the algorithm, decrypting `KHOOR` back to `HELLO`.

### 3. Vigenère Cipher
* **Mechanism:** A method of encrypting alphabetic text by using a series of interwoven Caesar ciphers based on the letters of a dynamic keyword (polyalphabetic substitution).
* **Example Execution:** Encrypting the plaintext `ATTACKATDAWN` using the repeating keyword `LEMONLEMONLE` outputs the complex cipher text `LXFOPVEFRNHR`. The decryption matrix successfully reverses this operation back to the original plaintext.
