## Linux Shell in C++

This project implements a basic Linux shell in C++. It provides the following functionalities:

**Supported Commands:**

* `cd`: Change directory
* `cp`: Copy files
* `mv`: Move files
* `ls`: List files and directories
* `rm`: Remove files and directories

**Command Options:**

Each command offers various options for specific behavior. Here's a breakdown:

**cd:**

* `--help`: Displays help message
* `..`: Returns to the previous directory
* `~`: Changes to the home directory
* `/`: Changes to the root directory
* `<path>`: Changes to the specified path

**cp:**

* `--help`: Displays help message
* `-n`: Prevents overwriting existing files
* `-u`: Copies only if the source file is newer
* `-i`: Prompts before overwriting existing files
* `-a` (or `-R`): Copies recursively, preserving attributes

**ls:**

* `--help`: Displays help message
* `-a`: Lists all entries, including hidden files
* `-R`: Lists subdirectories recursively
* `-Q`: Encloses entries in double quotes
* `-lh`: Lists in long format with human-readable sizes
* `-l`: Lists in long format

**mv:**

* `--help`: Displays help message
* `-i`: Prompts before overwriting existing files
* `-u`: Moves only if the source file is newer
* `-R`: Moves entire directories recursively
* `-n`: Prevents overwriting existing files

**rm:**

* `--help`: Displays help message
* `-d`: Removes empty directories
* `-v`: Explains what is being done
* `-R`: Removes directories and their contents recursively
* `-i`: Prompts before every removal
* `-f`: Forces removal without confirmation

**Multithreading:**

This project utilizes multithreading to improve performance for recursive operations in `ls` and `cp`. We've conducted time difference analysis to measure the impact of multithreading on execution speed.

**Running the project**
- make make_file.txt
- ./shell
