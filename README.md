# HTML/JS Security Playground

This is a simple, single-file web application that provides a hands-on environment for exploring basic client-side security concepts. It's built entirely with vanilla HTML, CSS, and JavaScript, leveraging the powerful **Web Crypto API** for all cryptographic operations.

This project serves as a great pet-project to demonstrate understanding of browser-native cryptography and secure frontend practices.

## Demo

![Security Playground Demo](httpsimg/securityplaygroundexample.gif)

---

## Getting Started

You can run this project in two ways:

### 1. Live Demo (Recommended)

The project is hosted on GitHub Pages. Simply visit the site to start using the playground:

**[Visit the Live Site](https://kvarbulemba.github.io/your-repo-name/)**

### 2. Local Setup

If you want to run the project locally:

1.  Clone this repository:
    ```bash
    git clone [https://github.com/kvarbulemba/your-repo-name.git](https://github.com/kvarbulemba/your-repo-name.git)
    ```
2.  Navigate to the directory:
    ```bash
    cd your-repo-name
    ```
3.  Open the `index.html` file directly in your favorite web browser.

---

## Features

The playground is divided into four main modules:

* ** Hashing (SHA-256):**
    * Calculates the SHA-256 hash of any text input in real-time.
    * Demonstrates the one-way nature of hashing.

* ** Encryption (AES-GCM):**
    * Symmetrically encrypts and decrypts text using a user-provided password.
    * Uses **PBKDF2** (`crypto.subtle.deriveKey`) to create a secure key from the password.
    * Uses **AES-GCM** (`crypto.subtle.encrypt/decrypt`) for modern, authenticated encryption.
    * Packs the `salt`, `iv`, and `ciphertext` into a single `Base64` string for easy transport.

* ** Password Generator:**
    * Generates strong, random passwords using the cryptographically secure `crypto.getRandomValues`.
    * Provides customizable options:
        * Length (8-64 characters)
        * Uppercase letters
        * Lowercase letters
        * Numbers
        * Symbols
    * Includes a "Download (.txt)" feature.

* ** Password Strength Checker:**
    * Provides real-time feedback on password strength.
    * Uses a simple scoring algorithm based on length, character variety (uppercase, lowercase, numbers, symbols).
    * Displays a visual strength bar and actionable text feedback.

---

## Tech Stack

No frameworks, no libraries, no dependencies.

* **HTML5:** For the core structure.
* **CSS3:** For all styling, including the dark mode UI, flexbox layout, and animated GIF background.
* **Vanilla JavaScript (ES6+):** For all application logic and DOM manipulation.
* **Web Crypto API:** The core of the project. Used for:
    * `crypto.subtle.digest` (Hashing)
    * `crypto.subtle.deriveKey` (PBKDF2)
    * `crypto.subtle.encrypt` / `crypto.subtle.decrypt` (AES-GCM)
    * `crypto.getRandomValues` (Secure password generation)

---

## Author

**kvarbulemba**

* **GitHub:** [@[kvarbulemba]](https://github.com/kvarbulemba)
* **LinkedIn:** [Illia Denysenko](https://www.linkedin.com/in/illia-denysenko-aa2056375)
* **Resume:** [View My Resume](https://kvarbulemba.github.io/cv-website)
