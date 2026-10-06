# Ohm's Law Calculator

## Purpose
This program calculates electric current using Ohm's Law. The user enters a voltage in volts and a resistance in ohms, and the program calculates the current using I = V / R.

## Input Format
Enter two numeric values separated by a space:

voltage resistance

For example:

12 4

The resistance must be greater than zero. Non-numeric input and resistance values that are zero or negative are considered invalid.

## Build
Compile the program using:

g++ -std=c++17 -Wall -Wextra -pedantic src/main.cpp -o build/app

## Run
Run the program using:

./build/app

Then enter the voltage and resistance.

## Example Output
Input:

12 4

Output:

Current: 3 A

## Testing
Run the acceptance tests using:

bash test.sh

If all tests pass, the terminal displays:

All acceptance tests passed

## Limitations
The calculator only calculates current using voltage and resistance. It does not calculate voltage or resistance. Resistance must be greater than zero, and the program expects numeric input.

## Debugging Reflection
While testing the program, I found that the expected-output files must match the program output exactly. One test initially failed because the expected-output file did not contain a newline at the end. Adding the newline allowed the output to match and the acceptance tests to pass.