To run this everyday at 2 am, edit the crontab using: crontab -e 
Next add this to the crontab file: 0 2 * * * /usr/local/bin/move_old_logs.sh
