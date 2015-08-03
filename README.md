# Projects_streaming
Project_videostreaming


This is just some of the code that I used to stream video from a weather balloon from ground to 95,000 ft.

We used a Ubiquiti Rocket dish with Ubiquiti M5 modems on each side


The pc side was set to static but I think dynamic will work with out too many problems.  The main one is that 
if you want to streamout on the pc side to a computer somewhere you need to know your public IP address and 
make sure that you are using the right video transcoder. 


I used vlc player to do the network recieving and streaming.  There are many different ways to stream but for a cheap 
video player that has a decent gui I found vlc to be the easiest.

The video command shell just uses the Raspberry Pi's pi camera(not python) commands.  

The Raspberry Pi that streams from the balloon needs to have a static IP over the ethernet port (eth0) So that the 
Ubiquiti M5 can communicate with it.  I set mine to 192.168.1.3, this allowed me to have a constant address in case
I needed to restart the Pi in the flight.  
