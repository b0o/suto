### suto 
#### get sudo timeout status

suto simply returns the current sudo timeout status.


#### Usage:
suto [-h] | [-ve]

#### Results:
| Result | Status | Explanation |
| ------ |:------:|:------------|
| 0 | sudo is not timed out | the user **will not** need to re-enter their password to run sudo |
| 1 | sudo is timed out     | the user   **will**   need to re-enter their password to run sudo |

#### Options:
 - `-h`            Print help message and exit
 - `-v`            Print verbose output to stderr
 - `-e`            Exit with result as exit code

#### Notes:
Remember that the result of this command is only valid for the exact moment it is run.

It's possible the sudo timeout will expire immediately after this command is run.

#### License:
&copy;2017 Maddison Hellstrom; MIT License
