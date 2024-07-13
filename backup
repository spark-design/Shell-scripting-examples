#!/bin/bash

# Source and destination directories
SOURCE_DIR="/var/log"
BACKUP_DIR="/backup/logs"

# Create backup directory if it doesn't exist
mkdir -p $BACKUP_DIR

# Find and move logs older than 30 days
find $SOURCE_DIR -type f -name "*.log" -mtime +30 -exec mv {} $BACKUP_DIR \;

# Optional: Add a log entry for this action
echo "$(date): Moved logs older than 30 days from $SOURCE_DIR to $BACKUP_DIR" >> /var/log/move_old_logs.log
