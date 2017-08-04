# system-backup
This script either generates a system wide backup and/or moves the resulting
backup file to a specified location. rsync is used to move the file, as the
original idea was to transfer the backup to a remote location.

## Usage

Running this script with the backup argument should be done as root,
otherwise protected files will not be backed up.

```bash
system-backup [argument]
```

### Arguments

The script must be called with one of the following arguments:

| Argument | Description                                  |
|----------|----------------------------------------------|
| backup   | Backup the whole system to a .tar.gz file.   |
| archive  | Move the backup file to an archive location. |
| all      | Perform both backup and archive actions.     |
