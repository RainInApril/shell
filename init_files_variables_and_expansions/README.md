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
