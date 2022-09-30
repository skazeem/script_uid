# script_uid
#!/bin/bash
username=`cat /etc/passwd | grep $1 | awk -F: '{ print $1 }'`
last | grep $username | wc -l
