# Ubuntu Backup & Mini Shell Assignment

## Part 1 — Automatic Backup Script

### Description
A Bash script that creates automated, periodic backups of a directory.  
Older backups are deleted once the max count is reached.

### How to Use (Ubuntu)
1. Make it executable:
   chmod +x backup.sh

2. Run manually:
   ./backup.sh ./data ./backups 60 5

   - `./data` is the folder to back up  
   - `./backups` is the destination  
   - `60` = backup every 60 seconds  
   - `5` = keep only the 5 most recent backups  

3. Or use Makefile:
   make prepare
   make backup

4. Stop anytime using:
   Ctrl + C

---

## Part 2 — Mini Shell

### Description
A simple Linux shell written in C that can execute commands using `fork()` and `execvp()`.

### Run (Ubuntu)
1. Compile:
   make shell

2. Example usage:
