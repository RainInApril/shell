su betty script switches the current user to the user betty
whoami script prints the effective username of the current user
groups script prints all the groups the current user is part of
chown betty hello script changes the owner of the file hello to the user betty
touch hello creates an empty file called hello
chmod u+x hello script adds execute permission to the owner of the file hello
chmod ug+x,o+r hello script adds execute permission to the owner and the group owner, and read permission to other users, to the file hello
chmod +x hello script adds execution permission to the owner, the group owner and the other users, to the file hello
chmod 007 hello script sets the permission to the file hello as follows:
Owner: no permission at all
Group: no permission at all
Other users: all the permissions
chmod 753 hello script sets the mode of the file hello to this:
-rwxr-x-wx 1 julien julien 23 Sep 20 14:25 hello
The file hello will be in the working directory
You are not allowed to use commas for this script
chmod --reference=olleh hello script copies hello file permissions to file olleh
chmod -R +X . script adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users. Regular files should not be changed.
mkdir -m 751 my_dir script creates a directory called my_dir with permissions 751 in the working directory
chgrp school hello script changes the group owner to school for the file hello
chown vincent:staff * script changes the owner to vincent and the group owner to staff for all the files and directories in the working directory
chown -h vincent:staff _hello script changes the owner and the group owner of _hello to vincent and staff respectively
The file _hello is in the working directory
The file _hello is a symbolic link
