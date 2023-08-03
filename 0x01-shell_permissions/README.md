su betty: switches the current user to the user betty

whoami : prints the effective username of the current user.

groups: prints all the groups the current user is part of

chown betty hello : change the owner of the file hello to betty

touch hello: creates an empty file named hello

chmod u+x hello: adds execute permission to the owner and the group owner, and read permission to other users, to the file hello.

chmod ug+x,o+r hello: Write a script that adds execute permission to the owner and the group owner, and read permission to other users, to the file hello.

chmod ugo +x hello: Write a script that adds execution permission to the owner, the group owner and the other users, to the file hello

chmod 007 hello : sets the permission to the file hello as follows:
	Owner: no permission at all
	Group: no permission at all
	Other users: all the permissions

chmod 753 hello : sets the mode of the file hello to this:
	-rwxr-x-wx 1 julien julien 23 Sep 20 14:25 hello
	The file hello will be in the working directory
	You are not allowed to use commas for this script


chmod --reference=olleh hello : sets the mode of the file hello the same as olleh’s mode.
	The file hello will be in the working directory
	The file olleh will be in the working directory

find . -type d -exec chmod ugo+rx {} + :adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users

12-directory_permissions : Create a script that creates a directory called my_dir with permissions 751 in the working directory.

