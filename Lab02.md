## Lab 02

- Name: Kevin Turcios
- Email: turcios.2@wright.edu

## Part 1 Answers

Command to SSH to AWS instance:
```
ssh -i /Users/mag/ceg2350.pem ubuntu@3.81.181.159
```

## Part 2 Answers

1. `chmod u+r bubbles.txt`
    - Means: performing this command grants the user and owner of the bubbles.txt file read privileges.
2. `chmod u=rw,g-w,o-x banana.cabana`
    - Means: this command grants the user reading and writing permissions, it removes the writing permissions for the group and removes the execute permissions of any other users not in the group.
3. `chmod a=w snow.md`
    - Means: this sets all users with only write permissions for the file snow.md.
4. `chmod 751 program`
    - Means: in this command the numbers allow for a numeric mode to grant permissions to the program file/directory. 7 means the owner will get read, write, and execute permissions. 5 means the group will get read and execute permissions. 1 means other users will get the execute permission only.
5. `chmod -R ug+w share`
    - Means: this command will grant user and group with write permissions and apply them recursively to all files or subdirectories in the share file/directory. 

## Part 3 Answers

1. Command to create new user: `sudo adduser kturcios`
2. Path to user's home directory: `/home/kturcios`
3. Evaluate if `ubuntu` can add files to user's home directory: ubuntu cannot add files to bob's home directory, the default permissions don't allow for this to occur.
4. Command to switch to user: `su - kturcios`
5. Command(s) to go to user's home directory: `cd /home/kturcios`
6. Evaluate if user can add files to user's home directory: `touch testfile.txt` was applied and then `ls` showed file was in home directory, so yes user can add files. 
7. Command to switch to `ubuntu`: `exit`
8. Command to return to `ubuntu` home directory: `cd ~`

## Part 4 Answers

For each, write the command used or answer the question posed.

1. Command to create group named `crew`: `sudo groupadd crew`
2. Command(s) to add `ubuntu` & user to group `crew`: `sudo usermod -aG crew ubuntu` `sudo usermod -aG crew kturcios`
3. Command to modify `share` to have group ownership of `crew`: `sudo chown -R :crew /home/ubuntu/share`
4. Command to switch to user: `su - kturcios`
5. Command to add file to `share`: 
6. Evaluate why these steps allowed the above action: 

## Part 5 Answers

For each, write the command used or answer the question posed.

1. Command to create file using `sudo`: `touch sudowho.txt`
2. Evaluate (in plain text) the permission of the file: owner can read and write, group can read and write and others can r only.
3. Provide a method to edit the file without modifying permissions: `sudo nano /home/ubuntu/sudowho.txt`
4. Command(s) to modify permissions: `sudo chown ubuntu:crew /home/ubuntu/sudowho.txt`

## Citations

Using Microsoft Copilot- prompt `chmod 751 program` was used to determine the octal representations. 