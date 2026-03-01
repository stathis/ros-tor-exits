# RouterOS TOR Exits
Importable TOR exit node list for MikroTik RouterOS in the form of an .rsc file.

## Using
To use, create a script like the one below on your system and a scheduled task for the aforementionted script.

```
/tool fetch address=raw.githubusercontent.com host=raw.githubusercontent.com mode=https src-path=stathis/ros-tor-exits/master/tor-exits.rsc
/ip firewall address-list remove [/ip firewall address-list find list=__TOR_EXIT]
/import tor-exits.rsc
```

## Other info
This repo should be a updated once a day, but then again, it might not be.

## License
MIT license.
