## 🚀 30-Day Coding Challenge: Day 22

This project is the twenty-second entry in my 30-day coding challenge. Today's goal was to build the classic game of Tic-Tac-Toe using React. This project is a foundational exercise for understanding state management, immutability, and component logic in a React application.

### 📖 Project Overview

This is a fully functional Tic-Tac-Toe game with a clean, modern interface. The application allows two players to take turns, determines the winner or if the game is a draw, and highlights the winning line of squares. It also includes a "Reset Game" button to start a new match. The entire game logic, from tracking turns to calculating the winner, is handled within React components.

### ✨ Live Demo & Screenshot

Below is a screenshot of the application's interface.
![Jun-30-2025 16-12-10](https://github.com/user-attachments/assets/c1d35678-1553-4d3c-878a-94d69ed4c143)


### 🌟 Key Features

* **Complete Game Logic:** Handles alternating turns between 'X' and 'O'.
* **Winner Detection:** Automatically detects when a player has won by checking all rows, columns, and diagonals.
* **Draw Detection:** Recognizes when the board is full and no winner can be declared.
* **Winning Line Highlight:** The three squares that form the winning line are visually highlighted.
* **Game Status Display:** A clear status message indicates whose turn it is, who the winner is, or if the game is a draw.
* **Reset Functionality:** A "Reset Game" button allows players to start a new game at any time.
* **State History:** The application maintains a history of all moves, which allows for potential future features like an "undo" button or "time travel" to previous moves.

### 💻 Technologies Used

This project was built using a modern, lightweight React setup.

![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)
![Babel](https://img.shields.io/badge/Babel-%23F9DC3e.svg?style=for-the-badge&logo=babel&logoColor=black)
![TailwindCSS](https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white)

* **React:** The core library for building the user interface and managing game state.
* **ReactDOM:** Used to render the React component into the browser's DOM.
* **Babel:** Used as a transpiler to convert JSX into standard JavaScript.
* **Tailwind CSS:** For all styling and layout.

### 🛠️ How to Run Locally

This project is set up to be extremely simple to run, with no build process required:

1.  **Clone the repository (or download the code):**
    ```bash
    git clone https://github.com/timothy-agboada/react-tic-tac-toe.git
    ```
2.  **Navigate to the project directory:**
    ```bash
    cd react-tic-tac-toe
    ```
3.  **Open the `index.html` file in your web browser.** The CDN links will handle loading all necessary libraries automatically.

### 🎯 Learning Objectives

This project was a fundamental exercise in several key React concepts:

* **Lifting State Up:** Managing the entire game state in the top-level `Game` component and passing data and functions down to child components (`Board`, `Square`) via props.
* **Immutability:** Practicing the core React principle of not modifying state directly. The board state is updated by creating a copy of the array for each move.
* **Component Composition:** Building the UI by composing smaller, reusable components together.
* **Derived State:** Calculating values like the `winner` and game `status` from the base state on every render, rather than storing them in state themselves.
* **Handling User Interaction:** Passing functions as props to allow child components to update the parent's state.
