### btlnet-BonusChallengeA
###  Answer to Bonus Question


#Author:   Cornel Earle
#Date:  19 June 2022   04:18am
# Purpose of script  - To create a cron file which will watch the /etc/passwd file every 15 minutes for changes or access


SHELL=/bin/bash
PATH=/sbin:/bin:/usr/sbin:/usr/bin


#  run cronjob every 15 minutes
*/15 * * * *   -w /etc/passwd -p wa -k /var/log
