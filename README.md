# FAT32
This is a user space shell application that interprets a FAT32 file system image and allows users to open files, change directories, and display information about the filesystem . The user can open and close a FAT32 .img file, as well as execute basic commands such as ls, cd, info etc...


# open
close
info
stat
get
cd
ls
read


# Implemented Commands
<br>


## open `<image name>`
Opens fat32.img file with error handling

<br>



## close
Closes fat32.img with error handling

<br>


## info
Print out values for:
BPB_BytesPerSec
BPB_SecPerClus
BPB_RsvdSecCnt
BPB_NumFATS
BPB_FATSz32

<br>


## stat `<filename>`
Print attributes and starting cluster number of the file or directory name. 

<br>

  
## get `<filename>`
Retrieves file from the FAT32 image and places it in your cwd (current working directory). If it does not exist, print "Error: File not found."

<br>


## cd `<folder>`
Changes directories similar to a bash shell. Supports '..' to go back to previous directory

<br>


## ls
List directory contents.

<br>

## read `<filename>`
Reads from the given file at the position, in bytes, specified by the position parameter and output the number bytes specified.' Byte is in size 1, use fseek and have the position be used as the offset. Number of bytes is the count to read.

