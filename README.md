raspberry-gpi-shutdown
======================

Python script that shutdown or reboot raspberry pi from gpio pins


PREREQUISITES:
==============
Run this commands to install dependencies:
 sudo apt-get install python-dev
 wget http://pypi.python.org/packages/source/R/RPi.GPIO/RPi.GPIO-0.4.1a.tar.gz
 tar xvfz RPi.GPIO-0.4.1a.tar.gz
 sudo python setup.py install

HOW TO INSTALL: 
===============
1. Put this script in /home/pi/bin/shutdown.py
2. Edit /etc/rc.local and add this
	line just before "exit 0" statment:
	python /home/pi/bin/shutdown.py &
3. Shutdown raspberry
4. Connect gpio 17 and 18 to both switches
5. Reboot raspberry
6. Be happy!
