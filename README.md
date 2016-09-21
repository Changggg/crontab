# 
Crontab is way by which we can schedule a system job at certain intervals.

To know more about crontab visit this blog for better understanding [click here](http://www.thegeekstuff.com/2011/07/cron-every-5-minutes/?utm_source=feedburner&utm_medium=feed&utm_campaign=Feed%3A+TheGeekStuff+(The+Geek+Stuff)) 


To run a crontab job,first we need to create the script which we want execute. We have 2 crontab jobs in our system pull_data_weekly[see code](https://github.com/ou-ecolab/crontab/blob/master/pull_data_weekly) and weekly_forecast[see code](https://github.com/ou-ecolab/crontab/blob/master/weekly_forecast). These scripts are located in /home/ecopad/services/crontab_ecolab . 


Schedule the crontab jobs
-----------------------------

SSH to the system and type

`# crontab -e`

Insert the following 2 lines

`# 5  23 * * 0 /path_to_pull_data_weekly `

`# 30 23 * * 0 /path_to_weekly_forecast `
