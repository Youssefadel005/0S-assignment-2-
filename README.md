
# Backup Script - Ubuntu Instructions

## Description
This script automatically creates periodic backups of a directory.
Old backups are deleted once the maximum count is reached.

## Usage
1. Give execute permission:
   chmod +x backup.sh

2. Run manually:
   ./backup.sh <source_dir> <backup_dir> <interval_seconds> <max_backups>

Example:
   ./backup.sh ./mydata ./backups 60 5

3. Run via Makefile:
   make run

4. To clean all backups:
   make clean

## Notes
- Works on Ubuntu (tested on bash 5.1)
- Uses tar to create compressed .tar.gz archives
- Script runs continuously — press Ctrl+C to stop
