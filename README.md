dalvikcache-mover
=================

init.d script to move dex files outside /data/dalvik-cache

After first boot (with dalvik cache already generated), put the script it in /system/etc/init.d, chmod it 655 then reboot.

The script will relocate the files, as long as there is free space, in /preload/dalvik-cache.

The script moves just app/asec cache files, not system nor framework ones. The folders can be customized, just look at the first lines of the script.

Tested on Asylum OmniRom on Samsung Galaxy Note N7000.
