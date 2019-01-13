# i3blocks-config
This is my i3blocks configuration. It might require some extra packeages to be installed.

<h2> Installation: </h2>

<h4> &nbsp;&nbsp; 1. Install i3blocks: </h4>

Start of by installing [i3blocks](https://www.archlinux.org/packages/community/x86_64/i3blocks/).

<h4> &nbsp;&nbsp; 2. Modify i3 configuration file: </h4>

*~/.config/i3/config*:
```
bar {
  position top                  # Position should be 'bottom' or 'top'.
  status_command i3blocks       # Invoke i3blocks.
  
  # Possible other bar configurations go here...
  # ...
}
```
<h2> Modification: </h2>

It is easy to modify the bar. Take a look at [.config/i3blocks/config](https://github.com/miklhh/i3blocks-config/blob/master/.config/i3blocks/config) and see for yourself how easy it is to modify the bar. If something is not working, this should be the 
entypoint for your bug searching. I have not tested any this on any other computer, it will probably break
and I leave you to fix it for yourself. Heeh.
<br/> <br/>
If you want to modify the weather location data, take a look into [config/i3blocks/weather/weather.py](config/i3blocks/weather/weather.py).
This to is easy to modify, just change the YR.no XML link. Example YR link: [https://www.yr.no/place/Sweden/Stockholm/Stockholm/forecast.xml](https://www.yr.no/place/Sweden/Stockholm/Stockholm/forecast.xml). Simply go to the YR webpage you desire and add */forecast.xml* to the end of the URL (english YR version only) to get the appropriate link for the weather script.


<h3>Thumbnail:</h3>

![Thumbnail1](resources/i3blocks-thumbnail-1.png) 
<br/>
![Thumbnail2](resources/i3blocks-thumbnail-2.png)
***

<h2>Requiered software and packages.</h2>

* [I3BLOCKS](https://www.archlinux.org/packages/community/x86_64/i3blocks/): The actuall bar.
* [NOTO-FONTS-EMOJI](https://www.archlinux.org/packages/extra/any/noto-fonts-emoji/): Or other emojicon font.
* [DUNST](https://www.archlinux.org/packages/community/x86_64/dunst/): Or other notification daemon.
* [ACPI](https://www.archlinux.org/packages/community/x86_64/acpi/): For getting battery information.
* [CPU-STAT](https://github.com/vivaladav/cpu-stat): For getting CPU usage. This should be manually installed and the executable should be runable from '.config/i3blocks/cpu/cpu-stat'.
* [CURL](https://www.archlinux.org/packages/core/x86_64/curl/): Probably already installed.
* [PYTHON 3](https://www.archlinux.org/packages/extra/x86_64/python/): Probably already installed.
* [PYTHON-REQUESTS](https://www.archlinux.org/packages/extra/any/python-requests/): For getting weather. Could be installed with pip.
