
# Utility Scripts

## Overview

This repository contains some utility scripts:

1. `nodeModulesRemove.sh` - A script to recursively remove all `node_modules` directories within a specified directory.
2. `malware_scan.sh` - A script to scan a directory for malware using ClamAV.

## Scripts

### 1. Node modules remove

#### Description

This script removes all `node_modules` directories within a specified directory. This can be useful for cleaning up disk space or resetting dependencies in a project.

#### Usage

```sh
./nodeModulesRemove.sh DIRECTORY_PATH
```

#### Parameters

- `DIRECTORY_PATH`: The path to the directory where you want to remove `node_modules`.

#### Example

```sh
./nodeModulesRemove.sh /path/to/your/project
```

#### Help

To display the help message:

```sh
./nodeModulesRemove.sh -h
```

### 2. Malware Scan

#### Description

This script scans a directory for malware using ClamAV. It recursively scans all files in the specified directory and logs the results.

#### Usage

```sh
./malware_scan.sh -d DIRECTORY_PATH -l LOG_FILE
```

#### Parameters

- `-d DIRECTORY_PATH`: The path to the directory to scan.
- `-l LOG_FILE`: The path to the log file where the scan results will be saved.

#### Example

```sh
./malware_scan.sh -d /path/to/your/site -l /path/to/log/file.log
```

#### Help

To display the help message:

```sh
./malware_scan.sh -h
```

## Implementation

1. **Clone the Repository**:

   ```sh
   git clone https://github.com/DHsustainer/utility-scripts.git
   cd tools
   ```

2. **Make Scripts Executable**:

   ```sh
   chmod +x nodeModulesRemove.sh
   chmod +x malware_scan.sh
   ```

3. **Run the Scripts**:

   Follow the usage examples provided for each script to run them.

## Notes

- Ensure you have the necessary permissions to execute the scripts and to access the directories specified.
- The `malware_scan.sh` script requires ClamAV to be installed on your system. Install it using your package manager (e.g., `sudo apt-get install clamav`).

For any issues or contributions, please open an issue or a pull request on the GitHub repository.

## License

This project is licensed under the MIT License.
