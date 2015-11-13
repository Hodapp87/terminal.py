# terminal.py

This is a fork of <https://git.jim.sh/jim/terminal.git> from Jim Paris
with some changes I had made.  Hackaday also had a nice write-up on
this: [Python script lets you monitor multiple serial devices at once]
(http://hackaday.com/2012/11/16/python-script-lets-you-monitor-multiple-serial-devices-at-once/)

These changes are here because I was unable to get a hold of him via
email to accept a patch I'd written.  I found his tool very useful for
some of my work: I was trying to debug some serial communications
between two devices, and had no way to clearly show the transactions
between them.

I fixed some Python 3.x bugs, added functionality for logging to a
file, and I started trying to add functionality for timestamps at each
line - but this is still not working right.
