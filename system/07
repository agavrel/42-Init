# Figure out the PID of the SSHD service
service ssh status | grep 'Main PID' | awk -F '[ ]' '{print $3" " $4}'
