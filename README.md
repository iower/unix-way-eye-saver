# Unix-way eye saver

Shows a simple notification. 50 minutes of work, 10 minutes of rest.

## How to setup?

1) Run `crontab -e`
2) Add this line to the end of the file

`50 * * * * DISPLAY=:0.0 notify-send "Time to relax" "10 min" --expire-time=600000 -i important`

3) Save & exit
4) Run `sudo service cron reload`

## How to change the icon?

Use any icon from `/usr/share/icons/` instead of `important`.
