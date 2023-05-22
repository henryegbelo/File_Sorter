# File_Sorter
Automated File Sorter

This script categorizes files in a specified directory based on their extensions and moves them to corresponding folders.

1. Import the necessary modules for working with the operating system and performing file operations.
2. Specify the directory path where the files are located.
3. Define a dictionary that maps file categories to their corresponding extensions.
4. Start a loop that iterates over each file name in the specified directory.
    5. Construct the full path of the file by joining the directory path and the file name.
    6. Check if the item in the directory is a file (not a directory).
    7. Start another loop that iterates over each folder name and its corresponding list of extensions.
        8. Check if the file name ends with any of the specified extensions (ignoring the case).
        9. Construct the full path of the destination folder by joining the directory path and the folder name.
        10. Check if the destination folder does not exist. If it doesn't, create the folder.
        11. Copy the file from the current location to the destination folder.
        12. Break out of the inner loop since the file has been successfully copied.
    13. Repeat this process for each file in the directory, categorizing and copying them based on their extensions.
