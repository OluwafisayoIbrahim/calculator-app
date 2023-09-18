# React Calculator

This is a simple calculator application built using React. It allows users to perform basic arithmetic operations such as addition, subtraction, multiplication, and division.

![image](https://github.com/OluwafisayoIbrahim/calculator-app/assets/78263397/50a1dd83-4aae-4c0e-81be-6494fbb9a9ed


## Table of Contents

- [Overview](#overview)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Components](#components)
- [Styles](#styles)
- [Actions](#actions)
- [Reducer](#reducer)
- [Utility Functions](#utility-functions)
- [Contributing](#contributing)
- [License](#license)

## Overview

The React Calculator application provides a user-friendly interface for performing arithmetic calculations. It features a responsive grid layout of buttons for digits, arithmetic operations, and control functions.

## Getting Started with Create React App

This project was bootstrapped with Create React App. For more information about Create React App, visit the [documentation](https://facebook.github.io/create-react-app/docs/getting-started).

### Available Scripts

In the project directory, you can run:

- `npm start`: Runs the app in the development mode. Open [http://localhost:3000](http://localhost:3000) to view it in your browser. The page will reload when you make changes, and you may also see any lint errors in the console.
- `npm test`: Launches the test runner in interactive watch mode. Learn more about [running tests](https://facebook.github.io/create-react-app/docs/running-tests).
- `npm run build`: Builds the app for production to the `build` folder. It optimizes the build for the best performance, minifies the code, and includes hashes in filenames. Your app is then ready to be deployed. Learn more about [deployment](https://facebook.github.io/create-react-app/docs/deployment).
- `npm run eject`: **Note: this is a one-way operation. Once you eject, you can't go back!** If you're not satisfied with the build tool and configuration choices, you can eject at any time. This command will copy all configuration files and dependencies to your project, giving you full control. Learn more about [ejecting](https://facebook.github.io/create-react-app/docs/available-scripts#npm-run-eject).

## Usage

1. Click on digit buttons to input numbers.
2. Use operation buttons (+, -, *, ÷) to select the desired arithmetic operation.
3. To clear the current calculation, click the "AC" button.
4. To delete the last entered digit, click the "DEL" button.
5. Click the "=" button to evaluate the entered expression and view the result.

## Components

### App.js

This is the main component that renders the calculator interface. It manages the calculator's state using the `useReducer` hook.

### DigitButton.js

A reusable component for rendering digit buttons. It dispatches the `ADD_DIGIT` action when a digit button is clicked.

### OperationButton.js

A reusable component for rendering operation buttons. It dispatches the `CHOOSE_OPERATION` action when an operation button is clicked.

## Styles

The calculator's styling is defined in the `styles.css` file. It includes the grid layout and styling for buttons and output display.

## Actions

The calculator uses the following actions defined in the `ACTIONS` object:

- `ADD_DIGIT`: Add a digit to the current operand.
- `CHOOSE_OPERATION`: Select an arithmetic operation.
- `CLEAR`: Clear the calculator's state.
- `DELETE_DIGIT`: Delete the last entered digit.
- `EVALUATE`: Evaluate the current expression and display the result.

## Reducer

The `reducer` function handles state changes based on dispatched actions. It performs various operations such as adding digits, choosing operations, clearing, deleting digits, and evaluating expressions.

## Utility Functions

- `evaluate`: Calculates the result of an arithmetic expression based on the selected operation.
- `formatOperand`: Formats the operand for display, adding thousands separators if applicable.

## Contributing

Contributions to this project are welcome! Feel free to submit pull requests to suggest improvements or fixes.
