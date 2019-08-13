# linux-cheat-sheet
Various commands for productivity and inspecting your machine

## Hardware

|---|---|
|dmesg|Detected hardware and boot messages|
|cat /proc/cpuinfo|CPU model|
|cat /proc/meminfo|Hardware memory|
|cat /proc/interrupts|Lists the number of interrupts per CPU per I/O device|
|lshw|Displays information on hardware configuration of the system|
|lsblk|Displays block device related information|
|free -m|Used and free memory (-m for MB)|
|ispci -tv|Show PCI devices|
|lsusb -tv|Show USB devices|
|dmidecode|Show hardware info from the BIOS|
|hdparm -i /dev/sda|Show info about disk sda|
|hdparm -tT /dev/sda|Do a read speed test on disk sda|
|badblocks -s /dev/sda|Test for unreadable blocks on disk sda|
|powertop|See battery usage|
|iotip|Disk access information|
|smartctl {disk}|Show what disk is doing|
|tlp-stat|Battery information including degredation|

## Network

|---|---|
|ip addr show|Display all network interfaces and ip addresses|
|ip address add 192.168.0.1 dev eth0|Set ip address|
|ethtool eth0|Show ethernet status|
|mii-tool eth0|Show ethernet status|
|dig {domain}|Get DNS information for domain
|dig -x {host}|Reverse lookup host|
|netstat -tupl|List all active listening ports
