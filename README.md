# rosedust
## a pretty, desaturated pink theme to calm your heart

## based on the palette from my personal website, rio.pink

## contains the following themes:

### gtk 2/3

need to add gtk install instructions

### firefox

you can access the theme on the marketplace here:

https://addons.mozilla.org/en-US/firefox/addon/rosedust/

### dark reader

browser extensions available here:

https://darkreader.org/

github repo:

https://github.com/darkreader/darkreader

installation: 
- click the dark reader icon on toolbar
- select "Settings"
- select "Manage Settings"
- select "Import Settings"
- select the Dark-Reader-Settings.json from this repository

### tree style tab (TST)

firefox extension:

https://addons.mozilla.org/en-US/firefox/addon/tree-style-tab/

chrome extension:

https://chrome.google.com/webstore/detail/tree-style-tab/oicakdoenlelpjnkoljnaakdofplkgnd?hl=en

installation:

firefox:

- visit about:addons in the URL bar
- click three dots next to the extension name
- select "Preferences" and expand "Advanced"
- under "Extra style rules for contents provided by Tree Style Tab, either select "Load from File" and select tresstyletab.css from this repository or copy its contents into the text field

chrome:

TBD

### thunderbird

if you have already installed the gtk theme, you should be able to select the hamburger menu (three lines)->settings->general->Colors... and enable "Use system colors". A real thunderbird theme is in the works.


### joplin

download application:

https://joplinapp.org/

installation:

- install the Rich Markdown plugin here (instructions are in their README):
https://github.com/CalebJohn/joplin-rich-markdown
- move the userchrome.css and userstyle.css files to the config directory:
Linux/macOS: ~/.config/joplin/
Windows: C:\Users\%USERNAME%\.config\joplin\

- select "Tools"
- select "Options"
- select "Rich Markdown" 
- select "Add additional CSS classes for enhanced customization"
- return to "Options"
- select "Appearance"
- change "Theme" to "Dark"

### kitty

- install from here (instructions are in their README):
https://github.com/kovaidgoyal/kitty
- copy the contents of rosedust-kitty.txt into your kitty.conf file. You can open it within kitty with ctrl-shift-f2 or check its default location, ~/.config/kitty/kitty.conf
- make sure to remove or comment out any previous duplicate settings

### polybar

- install from here (instructions are in their README):
https://github.com/polybar/polybar
- copy the contents of rosedust-polybar.txt into yout config.ini file. It is usually found in ~/.config/polybar. If it isn't, you can copy a default config from /etc/polybar/config.ini
- make sure to remove or comment out any previous duplicate settings

### rofi

- installation instructions here:
https://github.com/davatorium/rofi/blob/next/INSTALL.md

- create a default config file if it does not exist
```
mkdir -p ~/.config/rofi
rofi -dump-config > ~/.config/rofi/config.rasi
```

- add this line to config.rasi:
```
@theme "rosedust"
```

- copy rosedust.rasi from this repository into your preferred theme directory. They will be accessed by rofi in this order:
```
    ${XDG_CONFIG_HOME}/rofi/themes/
    ${XDG_CONFIG_HOME}/rofi/
    ${XDG_DATA_HOME}/rofi/themes/
    ${INSTALL PREFIX}/share/rofi/themes/
```

### btop

- install from here:
https://github.com/aristocratos/btop
- from their docs:
```
Themes should be placed in "../share/btop/themes" relative to binary or "$HOME/.config/btop/themes"
```
- copy 'rosedust.theme' from this repo into one of those paths
- add `color_theme = "YOUR/CHOSEN/PATH"` to your btop.conf file, it should be in `$HOME/.config/btop`.

## TO-DO

### I need to define an official palette and tweak some of these themes to reflect it. No themes (except gtk) have been uploaded yet for this reason.
### I need to add a screenshot/rice of this theme in use
### I need to add gtk install instructions
### I need to add the color config I use in i3.conf
### I would like to theme the following applications, if I can figure out how:
- vs code
- signal desktop
- bitwarden desktop
- steam
(basically all the other apps that I use every day. some of those might be tricky, so if you would like to help, let me know.)

