Exercise 1a: make another directory inside the “unixstuff” directory called “backups”

Exercise 1b: Use the commands cd, ls and pwd to explore the file system. (Remember, if you get lost, type cd by itself to return to your home-directory)

Exercise 2a: Create a backup of your science.txt file by copying it to a file called science.bak
To create a backup of your science.txt file by copying it to a new file called science.bak, use the cp command in Unix.
Command: cp science.txt science.bak




Exercise: We are now going to move the file science.bak to your backup directory.






Exercise 2b: Create a directory called tempstuff using mkdir , then remove it using the
rmdir command.

Bellow screen short shows the tempstuff directory is created using mkdir command 




Bellow screen short shows that tempstuff directory is deleted using rmdir command



Q. How can you view the last 15 lines of the file?
To view the last 15 lines of a file in Unix, use the tail command with the -n option:
Command: tail -n 15 filename
Example: tail -n 15 science.txt

This will display the last 15 lines of the file science.txt.

Q.What difference did the -5 do to the head command?
In Unix, the -5 option with the head command changes the number of lines displayed.
By default, head shows the first 10 lines of a file.
When you add -5, it tells head to show only the first 5 lines of the file.
Example: head -5 filename

Exercise 3a: Using the above method, create another file called list2 containing the following fruit: orange, plum, mango, grapefruit. Read the contents of list2

The list2 file is created in home directory as bellow



Exercise 3b: Using pipes, display all lines of list1 and list2 containing the letter 'p', and sort the result.
To display all lines of list1 and list2 containing the letter 'p', and then sort the result using pipes, you can use the following command: cat list1 list2 | grep "p" | sort

Explanation:
1.cat list1 list2: Combines the contents of both list1 and list2.
2.grep "p": Filters the lines that contain the letter 'p'.
3.sort: Sorts the filtered lines alphabetically.
This will display all lines from list1 and list2 that contain 'p', sorted in order.

Exercise 5a: Try changing access permissions on the file science.txt and on the directory backups. Use ls -l to check that the permissions have changed.
Changing access permissions on file as bellow
1.Remove write permission on user on science.txt file: chmod u-w science.txt 

2.Remove read and write permission for group and others on science.txt file:          chmod go-rw science.txt

3.Give all permissions for users (owner, group and others) on science.txt file:          chmod a+rw science.txt

Changing access permissions on directory as bellow
1.Remove write permission on user on backups directory: chmod u-w backups

2.Give read and write permissions to the owner and group on a directory backups:           chmod u+rw,g+rw backups

3.Remove execute permission for others: chmod o-x directory_name

4.Give all permissions for users (owner, group and others) on backups directory:          chmod a+rw backups and chmod a+rwx backups 
