Features and How to of the AndroidianiOpenRecovery

HowTo & explanation of OpenRecovery Features

# Introduction #

This OpenRecovery is based on the latest 1.42 build from Skrilax\_CZ, all credits for the creation of original openrecovery goes to him!
Our OpenRecovery is only a Mod, specifically for our milestones, and add a lot of features, for modding both eclair and froyo (Motofrezy an Cyanogen mod).
The open recovery, has a clear menu, easy to use, for Eclair modding and one for Froyo modding.


# Details #

So starting from **Eclair Modding Menu**:
Entering this menu you'll see:


_Install Recovery at Boot_:
Will install a boot script that will let you to Boot your recovery directly in OpenRecovery instead of passing per Update.zip!!

_install memhack_:
Installs the hack to move Dalvik cache from /data to /cache, freeing a lot of space for apps!!

_install Conservative governor_:
Installs the modules and scripts to have the conservative governor from boot; It's a governor that have the lowest power consumption at all, it's a little slower to raise frequencies in comparison with the Interactive or Ondemand, but have the lowest power consumption

_install Interactive Governor_:
Installs the Interactive governor, a little faster of Conservative, but more power hungry (still less than ondemand)

NB: for Governors, credits goes to nadlabak http://android.doshaska.net/ here you see all the article for governors

_install Jitv7_:
This will install the latest froyo's jit, directly from samdroid, it's more stable and reliable than the obsolete one from GOTs OR

**NEW**_install flac support_
This will install libraries and framework.jar, so the rom will support also the playback of .flac files!

_install ADBDBoot_:
This will install a little hack that starts at boot, and will allow adb to start directly as Root! (without to have root installed BTW)very nice utility

**_install RecoveryBoot_**:
This is the newest news from 1.42 openrecovery!
You can boot into recovery without pass for the original one! this will substitute the original one at the boot, and will boot directly in OpenRecovery! A very neat feature!

_nb_: if you wipe cache, you have to boot another time in recovery as the command to boot directly in recovery is in cache!

Then there will be some modding menus:

_overclock menu_:
A lot of choice for you!
There is for all flavours; all overclocks are undervolted from the first to the 800mhz one, 900 mhz and 1000 mhz are at original vsel, and for 1,1ghz we have a little overvolt; even with original vsel (or overvolt) all other steps are sightly UNdervolted!
Battery consumption is less even at 1,1ghz!
550mhz step is only a undervolt, 550mhz with 38vsel (vs original 56)

steps are:
550mhz (undervolt only)

650mhz

750mhz (x2 one from 125mhza and one starting at 250)

800mhz (x2)

900mhz(x2)

1ghz (x2)

1,1ghz (x2)

**NEW**
_Scripts menu_:
This is a menu where you can find the most important script utility for your milestone!
All of them will be installe din /system/xbin and can be used both from adb or a terminal emulator.
thw choice is:
To install _Nano editor_: very neat utility (recommended using adb as is not confortable on small milestone screen), a text editor commandline.

Install _Camerasound on/off_: this little script will shut off or on you camera sounds (type **soundon or soundoff** in terminal/adb)

Install _Mount/unmount system scripts_: will install 2 little script to mount system in Read/write (**mountrw**) or Read/Only (**mountro**)

Install _switch bootanimation script_: little script (**switchba**) to swap your bootanimation with one on you sdcard (must be in the root, and named "bootanimation.zip")

Install _Movecache script_: with this script (**movecache**) you can move the cache from /cache to sdcard (freeing a lot of space!)

Install _Show/Hide ads_: this will install 2 script (**showads** and **blockads**) that will enable/disable the ads in the system (IN THE APPLICATIONS FOR EXAMPLE)

Install _Bash_: alternative to Busybox, or you can install both altogether just tpe **bash** in adb/terminal

Install _Zipalign script_: this will install a script (**zipalign\_apks**) that will zipalign all system apks (see below for info on zipaligning)

_BusyBox menu_:
Installs busybox in /data /sbin and /xbin

_menu App2sd_:
To install app2sd, split memory cards, and use app2sd both in original and symplink edition!

_Menu Install theme_:
To install the theme or restore the old one!

After those, here is the **Froyo Modding menu**:

_App2sd_ menu dedicated to app2sd for froyo images;

We have
_install conservative governor_
_install interactive governor_

_ALL THE OVERCLOCKS ARE THE SAME AS IN ECLAIR SO READ ABOVE FOR THEM_

_Install Memhack_:

_Auto off Buttons Led_:

It will start a daemon that will automatically shut off buttons led after a while, sparing some juicy battery life!!!
Credits to Azhad for this! -> Recommended to MotoFrenzy

_Scripts menu_:

it's a link to the Eclair one is the same, so read above!

_Install Recovery at Boot_:
Will install a boot script that will let you to Boot your recovery directly in OpenRecovery instead of passing per Update.zip!!!



