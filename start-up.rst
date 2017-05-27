=====================
How to Start the Boat
=====================

Connect power.

Check lights are flashing on the Pi and Capt Morgan. 

Wait for WiFi hotspot to start up, then connect to it.

shh into the Pi.

Run tmux

Check boatd status by running::

    sudo systemctl status boatd
    
Check there is no failure on boatd status (this should be obvious).

To see the output from boatd api you can run::

    curl localhost:2222/boat

At this point you can run a behaviour by running::

    cd dewi/dewi-behaviour

    ./any-behaviour

Where any-behaviour should be replaced with the name of the behaviour you
want to run.

Logs will appear. 

If you need to end the current behaviour, use ctrl+c to end behaviour (boatd will continue to run)

You can then run another behaviour.

Mavlink
=======


Waypoint Loading
================
Before starting a behaviour, you can edit the waypoints. To do this, edit the boatd config file ``/etc/boatd-config.yaml`` to include the path name of the waypoint file ( ``waypoint_file: '/some/path'`` ).

The waypoint file should hold a list of latitudes and longs. These should have a space separating the lat from the long, with each new waypoint on a new line, e.g.::

    53.23456 -4.34245
    53.54151 -4.24565

The waypoint at the top of the list will be the first waypoint used by boatd. 






