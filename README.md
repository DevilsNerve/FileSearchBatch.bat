# File Search Batch Script

This batch script allows the user to search for files in a directory based on a specified file type, date range, and keyword. It provides a convenient way to locate files that match specific criteria within a given directory. Please note that this script is provided as-is and should be used at your own discretion.

## Usage

1. Make sure you have a Windows operating system installed.
2. Open a text editor and create a new file.
3. Copy the contents of the batch script into the newly created file.
4. Save the file with a `.bat` extension, for example, `file_search.bat`.
5. Double-click on the saved `.bat` file to execute the script.

## Script Explanation

The script contains the following sections and features:

### 1. Echo Off and Title

The `@echo off` command turns off the command echo so that the commands executed in the script are not displayed in the command prompt. The `title Created by Austen Green` sets the title of the command prompt window.

### 2. Variables and Input Prompts

The `setlocal` command limits the scope of variable changes to the current batch script. The script prompts the user to enter the search directory, file type, start date, end date, and keyword using the `set /p` command. These values are assigned to variables for further use in the script.

### 3. File Search

The script uses a `for` loop to search for files in the specified directory and file type. It utilizes the `findstr` command to search for the keyword in the file contents. If the keyword is found, the file path is printed. If the keyword is not found in the file contents, the file path is checked again using the `findstr` command to search for the keyword in the file name. If the keyword is found, the file path is printed.

### 4. Time Calculation

The script calculates the time taken to complete the search. It records the start and end times, converts them to seconds, and calculates the time difference.

### 5. Search Completion Message

After the search is complete, a message is displayed indicating the completion of the search and the time taken to complete it. The `pause` command keeps the command prompt window open until the user presses a key.

## Example Usage

An example usage is provided within the script as comments. It demonstrates how to enter the search directory, file type, date range, and keyword. Modify the example usage to fit your specific search criteria.

## License

This batch script is provided under the following license:

```
MIT License

Permission is hereby granted, free of charge, to any person obtaining a copy of this script, to deal in the script without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the script, and to permit persons to whom the script is furnished to do so, subject to the following conditions:

The script is provided "as is", without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose, and noninfringement. In no event shall the authors or copyright holders be liable for any claim, damages, or other liability, whether in an action of contract, tort, or otherwise, arising from, out of, or in connection with the script or the use or other dealings in the script.

By using this script, you agree to release Austen Green from any responsibility or liability for its usage.

```

Feel free to modify or adapt the script according to your needs. However, please note that the author, Austen Green, is not responsible for any consequences or damages resulting from

 the use of this script. Use it at your own risk.
