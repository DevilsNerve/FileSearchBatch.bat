# File Search Batch Script

This batch script allows users to search for files in a directory based on a specified file type, date range, and keyword. It provides a convenient way to locate files that match specific criteria within a given directory.

## Code Explanation

The provided batch script includes comments to explain each section of the code. Here is a breakdown of its functionality:

- The script starts with the `@echo off` command to turn off command echoing, ensuring that the commands executed in the script are not displayed in the command prompt.
- The `title Created by Austen Green` command sets the title of the command prompt window.
- The `setlocal` command limits the scope of variable changes to the current batch script.
- The script prompts the user to enter the search directory, file type, start date, end date, and keyword using the `set /p` command. The user's input is assigned to corresponding variables.
- The `start_time` variable is set to the current time using the `%time%` system variable.
- A `for` loop searches for files in the specified directory and file type. It uses the `findstr` command to search for the keyword within the file contents. If the keyword is found, the file path is printed. If the keyword is not found in the file contents, the file path is checked again using `findstr` to search for the keyword in the file name. If the keyword is found, the file path is printed.
- The `end_time` variable is set to the current time using the `%time%` system variable.
- The `time_diff` variable is calculated by converting the start and end times to seconds and subtracting them.
- The script prints a message indicating that the search is complete and displays the time taken to complete the search using the `echo` command. The `pause` command keeps the command prompt window open until the user presses a key.

## Example Usage

To use the batch script, follow these steps:

1. Save the script with a `.bat` file extension (e.g., `file_search.bat`).
2. Open a command prompt window and navigate to the directory where the script is saved.
3. Run the script by entering its filename (e.g., `file_search.bat`).
4. Follow the prompts and enter the required information:
   - Enter the search directory (e.g., `C:\Users\JohnDoe\Documents`).
   - Enter the file type to search (e.g., `*.docx`).
   - Enter the start date for the search in the format MM/DD/YYYY (e.g., `01/01/2021`).
   - Enter the end date for the search in the format MM/DD/YYYY (e.g., `12/31/2021`).
   - Enter the keyword to search for (e.g., `confidential`).
5. The script will search for files that match the specified criteria and display the file paths. It will also provide the time taken to complete the search.

Please note that this script is designed to be executed in a Windows command prompt environment.

Feel free to customize and integrate this script into your workflow to enhance file search capabilities.

