echo "Hello, World" script prints “Hello, World”, followed by a new line to the standard output
echo "\"(Ôo)'" script displays a confused smiley "(Ôo)'
cat /etc/passwd script displays the content of the /etc/passwd file
cat /ect/passwd /etc/hosts script displays the content of /etc/passwd and /etc/hosts
tail -10 /etc/passwd script displays the last 10 lines of /etc/passwd
head -10 /etc/passwd script displays the first 10 lines of /etc/passwd
head -3 iacta | tail -1 script displays the third line of the file iacta
echo "Best School" > "\*\\\'\"Best School\"\'\\\*$\?\*\*\*\*\*:)" script creates a file named exactly \*\\'"Best School"\'\\*$\?\*\*\*\*\*:) containing the text Best School ending by a new line
ls -la > ls_cwd_content script writes into the file ls_cwd_content the result of the command ls -la. If the file ls_cwd_content already exists, it should be overwritten. If the file ls_cwd_content does not exist, create it.
tail -1 iacta >> iacta script duplicates the last line of the file iacta
find . -type f -name '*.js' -delete script deletes all the regular files (not the directories) with a .js extension that are present in the current directory and all its subfolders
find . -mindepth 1 -type d | wc -l script counts the number of directories and sub-directories in the current directory
The current and parent directories should not be taken into account
Hidden directories should be counted
ls -1t | head -10 script displays the 10 newest files in the current directory
Requirements:
One file per line
Sorted from the newest to the oldest
sort | uniq -u script takes a list of words as input and prints only words that appear exactly once.
Input format: One line, one word
Output format: One line, one word
Words should be sorteod
grep root /etc/passwd script displays lines containing the pattern “root” from the file /etc/passwd
grep -c bin /etc/passwd script display the number of lines that contain the pattern “bin” in the file /etc/passwd
grep -A 3 root /etc/passwd script display lines containing the pattern “root” and 3 lines after them in the file /etc/passwd
grep -v bin /etc/passwd script display all the lines in the file /etc/passwd that do not contain the pattern “bin”
grep ^[[:alpha:]] /etc/ssh/sshd_config script display all lines of the file /etc/ssh/sshd_config starting with a letter.
Include capital letters as well.
tr 'A' 'Z' | tr 'c' 'e' script replace all characters A and c from input to Z and e respectively.
tr -d c | tr -d C script removes all letters c and C from input.
rev script reverse its input.
cut -d : -f1,6 /etc/passwd | sort script displays all users and their home directories, sorted by users.
Based on the the /etc/passwd file.
find . -empty -printf "%f\n" script finds all empty files and directories in the current directory and all sub-directories.

Only the names of the files and directories should be displayed (not the entire path)
Hidden files should be listed
One file name per line
The listing should end with a new line
You are not allowed to use basename, grep, egrep, fgrep or rgrep
find . -type f -name "*.gif" -printf "%f\n" | rev | cut -d "." -f 2- | rev | LC_ALL=C sort -f script lists all the files with a .gif extension in the current directory and all its sub-directories.
Hidden files should be listed
Only regular files (not directories) should be listed
The names of the files should be displayed without their extensions
The files should be sorted by byte values, but case-insensitive (file aaa should be listed before file bbb, file .b should be listed before file a, and file Rona should be listed after file jay)
One file name per line
The listing should end with a new line
You are not allowed to use basename, grep, egrep, fgrep or rgrep
echo $(cut -c 1 | tr -d "\n") script decodes acrostics that use the first letter of each line.
The ‘decoded’ message has to end with a new line
You are not allowed to use grep, egrep, fgrep or rgrep
tail -n +2 | cut -f1 | sort | uniq -c | sort -nr | head -n11 | rev | cut -d" " -f1 | rev script parses web servers logs in TSV format as input and displays the 11 hosts or IP addresses which did the most requests.
Order by number of requests, most active host or IP at the top
You are not allowed to use grep, egrep, fgrep or rgrep
