# Portfolio Generator

A Node.js command-line tool that generates a professional portfolio webpage based on user input. The app prompts you for your name, GitHub username, an "About Me" section, and multiple projects. It then creates a fully styled HTML page with your portfolio content, ready to be deployed or shared.

## Features

- Interactive command-line prompts using **Inquirer.js**
- Collects:
  - Name and GitHub username
  - Optional "About Me" section
  - Unlimited projects with:
    - Project name, description, link
    - Technologies used (checkboxes)
    - Option to feature a project
- Generates a responsive HTML page with:
  - Styled header and footer
  - "About Me" section (if provided)
  - Featured projects displayed prominently
  - All projects shown in a clean grid layout
- Automatically copies a CSS stylesheet into the output folder
- Outputs files to a `dist/` directory for easy deployment



## My Portfolio Site

🔗 **Live site:** 
https://jthapa1987.github.io/portfolio-generator/


*(🚧 Currently deploying – screenshot shows how it will look)*

![Portfolio Screenshot](./images/screenshot.png)

## Technologies Used

- Node.js
- Inquirer.js (for interactive prompts)
- JavaScript (ES6+)
- CSS3 (with custom variables and responsive grid)
- HTML5

## Installation

1. **Clone the repository** (or download the files)
   ```bash
   git clone https://github.com/jthapa1987/portfolio-generator.git
   cd portfolio-generator

    Install dependencies
    bash

    npm install

    (Make sure you have Node.js installed. This project requires inquirer – install it with npm install inquirer if not already listed in package.json.)

Usage

Run the application from the terminal:
bash

node app.js

Then answer the prompts:

    Enter your name and GitHub username.

    Decide whether to add an "About Me" section.

    For each project, provide the name, description, technologies used (check all that apply), and the GitHub link.

    Choose if the project should be featured (featured projects appear at the top in full‑width cards).

    Add as many projects as you want.

After completing all prompts, a message will confirm file creation. Find your generated portfolio in:

    dist/index.html – the generated portfolio page

    dist/style.css – the stylesheet (automatically copied from src/style.css)

Open dist/index.html in your browser to view your portfolio.
Example

Here’s a sample of what the generated portfolio looks like (after running the app with sample data):

https://./200-project-endoflesson.jpg
Project Structure
text

portfolio-generator/
├── app.js                 # Main entry point (prompts and file generation)
├── package.json           # Dependencies and scripts
├── src/
│   ├── page-template.js   # HTML template generator
│   └── style.css          # Source CSS (copied to dist/)
├── utils/
│   └── generate-site.js   # Promise-based file utilities
├── dist/                  # Output folder (created on run)
│   ├── index.html
│   └── style.css
├── sample.js              # Example script to test with sample data
└── sample-answer.js       # Sample portfolio data for testing

Future Improvements

    Add more styling options or themes

    Support for adding a profile picture

    Deploy directly to GitHub Pages via script

License

This project is open source and available under the MIT License.
Author

    Jeevan Thapa – https://github.com/jthapa1987
