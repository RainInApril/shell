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
Words should be sorted
grep root /etc/passwd script displays lines containing the pattern “root” from the file /etc/passwd
grep -c bin /etc/passwd script display the number of lines that contain the pattern “bin” in the file /etc/passwd
