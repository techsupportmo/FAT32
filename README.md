# FAT32
FAT32 Filesystem Project


# open
close
info
stat
get
cd
ls
read


# Implemented Commands

## open `<image name>`
---
Opens fat32.img file with error handling

# close
Closes fat32.img with error handling

# info
Print out values for:
BPB_BytesPerSec
BPB_SecPerClus
BPB_RsvdSecCnt
BPB_NumFATS
BPB_FATSz32

# stat `<filename>`
Print attributes and starting cluster number of the file or directory name. 
  
# get `<filename>`
Retrieves file from the FAT32 image and places it in your cwd (current working directory). If it does not exist, print "Error: File not found."

# cd `<folder>`
Changes directories similar to a bash shell. Supports '..' to go back to previous directory

# ls
List directory contents.

# read `<filename>`
Reads from the given file at the position, in bytes, specified by the position parameter and output the number bytes specified.' Byte is in size 1, use fseek and have the position be used as the offset. Number of bytes is the count to read.

