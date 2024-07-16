# calorieCounter
This project is a web application that helps users track their calorie intake across 
different meals and compare it with their calorie budget. 
Users can add entries for different meals and exercises, and the app will calculate the remaining calories based on the provided inputs.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Code Explanation](#code-explanation)

## Overview
The Calorie Counter app allows users to input calorie data for various meals and exercises. 
It calculates the total calories consumed and burned and compares it against a user-defined calorie budget to determine a calorie surplus or deficit.

## Features
- Add entries for breakfast, lunch, dinner, snacks, and exercises.
- Calculate total calories consumed, burned, and remaining based on a calorie budget.
- Display results indicating whether there is a calorie surplus or deficit.
- Clear the form to reset all inputs and results.

## Getting Started
Follow these instructions to get a copy of the project up and running on your local machine.

### Prerequisites
- A web browser (e.g., Chrome, Firefox, Edge, etc.)

### Installation
1. Clone the repository
2. Navigate to the project directory
3. Open the index.html file in your web browser

## Usage
1. Open the index.html file in your web browser
2. Use the dropdown menu to select a meal or exercise category and click the "Add Entry" button to add new entries
3. Enter the names and calorie values for each entry
4. Enter your calorie budget
5. Click the "Calculate" button to see your calorie consumption, burned calories, and remaining calories
6. Click the "Clear" button to reset the form

## Code Explanation
### HTML Elements
- "calorieCounter": The main form element for the calorie counter
- "budgetNumberInput": Input for the calorie budget
- "entryDropdown": Dropdown menu to select a meal or exercise category
- "addEntryButton": Button to add new entries
- "clearButton": Button to clear the form
- "output": Element to display the calculation results

### JavaScript Functions
- "cleanInputString(str)": Removes invalid characters (+, -, and spaces) from a string
- "isInvalidInput(str)": Checks if the input string contains invalid scientific notation (e)
- "addEntry()": Adds a new entry input field for the selected category
- "calculateCalories(e)": Calculates the total calories consumed, burned, and remaining based on the inputs
- "getCaloriesFromInputs(list)": Sums up the calorie values from a list of input elements
- "clearForm()": Clears all input fields and results

### Event Listeners
- "addEntryButton.addEventListener("click", addEntry)": Adds a new entry when the "Add Entry" button is clicked
- "calorieCounter.addEventListener("submit", calculateCalories)": Calculates calories when the form is submitted
- "clearButton.addEventListener("click", clearForm)": Clears the form when the "Clear" button is clicked
