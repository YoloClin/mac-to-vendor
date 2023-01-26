# mac-to-vendor

Given a mac address, returns vendor information as per nmap-mac-prefixes.
Should be resilient / handle whacky mac formats, etc.

Written out of frustration, instead of reading stackoverflow / google to figure 
out macs, now in a shell I can just type `mac[tab]` to suggest what I want ;)

Depends on nmap.

## Usage:

```bash
$ mac-to-vendor f4:92:bf:ab:cd:ef
Ubiquiti Networks
$ echo 'f4:92:bf:ab:cd:ef' | mac-to-vendor
Ubiquiti Networks
$ mac-to-vendor F4:92:BF:ab:cd:ef # Case Insensitive
Ubiquiti Networks
```

