# Cheet Sheet For All Linux Command For Daily Use


## Linux Commands List

### Hardware Information

Show bootup messages:
````
dmesg
````
See CPU information:
````
cat /proc/cpuinfo
````
Display free and used memory with:
````
free -h
````
List hardware configuration information:
````
lshw
````
See information about block devices:
````
lsblk
````
Show PCI devices in a tree-like diagram:
````
lspci -tv
````
Display USB devices in a tree-like diagram:
````
lsusb -tv
````
Show hardware information from the BIOS:
````
dmidecode
````
Display disk data information:
````
hdparm -i /dev/disk
````
Conduct a read-speed test on device/disk:
````
hdparm -tT /dev/[device]
````
Test for unreadable blocks on device/disk:
````
badblocks -s /dev/[device]
````
Run a disk check on an unmounted disk or partiti
````
fsck [disk-or-partition-location]
````

### Searching
Search for a specific pattern in a file with grep:
````
grep [pattern] [file_name]
````
Recursively search for a pattern in a directory:
````
grep -r [pattern] [directory_name]
````
Find all files and directories related to a particular name:
````
locate [name]
````
List names that begin with a specified character [a] in a specified location [/folder/location] by using the find command:
````
find [/folder/location] -name [a]
````
See files larger than a specified size [+100M] in a folder:
````
find [/folder/location] -size [+100M]
````

### File Commands
List files in the directory:
````
ls
```
List all files (shows hidden files):
````
ls -a
```
Show directory you are currently working in:
````
pwd
```
Create a new directory:
````
mkdir [directory_name]
```
Remove a file:
````
rm [file_name]
```
Remove a directory recursively:
````
rm -r [directory_name]
```
Recursively remove a directory without requiring confirmation:
````
rm -rf [directory_name]
```
Copy the contents of one file to another file:
````
cp [file_name1] [file_name2]
```
Recursively copy the contents of one file to a second file:
````
cp -r [directory_name1] [directory_name2]
```
Rename [file_name1] to [file_name2] with the command:
````
mv [file_name1] [file_name2]
```
Create a symbolic link to a file:
````
ln -s /path/to/[file_name] [link_name]
```
Create a new file using touch:
````
touch [file_name]
```
Show the contents of a file:
````
more [file_name]
```
Show the contents of a file with cat command:
````
cat [file_name]
```
Append file contents to another file:
````
cat [file_name1] >> [file_name2]
```
Display the first 10 lines of a file with head command:
````
head [file_name]
```
Show the last 10 lines of a file with tail command:
````
tail [file_name]
```
Encrypt a file:
````
gpg -c [file_name]
```
Decrypt a file:
````
gpg [file_name.gpg]
```
Show the number of words, lines, and bytes in a file using wc:
````
wc
```
List number of lines/words/characters in each file in a directory with the xargs command:
````
ls | xargs wc
```
Cut a section of a file and print the result to standard output:
````
cut -d[delimiter] [filename]
```
Cut a section of piped data and print the result to standard output:
````
[data] | cut -d[delimiter]
```
Print all lines matching a pattern in a file:
````
awk '[pattern] {print $0}' [filename]
```
Overwrite a file to prevent its recovery, then delete it:
````
shred -u [filename]
```
Compare two files and display differences:
````
diff [file1] [file2]
```
Read and execute the file content in the current shell:
````
source [filename]
```
Sort file contents and print the result in standard output:
````
sort [options] filename
```
Store the command output in a file and skip the terminal output:
````
[command] | tee [filename] >/dev/null
```














