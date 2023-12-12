# Numbers Toolkit
#### Description: 
    This project aims to provide basic tools at hand for working with numbers.

## Project Overview and Usage

    My website is made up of one page for the simplicity of using the tools and the lack of need for other details.

    In the first part of the page is located the Numbers Extractor which was the main idea of the website. To use it properly you should enter the desired text in the first textbox using copy-paste or you could upload a text document by pressing 'Upload file' button then selecting the desired document. Afterwards, you should press 'Extract numbers' button and the result will be displayed in the second textbox.

    In the second part the Calculator can be seen which is a rudimentary basic calculator, but it comes in handy.

    In the last part the Random Number Generator can be seen which works like any other basic number generator existing on internet, but once again it is at hand. 

## Features

- Numbers extractor
- Basic calculator
- Random number generator
- No need to leave website environment for basic math tools

## Project Explanation
### HTML Structure

    1. Text to numbers Section:
        - Text areas for input and output
        - Buttons for number extraction, file upload, numbers copier and screen clearer

    2. Calculator Section:
        - A screen for displaying operations and the result
        - Buttons for digits and operations

    3. Random number generator Section:
        - Input fields for specifying minimum and maximum
        - Result area for the result
        - A button for number generator and a button for copying to clipboard

### CSS Styling

    .bg-image:
        - Sets background image

    .strtoint, .calculator, .numberpicker:
        - Set the background color and it's opacity
        - Set the border width and it's color

    !!! CSS NEED TO BE UPDATED !!!

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

        !!! JAVASCRIPT NEED TO BE UPDATED !!!

## File Dependencies

- The website is in index.html where HTML and JavaScript code is located
- The CSS styles are defined in the main.css file
- A favicon and background image located in images folder are used for enhanced visual appearence

## Notes

- The application relies on the browser's JavaScript functionality and may not work properly with JavaScript disabled.
- The website utilizes the Bootstrap framework for styling buttons
- You can add any features as you want

### Enjoy using Numbers Toolkit website!
