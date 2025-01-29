## Lab 01

- Name: Kevin Turcios
- Email: turcios.2@wright.edu

## Part 1 - GitHub Profile

1. [turcioskevin Profile](https://github.com/turcioskevin/turcioskevin)

## Part 2 - Research

| Windows | Linux / Mac | Action |
| ---     | ---         | ---    |
| help    | man         | gives info on what a command can do and how to format |
| Get-Location | pwd    | gives you the path of whatever item |
| Get-ChildItem | ls    | gets the items in one or more specified locations |
| mkdir   | mkdir       | lets you create a directory or multiple |
| Set-Location | cd     | used to change directory |
| New-Item | touch      | creates a new item and sets the value |
| Move-Item | mv        | moves an item and everything that comes with it to wherever you set to |
| Copy-Item | cp        | copies an item from a location to whatever location you set |
| Remove-Item | rm      | deletes one or more items |
| notepad.exe | vim     | Start-Process 'C:\windows\system32\notepad.exe' |

## Part 3 - Command Line Navigation

My OS is:
- [] Windows
- [] Linux
- [x] Mac

My Command Line Shell is: Terminal

### Navigating My OS on the Command Line

1. Create a directory named `DirA`: mkdir DirA
2. Create a directory named `Dir B`: mkdir "Dir B"
3. Go into `DirA`: cd DirA
4. Go into `Dir B` from `DirA`: cd "Dir B"
5. Return to your user's home directory: cd
6. Create a file named `test.txt`: touch test.txt
7. Move the file named `test.txt` into `DirA`: mv test.txt DirA
8. Contents of `test.txt`: 
```
Hello World
```
9. Make a copy of `test.txt` named `copy.txt` in `DirA`: cp test.txt copy.txt
10. View the contents of `DirA`: ls
11. Make a copy of `test.txt` in `Dir B` named `fodder.txt`: cp test.txt fodder.txt -> mv fodder.txt "Dir B"
12. Delete / remove both `fodder.txt` AND `Dir B`: rm fodder.txt rmdir "Dir B" 

## Citations

(https://phoenixnap.com/kb/how-to-copy-files-directories-linux)