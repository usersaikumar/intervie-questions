# Shell Scrpting
- A file called **sh** stores shell programs
- Text files containing commands to execute by a shell are called shell scripts.
- it is considered to be the easiest programming language to use
- Automation of the code compiling process
- Run a program or create an environment for programming.
- Complete batch processing and file manipulation.
- Integrate existing programs.
- Perform routine backups.

##  limitations of shell scripting
- Errors are frequent and costly, and a single error can alter the command.
- The execution speed is slow
- Bugs or inadequacies in the language's syntax or implementation
- Large, complex tasks aren't well suited to it.

## Shell variable
```
variable ="Hello" 
echo $variable
```
## different types of variables
- System-defined variables(**environment variable**)
  - it's in Capital Letters **ex:SHELL**
- User-defined variables
  - it's in lower case **ex:a=10**

## control instructions
- Sequence Control Instruction
- Decision Control Instruction
- Loop Control Instruction
- Case-Control Instruction

## Shortcuts or Links
- soft link
  
  - ```ln  -s [original filename] [link name]```
- Hard Link
  - ```ln [original filename] [link name]``` 

## connect to a database server
```isql –S serverName –U username –P password```
##  the command that is used to execute a shell file.
```
chmod +x script-name-here.sh 
./script-name-here.sh
```
```
sh script-name-here.sh
```
## ShellScript Commands
- echo (reflect same message as we mention)
- tput (alternative command for echo)
- echo $ # (Number of arguments passed through)
- **$?** (status of last command)
- **&** (add at end of command and run in background)
## Examples

https://www.kau.edu.sa/Files/830/Files/60761_Linux.pdf

- How commands will work
```
cd
mkdir bin
```
- To clear a screen and give a comment
```
cat > earse
```
```
# writing my first shell script
clear
echo "your comment"
```
```
chmod +x earse
```
```
./earse
```
```
cp earse ~/bin
```
- To show arguments
```
cat > aruguments
```
```
#!/bin/sh
#
# Script that demos, command line args
#
echo "Total number of command line argument are $#"
echo "$0 is script name"
echo "$1 is first argument"
echo "$2 is second argument"
echo "All of them are :- $*"

```
```
chmod +x arguments
```
```
./arguments
```
```
cp arguments ~/bin
```
- If Condition
```
cat > file_name
```
```
#!/bin/sh
#
#Script to print file
#
if cat $1
then
 echo -e "\n\nFile $1, found and successfully echoed"
fi
```
```
./file_name
```
```
cp fiel_name ~/bin
```
## rules
- looks like
-eq is equal to                 5 == 6    if test 5 -eq 6   if expr [ 5 -eq 6 ]
-ne is not equal to             5 != 6    if test 5 -ne 6   if expr [ 5 -ne 6 ]
-lt is less than                5 < 6     if test 5 -lt 6   if expr [ 5 -lt 6 ]
-le is less than or equal to    5 <= 6    if test 5 -le 6   if expr [ 5 -le 6 ]
-gt is greater than             5 > 6     if test 5 -gt 6   if expr [ 5 -gt 6 ]
-ge is greater than or equal to 5 >= 6    if test 5 -ge 6   if expr [ 5 -ge 6 ]