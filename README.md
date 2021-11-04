# Unix-way eye saver

Shows a simple notification. 50 minutes of work, 10 minutes of rest.

## How to setup?

1) Run `crontab -e`
2) Add this lines to the end of the file

```
50 * * * * DISPLAY=:0.0 notify-send "Time to relax" "10 min" --expire-time=600000 -i important`

0,5,10,15,20,25,30,35,40,45,50,55 23,0,1 * * * DISPLAY=:0.0 notify-send "Time to relax" "Good bye!" --expire-time=600000 -i sleep
3,33 23,0,1 * * * systemctl suspend
```

3) Save & exit
4) Run `sudo service cron reload`

## How to change the icon?

Use any icon from `/usr/share/icons/` instead of `important`.
