To setup the bash script, run this to create the script file: sudo nano /usr/local/bin/move_old_logs.sh
Next make the script executable: sudo chmod +x /usr/local/bin/move_old_logs.sh
To run this everyday at 2 am, edit the crontab using: crontab -e 
Next add this to the crontab file: 0 2 * * * /usr/local/bin/move_old_logs.sh
