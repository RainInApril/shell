pwd prints the absolute path name of the current working directory
ls displays the contents list of current directory
cd changes the working directory to the user's home directory
ls -l displays current directory contents in a long format
ls -la displays current directory contents, including hiddden files (starting with .) in long format
ls -lna displays current directory contents in long format, with user and group IDs displayed numerically and hidden files (starting with .)
mkdir /tmp/my_first_directory creates a directory named my_first_directory in the tmp directory
mv /tmp/betty /tmp/my_first_directory moves the file betty from /tmp/ to /tmp/my_first_directory
rm /tmp/my_first_directory/betty deletes the file betty
rm -r /tmp/my_first_directory deletes the directory my_first_directory that is in the /tmp directory
cd - changes the working directory to the previous one
ls -la . .. /boot lists all files in the current directory and the parent of the working directory and the /boot directory (in this order), in long format
file /tmp/iamafile prints the type of file named iamafile
ln -s /bin/ls __ls__ creates a symbolic link named __ls__ in the current working directory
cp -u *.html .. copies all the HTML files from the current working directory to the parent of the working directory, but only copy files that did not exist in the parent of the working directory or were newer than the versions in the parent of the working directory.
mv [[:upper:]]* /tmp/u moves all files beginning with an uppercase letter to the directory /tmp/u
rm *~ deletes all files in the current working directory that end with the character ~
