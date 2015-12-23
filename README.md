# Projects_streaming
Project_videostreaming


This Project is a rough summary of the Video Streaming system that was used in the MSGC Borealis 2015 Summer flights.  The kit is incomplete and there are some works in progress.

We used a Ubiquiti Rocket dish with Ubiquiti M5 modems on each side.  The Rocket dish is set on top of a servo assembly that allows for a rotation of tilt and pan.  We currently are polling a MySQL data base for gps addresses to track.  The servo system was created by a previous Borealis member that has since moved on into industry.

We stream the video to a website and have a connection to a wired ethernet connection.  This requires a wireless adapter of some kind and also a network adapter that uses a ethernet (cat5 or cat7 doesn't matter) cable to communicate with the Ubiquiti Rocket M5 Dish array.

We set up the main streaming pipeline through VLC media player.  In one of the set up files ...... the method to setting up a stream to a ip is explained out in detail.

To start the stream the we use a batch file to run a set of commands that are pre-defined on the Raspian operating system. 
A short example command is shown in the Create Video_streaming_pi_side

Current I am using this set up to stream video from a high altitude balloon over wifi. The Ubiquiti Dish connects to the Ubiquiti node on the balloon.  I need to know the address of the Pi when I set up the stream, so I set up the Raspberry Pi to have a static ip (there is a page of instructions for this.)
