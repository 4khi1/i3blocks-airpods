# i3blocks-airpods 💃🕺
i3blocks script for managing airpods and airpods pro.  
I love airpods 😃

## Controls
<b>left click:  </b> connect to airpods  
<b>middle click:</b> toggle A2DP or HSP/HFP  
<b>right click: </b> disconnect airpods

## Showcase
![i3blocks airpods](showcase.gif)

## Dependencies
```
   1.ofono.service  # systemd
   2.ofono-phonesim  
       sudo add-apt-repository ppa:smoser/bluetooth  
       sudo apt-get install ofono-phonesim  
   3.git clone https://github.com/rilmodem/ofono.git /opt/ofono  
```

## Tweak the script for first time
replace MAC and card name in the script
```
AIRPODS_MAC='4C:6B:E8:80:46:84' # it should be somewhere in blueman-manager  
AIRPODS_NAME='bluez_card.4C_6B_E8_80_46_84' # you can find this using 'pactl list cards' command  
```

## i3blocks.conf
```
[airpods]
command=/path/to/airpods
label=🎧 
interval=10
```

## Notice
you should first pair your airpods using blueman and trust them

## Discussion
https://www.reddit.com/r/i3wm/comments/hsx3l3/got_airpods_lets_setup_i3blocks_for_it/

## Contributions are welcome

## Say thanks:
  
  Just letting me know you're enjoying this plugin is a great way to say thanks!
  
  You can do so by staring the GitHub repo.
  
## Troubles?
  
  If you have any kind of trouble with it, just let me now by raising an issue on
  the GitHub issue tracker here:

  It should be there 👆 👀
