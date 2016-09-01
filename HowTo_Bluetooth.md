INSTALATION OF A BLUETOOTH DEVICE

$ sudo apt-get update
$ sudo apt-get upgrade
$ sudo apt-get autoremove

$ sudo apt-get install bluetooth bluez-utils blueman

$ cd /etc/bluetooth
$ sudo nando main.conf
	DisablePlugin = pnat

$ sudo hciconfig hci0 up
$ sudo hciconfig hci0 piscan \\ make it discoverable

$ sdptool add sp
$ sudo rfcomm listen hci0&

$ cat /dev/rfcomm0

$ sudo bluez-simple-agent


--------------------------------------
MAINTENANCE

	$sudo /etc/init.d/bluetooth restart
