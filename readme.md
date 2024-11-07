# Essential Checks for MT5 EAs
All EAs uploaded to the MQL5 marketplace have to pass a mandatory automatic validation. This validation checks for logic errors and most importantly edge cases such as checking for insufficient funds, volume limits and freeze levels.

A complete list of all the checks along with the solutions to resolve them are available on MQL5 site [here](https://www.mql5.com/en/articles/2555). In this repo, I have the compiled the checks that most traders are likely to miss into a single function to resolve most likely issues at validation.

## Instructions
1. Copy the code from the `checks_code` file to your EA.
2. Call `RunChecks` function with the correct arguments before every trade entry or modification and escape the code for a `false` return value