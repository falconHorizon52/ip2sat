# iptosat

IPtoSAT plugin
- It converts the IPTV channel as if it is a satellite channel, for example, you will see the beinsport channel on IPTV as if you are watching the one on Nilesat with EPG and signal.

- signal for the channel to work is necessary, and the channel must be encrypted

- You do not need the channel id, only the name of the channel on the satellite and the channel link from your IPTV file.
- This is the channel link from the m3u file, just open your file and take the channel link and put it in front of the url
- Like this is the bein sport 1 link in a file

Code:
http://sarhantv.xyz:25461/free/free99/3

Put it like this

Code:
{
     "playlist":[{
         "channel":"beIN SPORTS HD1",
         url: http://sarhantv.xyz:25461/free/free99/3

     }]
----------------------------------------------------------------------------------------	 
Update 1.1

- Stop the channel after the signal goes out
- Some improvements
-----------------------------------------------------------------------------------------
Update 1.2

- Added reader choice between gstplayer and exteplayer3
(After changing the reader, restart enigma2)
-----------------------------------------------------------------------------------------
update 1.3

- Fix the problem of working the plugin twice when entering
- Stopping the channel as soon as the signal goes away, or vice versa, restarting it after the signal returns
-----------------------------------------------------------------------------------------
Update 1.4

- Fix not working suptv problem and some links
-----------------------------------------------------------------------------------------
Update 1.5

- Dreamos OK
-----------------------------------------------------------------------------------------
Update 1.6

- Add a feature to set a channel with an iptv link
- The subscription type must be from the xtream panel
- First we put our subscription information in

Code:
/etc/enigma2/iptosat.conf

like this

[IPtoSat]
Host=http ://host:port
User=user
Pass=pass

Then we enter the feature
Then we choose the favourites
On the right-hand menu, our subscription packages will appear
We move with the right button and press ok on the appropriate package
Press ok to set the channel
Everything is fine. We will find the channel added in the iptosat.json file with ease
Suppose you entered the BEIN_SPORT_4K package by mistake
All you have to do is press the exit button and it will take you back to choosing packages again

-----------------------------------------------------------------------------------------
Update 1.7

- Access to favorites and satellites
- Possibility to delete a channel or all channels from the iptosat.json file
green button to show moon
And blue for favourites
For the list of satellites and favorites, the ch up and down buttons are activated to move between pages
When entering the feature to delete a channel or all channels, the channels that were previously set will appear with us
Green button to select one channel
Red button to select all channels

-----------------------------------------------------------------------------------------
Update 1.8

- Crash handling when pressing chUP/chDown button
- Added new reader for Dreamos images (Thanks audi06_19)
-----------------------------------------------------------------------------------------
