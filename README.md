# Linear Equation Solver Web Application

This is a simple web application that allows users to solve a system of linear equations with three variables (x, y, z) using Cramer's Rule. Users can input the coefficients of the variables and constants into a form, and the application will calculate and display the solutions for x, y, and z if they exist.

## Table of Contents

- [Linear Equation Solver Web Application](#linear-equation-solver-web-application)
  - [Table of Contents](#table-of-contents)
  - [Getting Started](#getting-started)
  - [Usage](#usage)
  - [How It Works](#how-it-works)
  - [Error Handling](#error-handling)

## Getting Started

To run this web application locally, follow these steps:

1. Clone or download this repository to your local machine.
2. Open the `index.html` file in a web browser.
3. Visit live demo [here.](<[google.com](https://yuniku01.github.io/solveforx/)>)

## Usage

1. In the web browser, you will see a form with input fields for the coefficients of x, y, and z, as well as constants for three linear equations.
2. Enter the coefficients and constants into the input fields. The form is structured as follows:

   - Equation 1: a<sub>00</sub>x + a<sub>01</sub>y + a<sub>02</sub>z = b<sub>0</sub>
   - Equation 2: a<sub>10</sub>x + a<sub>11</sub>y + a<sub>12</sub>z = b<sub>1</sub>
   - Equation 3: a<sub>20</sub>x + a<sub>21</sub>y + a<sub>22</sub>z = b<sub>2</sub>

3. After entering the coefficients and constants, click the "Solve" button to calculate the solutions for x, y, and z.
4. The results will be displayed below the form, showing the values of x, y, and z.

## How It Works

The web application uses Cramer's Rule to solve the system of linear equations. Here's how it works:

1. The coefficients of x, y, and z, as well as the constants, are extracted from the form.
2. The determinants of matrices are calculated for the main coefficient matrix (d) and for matrices where one column is replaced by the constants from the equations (dx, dy, dz).
3. The solutions for x, y, and z are calculated as follows:
   - x = dx / d
   - y = dy / d
   - z = dz / d

## Error Handling

The application provides error handling for different scenarios:

- If the determinant (d) is zero, it indicates that the system has either no solution or infinitely many solutions, and an appropriate message is displayed.
- If the determinant (d) is non-zero, it calculates and displays the solutions for x, y, and z.