NEW **ZIPALIGN MENU**
This menu is splitted in 3 parts:

Only data partition-> zipalign only on /data/app and /data/app-private

Only system partition-> zipalign only on /system/app and /system/framework

Both of them

zipaligning is a procedure, where the apk is very optimized. The purpose is to ensure that all uncompressed data starts with a particular alignment relative to the start of the file.Specifically, it causes all uncompressed data within the .apk, such as images or raw files, to be aligned on 4-byte boundaries. This allows all portions to be accessed directly with mmap() even if they contain binary data with alignment restrictions. The benefit is a reduction in the amount of RAM consumed when running the application.

**THIS IS COMPATIBLE WITH BOTH ECLAIR AND FROYO**
(on Cyanogen is useless as is already zipaligned!!

NEW **UNIVERSAL CAMCORDER RESOLUTION MOD**
This menu is present in all Eclair/Froyo menu, this hack will let you to choose wether to record in:

720x400--> Fit the screen resolution

720x480--> Default standard resolution

720x576--> Standard PAL resolution (nice if you want to see it on a TV Pal, while 720/480 fits better for a new 16:9 TV)

Those hacks includes also the 30fps hack, tweakings to the audio and video quality and bitrate!

**THIS IS COMPATIBLE WITH BOTH ECLAIR AND FROYO**

NEW **UNIVERSAL PIXEL DENSITY MOD**
This menu allows to simply apply the Res-hack that consist in "tricking" android and letting him think that we have a much higer res screen...so LOWING the number we INCERASE the resolution!
200 is the best for milestone so far, 190 is the lowes accettable and 240 is the standard...
this mod can also be used to INCERASE the button's size! setting it HIGHER than 240 will make buttons and all the system "bigger"...perfect to who do not see well, or simply prefer big buttons! ;D

**THIS IS COMPATIBLE WITH BOTH ECLAIR AND FROYO**

NEW **MENU APP**
This menu is very very brilliant, it allows to  copy and delete application to and from /system/apps, /data/apps (with ext2 apps2sd support), and an app folder in the recovery. With that you can:Delete system and user apps, with or without data, Copy apps from internal memory to system, Copy apps to Recovery,
Copy apps from Recovery to Internal or System memory and now also UPGRADE apps in recovery!
This tool is very very useful as a Backupping tool, as a Modding tool (to mod system apps) and a beautiful app-manager tool (to bring and move apps from data to system or vice-versa)

**THIS IS COMPATIBLE WITH BOTH ECLAIR AND FROYO**

NEW **UTILITY MENU**

In this menu are grouped all the small (and not so small xD) utility for BOTH ECLAIR AND FROYO:

_BLOCK ADDS_: blocks adds in the whole system, both in browser and apps!

_SCANDISK SD_: does the scandisc on your sd, very handy in some situations!

_SCANDISK EXT2_:as before, only for app2sd users obviously!

_ECLAIR/FROYO KERNEL TUNING SCRIPT_: as the name says, this is a VERY beautiful script that I tweaked a bit from original (from kholk & xslntx on XDA) that encache the performance and the soothness of our mileston A LOT...it also improves 3d managment and all the experience is much more smoother and faster!

_FIX PERMISSION APKS TO PREVENT FORCE CLOSES_:this is a very handy tool! this will re-set all permission in all apks in the entire system (system, data and for app2sd and froyo even sd) to prevent sudden FC in apps!

_SHOW FREE SPACE_:will display your free sd card and flash memory space :D

**THIS IS COMPATIBLE WITH BOTH ECLAIR AND FROYO**

**TO THE MAIN MENU:**

We added the option to **_wipe ext2 partition_** For who have app2sd and want to format his ext2 partition!

**HOW TO THEME:**

To install a theme, before using the recovery menu, we have to load a theme:
Under the Directory /sdcard/OpenRecovery, there is a directory theme;
IF you want to install a eclair theme; go to the "Eclair" folder and put the files in their respective directories,
IF you want a Froyo theme, go to Froyo and put files in their respective directories.
Then in the recovery you will find the right Theme menu under:
Eclair -> Theme
Froyo -> MotoFrenzy -> Theme
Froyo -> CyanogenMod -> Theme

**NEW RECOVERY THEMES**
To install a recovery theme, you simply have to go in -stettings-theme and choose what to install :-)
We for now have 4 themes for you:

_Original THEME_: the original AndroidianiOpenRecovery theme, white on black fonts(simple)

_AZHAD Theme_:a very nice theme, based on Black with RED fonts and Green LED status

_89Luca89 THEME_:This one is based on Original OpenRecovery theme, a DroidEYE background with blue fonts GREEN LED status.

_FANTASY THEME by 89Luca89_:This one is the most visual of them, features a beautiful fantasy background with red fonts and VIOLET status LED

Theming the recovery is very nice because gives you the possibility to have a custom milestone EVEN in the recovery :-D
In fact There will be much more themes in nex release!


By 89luca89