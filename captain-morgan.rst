=================
Captain H. Morgan
=================

Captain Morgan is an attempt to integrate the electronics of a 
robotic sailing boat into a single, easily testable PCB.
As of the time of writing, the GPS and power regulation 
for the autonomous control system is implemented and working
well. In future revisions it will also contain a real-time 
MCU to handle timing critical systems on the boat, various 
communication systems including Wifi and Xbee radios, input
protection on all external electrical connections, and 
battey monitoring circuitry.

Current Versions
----------------

There are currently two versions of the Captain Morgan in circulation,
the first is a very rough prototype, a heavily modified version was taken 
to Sailbot 2016 where is worked fairly well, however where possible
these should be replaced with later versions and removed from service.

The other version is v1.2, this is pretty much complete and only requires
a minor bodge wire to enable using an active antenna, this is the version 
that went to WRSC 2016.

The final version currently in existance is the v1.2.2, this is a tweaked 
v1.2 which fixes the Vant pin not being connected to power an antenna.
At the time of writing this version is being fabbed and should be ready 
in early January. This version is meant to be a fully functional reserve
to allow development of new features while not compromising the functionality
of the boats for competitions.

Bill Of Materials
-----------------

Below is the Bill of Materials for the v1.2.2 Captain H. Morgan PCB.

+----------------------+----------------+-------+---------------+-----------+--------------------+----------------+
| Part                 | Refrence       | Count |  RS part no.  |  RS cost  |  Farnell part no.  |  Farnell cost  |
+======================+================+=======+===============+===========+====================+================+
| P header 2x20        | J1             | 1     | 254-6182      | £4.83     | 1569232            | £3.65          |
+----------------------+----------------+-------+---------------+-----------+--------------------+----------------+
| Pcb mount mmcx       | J2             | 1     | 680-7440      | £1.60     | 1056319            | £1.93          |
+----------------------+----------------+-------+---------------+-----------+--------------------+----------------+ 
| 2K2 1206 resistror   | R3/R4/R5/R2    | 4     | 223-2300P     | £0.01     | 9336168            | £0.04          |
+----------------------+----------------+-------+---------------+-----------+--------------------+----------------+ 
| 10k 1206 RESISTOR    | R1             | 1     | 223-2394      | £0.02     | 9335765            | £0.04          |
+----------------------+----------------+-------+---------------+-----------+--------------------+----------------+
| Polyfuse             | F1             | 1     | 647-8364P     | £0.19     | 1817308            | £0.40          |
+----------------------+----------------+-------+---------------+-----------+--------------------+----------------+
| Schottky Diode       | D1-D2          | 2     | 485-612       | £0.13     | 8737819            | £0.18          |
+----------------------+----------------+-------+---------------+-----------+--------------------+----------------+
| Green Led 1204       | LED5/LED1/LED3 | 3     | 906-3508      | £0.09     | 206226             | £0.31          |
+----------------------+----------------+-------+---------------+-----------+--------------------+----------------+
| Red Led 1204         | LED2/LED4/LED6 | 3     | 906-3527      | £0.09     | 2062231            | £0.57          |
+----------------------+----------------+-------+---------------+-----------+--------------------+----------------+
| Maestro A2200-A      | U1             | 1     | Discontinued  | N/A       | 2281694            | £13.57         |
+----------------------+----------------+-------+---------------+-----------+--------------------+----------------+

