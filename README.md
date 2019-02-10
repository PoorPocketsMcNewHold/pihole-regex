## Regex Filters for Pi-hole
This is a custom `regex.list` file for use with Pi-hole v4+ (FTLDNS).

All commands will need to be entered via Terminal (PuTTY or your SSH client of choice) after logging in.

HOWEVER: This one add to this fork, the ones from https://github.com/IcedComputer/Personal-Pi-Hole-configs so... Feel free to only just the original one list from mmotti if you don't want a regex list overload.
### [OPTIONAL] Back up your existing regex list
```
sudo cp /etc/pihole/regex.list /etc/pihole/regex.list.bak
```

### Installation Instructions
```
curl -sSl https://raw.githubusercontent.com/PoorPocketsMcNewHold/pihole-regex/master/install.sh | bash
```

### Removal Instructions
```
curl -sSl https://raw.githubusercontent.com/PoorPocketsMcNewHold/pihole-regex/master/uninstall.sh | bash
```

### Testing the regex filter
See if you can access https://ad.pi-hole.net/

Then check the query log in the Pi-hole admin console for your blocked domain. It should show as **Pi-holed (wildcard)**.

![alt test](https://image.ibb.co/j5kWTz/Blocked.png)
