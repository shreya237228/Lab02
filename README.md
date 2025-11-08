

# Part 1 - Creating Directories

Use mkdir to create the following directories. Remember the -p option:
```
project
    ├── archives     
    ├── documents
        └── frontend
        └── backend
    ├── pictures
        └── jan
        └── feb
        └── march
    └── programs
        └── tools
        └── fun
```
# Part 2 - File Creation

Use touch to create files at the following locations:
```
project
    ├── archives
    ├── documents
        └── frontend
            └── design.txt
            └── issues.txt
        └── backend
            └── api.txt
            └── issues.txt
    ├── pictures
        └── jan
            └── locations.txt
        └── feb
            └── locations.txt
        └── march
            └── locations.txt
    └── programs
        └── tools
        └── fun
```
# Part 3 - File/Directory Operations

## Tasks
+ Use mv to move the pictures into the correct folders, use ls or find to check the modified date.
+ Soft Link compile.sh to the tools folder
+ Hard Link moosay.sh to the fun folder
+ Move compile.sh and moosay.sh to programs folder.
    + Not the linked versions but the original ones in the root of this repository.
+ Execute moosay.sh and compile.sh from the programs/tools and programs/fun directories
    + Should they both still work? only hardl;ink works, softink is broken since the file was moved
+ Archive the documents, pictures, and programs folders and put the archives into the archives folder. You can use zip or tar to create the archive.
    + Shortcut: Use the find command to find all .zip or .tar files and use the -exec option to move them

# Part 4 - Temp Files and Directories

## Tasks
+ Use mktemp to create 3 new temporary directory in the projects direcotry
    + Hint: Use the manpage and look for the -p and -d options
+ Use mktemp to create a temporary file in one of the temporary directories
+ Use rmdir to remove all empty tmp directories
    + Hint: Use a wildcard `*` to do this in one command.
+ Use rm to remove the remaining temporary directory and file.
