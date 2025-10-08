# Weight Converter

A simple Python script to convert weight between Kilograms and Pounds based on user input.

## Description

This Python program allows users to input a weight value and its unit (Kilograms or Pounds) and converts it to the other unit. The program handles invalid inputs by displaying an error message if an unrecognized unit is provided.

## Features

- Converts weight from Kilograms to Pounds and vice versa.
- Rounds the converted weight to two decimal places for readability.
- Validates user input and displays an error for invalid units.

## Installation

1. Clone the repository:
   git clone https://github.com/darbabhargav19/WeightCalculator.git
2. Navigate to the project directory:
   cd <your-repo-name>
3. Ensure you have Python installed (version 3.x recommended). Check your Python version:
   python --version
   or
   python3 --version

## Usage

1. Run the script using Python:
   python weight_converter.py
   or
   python3 weight_converter.py
2. Follow the prompts:
   - Enter the unit of the weight (K for Kilograms or L for Pounds).
   - Enter the weight value.
3. The program will display the converted weight or an error message if the unit is invalid.

### Example
enter your weight : 70
kilograms or pounds? (K or L) : K
your weight is : 154.35 Lbs

enter your weight : 154.35
kilograms or pounds? (K or L) : L
your weight is : 70.0 Kgs

enter your weight : 70
kilograms or pounds? (K or L) : G
G was not valid

## Code

weight = float(input("enter your weight : "))
unit = input("kilograms or pounds? (K or L) :")

if unit == "K":
    weight = weight * 2.205
    unit = "Lbs"
    print(f"your weight is : {round(weight, 2)} {unit}")
elif unit == "L":
    weight = weight / 2.205
    unit = "Kgs"
    print(f"your weight is : {round(weight, 2)} {unit}")
else:
    print(f"{unit} was not valid")

## Requirements

- Python 3.x
- No external libraries required

## Contributing

Contributions are welcome! If you'd like to improve this project, please follow these steps:
1. Fork the repository.
2. Create a new branch (git checkout -b feature-branch).
3. Make your changes and commit (git commit -m 'Add some feature').
4. Push to the branch (git push origin feature-branch).
5. Open a pull request.

## Acknowledgments

- Inspired by simple command-line utility projects.
- Thanks to the Python community for excellent resources and documentation.
