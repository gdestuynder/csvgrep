csvgrep
=======

* Tiny handy script to grep csv files by field, no matter where the field is located
* Original made for ArcSight csv exports
* You probably want to run this as ./csvgrep <file> <columns> | column -t
* Since column doesn't implement proper signaling I didn't include it by default, since | head'ing the script would otherwise take forever on big files

If that's possible to do with other tools such as ack or other context sensitive grep tools, let me know. Meanwhile, this works ;-)

I currently found 3 implementations (perl, and 2 python), but they're extremely slow (4 to 10 times slower) than the awk wrapper
