# 🔐 Secure Random Password Generator

A robust, web-based tool designed to generate high-entropy, secure passwords. This project features a modern, "charming" Dark Mode UI with neon accents, providing a smooth user experience while ensuring cryptographic strength.

![App Screenshot]
https://github.com/rajeevsheoran/Password-Generator/blob/main/Screenshot%202025-12-08%20223032.png
## 🚀 Live Demo
https://github.com/rajeevsheoran/Password-Generator.git

## 🛠️ Features

* **Customizable Length:** Slider control to adjust password length (1-20 characters).
* **Complexity Options:** Toggles for Uppercase, Lowercase, Numbers, and Special Symbols.
* **Visual Strength Indicator:** Real-time color-coded feedback (Red, Yellow, Green) based on password entropy.
* **One-Click Copy:** Copies the generated password to the system clipboard instantly.
* **Responsive UI:** A "charming" interface featuring CSS gradients, custom variables, and neon glow effects.

## 💻 Tech Stack

* **HTML5:** Sematic structure.
* **CSS3:** Flexbox, CSS Custom Properties (Variables), Linear Gradients, Box Shadows.
* **JavaScript:** DOM Manipulation, Event Handling, Randomization Logic.

## 🧠 How It Works (The Logic)

1.  **Character Pools:** The script maintains strings for all selected character types (Upper, Lower, Number, Symbol).
2.  **Mandatory Characters:** To ensure strict adherence to user selection, the script first forces one random character from *each* checked category into the password.
3.  **Random Filling:** The remaining length is filled by randomly selecting characters from the combined pool.
4.  **Shuffling:** The final string is shuffled to randomize the position of the mandatory characters so the pattern isn't predictable.
5.  **Strength Calculation:** The indicator logic checks for a mix of character types and minimum length to assign a strength rating (Weak, Medium, Strong).

## 📂 Installation

1.  Clone the repository:
    ```bash
    git clone https://github.com/rajeevsheoran/Password-Generator.git
    ```
2.  Navigate to the project directory:
    ```bash
    cd password-generator
    ```
3.  Open `index.html` in your browser.

## 📝 What I Learned

* **DOM Manipulation:** deeply understanding `querySelector`, event listeners, and updating UI elements dynamically.
* **CSS Variables:** Using `:root` to manage a consistent color theme and make updates easier.
* **Algorithm Logic:** Implementing the logic to ensure at least one character of a selected type appears in the final output.
* **Clipboard API:** How to write text to the system clipboard using `navigator.clipboard.writeText`.

Made with ❤️ by Rajeev
