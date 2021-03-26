# weather
Linux lab week 11

This project will, once installed, find a weather report for you and store it in /etc/motd.
The weather report will be checked 5 minutes after your system boots up, and then every hour it
remains up after that.

========Getting Started========
===================

1. Clone this repository into your linux machine, preferably somewhere in your home directory.
2. Create a bin directory in your home directory, if one does not already exist.

========Installing========
===================

1. Move or copy the file "wthr" into your bin directory, in your home directory.
2. Inside of your bin directory, type the following command:

	chmod 777 wthr
	
4. Move or copy the file "weather.service" into your "/etc/systemd/system" directory.
5. Move or copy the file "weather.timer" into your "/etc/systemd/system" directory.
6. Run the following commands:

	sudo systemctl enable weather.service
	
	sudo systemctl enable weather.timer
	
	sudo systemctl daemon-reload

========Authors========
===================

Bryan Rainbow
