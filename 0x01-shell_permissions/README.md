su betty: switches the current user to the user betty

whoami : prints the effective username of the current user.

groups: prints all the groups the current user is part of

chown betty hello : change the owner of the file hello to betty

touch hello: creates an empty file named hello

chmod u+x hello: adds execute permission to the owner and the group owner, and read permission to other users, to the file hello.

chmod ug+x,o+r hello: Write a script that adds execute permission to the owner and the group owner, and read permission to other users, to the file hello.

chmod ugo +x hello: Write a script that adds execution permission to the owner, the group owner and the other users, to the file hello
