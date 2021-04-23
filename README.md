# check_file-modification
small icinga/nagios script to check if a file hasn't been modified since X seconds

## Usage: 

```bash
./check_file-modification -f <full path to file> -c <seconds>
```

## Installation:
Just move the file into your plugin directory and add a new command and service to your icinga configuration. Don't forget to grant execution permissions. 

## Output

```
FILE-MODIFICATION OK - last modified: 1 minute, 53 seconds
```

## Example:
Check whether a file was modified 10 minutes (600 seconds) ago:
```bash
./check_file-modification -f /path/to/file -c 600 
```
