# Uncommon Bash Error: Missing Error Checking

This repository demonstrates a common, yet subtle error in bash scripting:  neglecting to check the exit status of external commands used within command substitution. The script `bug.sh` attempts to process a file but lacks proper error handling, which can lead to unexpected results or silent failures.

The solution, `bugSolution.sh`, showcases the correct approach, utilizing conditional statements to check the exit status and handle failures gracefully.

## How to Reproduce

1. Clone this repository.
2. Run `bug.sh`.
3. Observe the output (or lack thereof) if `my_file.txt` is missing or inaccessible.
4. Run `bugSolution.sh` to see the improved error handling.