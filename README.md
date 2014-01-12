dalvikcache-mover
=================

init.d script for android to move dex files outside /data/dalvik-cache

Put the script it in /system/etc/init.d, chmod it 655 then reboot.

The script moves just app/asec cache files, not system nor framework ones. The folders can be customized, just look at the first lines of file.

During each boot phase, the script will relocate the files, as long as there is free space, to the configured directory (/preload/dalvik-cache is the default one), after having deleted the unused ones.



Tested on Asylum OmniRom 4.4.2 on Samsung Galaxy Note N7000, with ART enabled.
