# File Organizer Script
## Overview
This Python script organizes files from a source folder into subfolders based on their categories. It classifies files into the following categories: Pictures, Music, Documents, Videos, and Others. Additionally, it organizes files further into subfolders based on their file extensions.

## Prerequisites
- Python 3.6 or above
- Required Python packages can be installed using:
```sh
$ pip3 install termcolor aiofiles

```
## Usage
## Command-line Arguments
- source_folder: Path to the source folder containing the files to be organized.
- destination_folder: (Optional) Path to the destination folder for organizing files.
- If not provided, the script will use the current working directory.
## Running the Script
1- Open a terminal or command prompt.
2- Navigate to the directory containing the script.
3- Run the script with the following command:
```py
python3 organizer.py <source_folder> <destination_folder> 
```
3- The script will organize files based on their categories and move them to the specified destination folder or create subfolders in the current working directory.

## Additional Information
- The script recognizes various file types such as:
  - images (JPG, JPEG, PNG, GIF, BMP, TIFF, WEBP, SVG).
  - music (MP3, WAV, OGG, FLAC, AAC, M4A).
  - documents (PDF, ZIP, RAR, 7Z, EXE, DEB, ISO).
  - videos (MP4, AVI, MKV, MOV, WMV, WEBM), and other miscellaneous file types.
File extensions with unsupported types are categorized as "Other."
The script handles the sanitization of filenames, removing specific characters (except underscores) and replacing hyphens with underscores.
## Example:
```py
$ python3  orgnaizer.py Downloads/
```
## Result
```sh
Report:
Execution Time: 1.13 seconds
Category Counters:
Documents: 414 files
Other: 42 files
Pictures: 2 files
Videos: 10 files
Documents/Office: 5 files
Music: 2 files
Total Files Moved: 475
Total Size Moved: 12.39 GB
Script executed successfully.

```

