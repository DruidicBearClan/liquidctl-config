# liquidctl-config
systemd service files for controlling hardware with RGB headers.
The settings work for only my setup, don't recommend using those, you can use the template.

The liquidcfg.service file is for enabling liquidctl at boot with my desired settings.
The liquidcfg-suspend.service file is for resuming liquidctl with those settings from suspend/sleep mode.


Shoutout to the liquidctl devs for their tool
https://github.com/liquidctl

For more documentation see: 
https://github.com/liquidctl/liquidctl#set-up-linux-using-systemd

remember to reload systemctl daemon and start/enable your new service

systemctl daemon-reload
systemctl start liquidcfg.service
systemctl enable liquidcfg.service 

or liquidcfg-suspend.service
