# OINP-Monitor
A python script that checks for OINP update every 20s and notify you by sending a text message with Twilio

Running Environment: Raspberry Pi 3 Model B, Raspbian Linux 4.9, Python 2.7.13

Python Libraries Needed:
* pickle
* urllib3
* BeautifulSoup
* time
* logging
* twilio

Other Utility Needed:
* cron

How to Implement:
1. Install Python 2.7 and all libraries/utilities needed
1. Put `OINP.py` and `OINP.pickle` in a folder of your choice.
1. Schedule a cron task to run `OINP.py` every 10 mins: `*/10 * * * * python /home/pi/python_scripts/OINP.py`
1. Schedule a cron task to reboot the computer everyday at midnight to prevent crashes: `0 0 * * * sudo reboot`
