alias ls="rm *" script  creates an alias.
Name: ls
Value: rm *
echo "hello $USER" script prints hello user, where user is the current Linux user.
export PATH=$PATH:/action script add /action to the PATH. /action should be the last directory the shell looks into when looking for a program.
echo $PATH | tr ':' '\n' | wc -l script counts the number of directories in the PATH.
printenv script lists environment variables.
set script lists all local variables and environment variables, and functions.
BEST="School" script  creates a new local variable.
Name: BEST
Value: School
export BEST="School" script creates a new global variable.
Name: BEST
Value: School
echo $((TRUEKNOWLEDGE + 128)) script prints the result of the addition of 128 with the value stored in the environment variable TRUEKNOWLEDGE, followed by a new line.
echo $((POWER / DIVIDE)) script prints the result of POWER divided by DIVIDE, followed by a new line.
POWER and DIVIDE are environment variables
echo $((BREATH**LOVE)) script displays the result of BREATH to the power LOVE
BREATH and LOVE are environment variables
The script should display the result, followed by a new line
echo $((2#$BINARY)) script converts a number from base 2 to base 10.
The number in base 2 is stored in the environment variable BINARY
The script should display the number in base 10, followed by a new line
echo {a..z}{a..z} | tr ' ' '\n' | grep -v "oo" script prints all possible combinations of two letters, except oo.
Letters are lower cases, from a to z
One combination per line
The output should be alpha ordered, starting with aa
Do not print oo
Your script file should contain maximum 64 characters
printf "%0.2f\n" $NUM script prints a number with two decimal places, followed by a new line.
The number will be stored in the environment variable NUM.
printf "%x\n" $DECIMAL script converts a number from base 10 to base 16.
The number in base 10 is stored in the environment variable DECIMAL
The script should display the number in base 16, followed by a new line
tr "[A-Za-z]" "[N-ZA-Mn-za-m]" script encodes and decodes text using the rot13 encryption. Assume ASCII.
paste - - | cut -f 1 script prints every other line from the input, starting with the first line.
printf "%o\n" $(( 5#$( echo $WATER | tr "water" "01234") + 5#$( echo $STIR | tr "stir." "01234" ) )) | tr "01234567" "bestchol" script adds the two numbers stored in the environment variables WATER and STIR and prints the result.
WATER is in base water
STIR is in base stir.
The result should be in base bestchol
