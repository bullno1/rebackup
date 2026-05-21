# rebackup

A collection of scripts to automatically backup a remarkable's data locally on plug in.

# Usage

Run `./setup` once which will setup the udev rule and systemd unit to do backup on plugging in.

Run `./backup` to do a manual backup.

The backups will be stored at `~/remarkable-backups/<device-id>/<timestamp>`.
Duplicated files will be hard linked from the previous backup to save disk space.
