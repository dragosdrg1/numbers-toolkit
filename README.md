# Numbers Toolkit
#### Video Demo:  
    https://youtu.be/YY0CF4x8fS0
#### Description: 
    This project aims to provide basic tools at hand for working with numbers.

## Project Overview and Usage

    My website is made up of one page for the simplicity of using the tools and the lack of need for other details.

    In the left side of the page is located the **numbers extractor** which was the main reason for the website. To use it properly you should enter the desired text in the first textbox using copy-paste or you could upload a text document by pressing 'Upload file' button then selecting the desired document. Afterwards, you should press 'Extract numbers' button and the result will be displayed in the second textbox.

    In the right upper corner you can see the **calculator** which is a rudimentary basic calculator, but it comes in handy. The design is inspired by Microsoft Windows 10 calculator, but with some minor changes to ensure originality and you can use it roughly the same way.

    In the right lower corner you can see the **random number generator** which works like any other basic number generator existing on internet, but once again it is at hand. 

## Features

- Numbers extractor
- Basic calculator
- Random number generator
- No need to leave website environment for basic tools

## Project Explanation
### HTML Structure

    1. Text to numbers Section:
        - Text areas for input and output
        - Buttons for triggering 'extractNumbers' function and file upload 

    2. Calculator Section:
        - 2 screens like in the windows calculator for displaying operations and the result
        - Buttons for digits and operations

    3. Random number generator Section:
        - Input fields for specifying minimum and maximum
        - Result area for the result
        - Button for triggering 'random' function and button for copying to clipboard

### CSS Styling

    .bg-image:
        - Sets background image

    .strtoint, .calculator, .numberpicker:
        - Set the background color and it's opacity
        - Set the border width and it's color

    .strtoint and .calculator and .numberpicker:
        - Set the layout of the each div

    .strtoint textarea:
        - Styles the textareas
    
    .strtoint #STRbuttons:
        - Styles the buttons

    .calculator input, .numberpicker input:
        - Styles the 2 screens of the calculator

### Javascript Functions

    1. Text to numbers:
        extractNumbers(text):
            - Gets a string and display numbers from it
        upload file functionality:
            - If the 'Upload file' button is pressed then the function get the file content and call the 'extractNumbers' function
    
    2. Calculator:
        isOperator(character):
            - Check if the character inputted is an operator
        appendOperator():
            - Append to the smaller screen expression the operator selected
            - If the screen must be reset then the clear screens functions are called
        appendDecimal():
            - Append to the bigger screen number a '.' for decimal numbers
            - If the screen must be reset then the clear screens functions are called
        calculate():
            - Evaluate expression on the smalle screen only if possible
            - If the expression can not be evaluated then a error message is displayed
        clearEvalScreen():
            - Clear the smaller screen
        clearScreen():
            - Clear the bigger screen
        appendDigit(digit):
            - Append to the bigger screen number the digit selected
            - If the screen must be reset then the clear screens functions are called
        removeLastCharacter():
            - Remove last character on the bigger screen when the specific button is pressed
    
    3. Random number generator:
        random():
            - Generates a random number in a range when the specific button is pressed
        copyRandom():
            - Copy to clipboard the number generated when the specific button is pressed

## File Dependencies

- The website utilizes the Bootstrap framework for styling
- The CSS styles are defined in the main.css file
- A favicon and background image located in images folder are used for enhanced visual appearence

## Notes

- The application relies on the browser's JavaScript functionality and may not work properly with JavaScript disabled.
- I know that the project has a terribled designed css, but I've tried very hard to fix this but I could not figure out how to fix it
- I will do my best to rewrite the css in the future

### Enjoy using Numbers Toolkit website!