# Rofi Theme Menu
This is a Rofi Theme Menu selector to change i3, polybar, and rofi config files all at once. 
![Rofi Image](https://raw.githubusercontent.com/sanicsquirtle420/rofi-theme-menu/main/pictures/rofi-theme.png)

## Dependencies
If you would like to use it how the stock [rofi-theme-menu.rasi](https://github.com/sanicsquirtle420/rofi-theme-menu/blob/main/rofi-theme-menu.rasi) file is set up.

`i3-gaps rofi polybar dunst nitrogen git` any Nerd Font (Arimo Nerd Font is used in the stock .rasi file)

## "Setup"
It's in quotes because it doesn't really feel like one lol.
```
cd ~/Downloads
git clone https://github.com/sanicsquirtle420/rofi-theme-menu
cp -r ~/Downloads/rofi-theme-menu/rofi-theme-menu.rasi ~/.config/rofi/
```

## Usage
Run or add to i3 config: `rofi -show p -modi p:~/.config/rofi/rofi-theme-menu.rasi`

Common Flags for Usage:
`-font "FONT XX"`
`-theme "THEME"`
`-width XX`
`-lines XX`
XX is a variable for any number and FONT/THEME are also variables for any Font name or Theme name.

## Configuring
In the stock file, all of my themed config files are located in `$HOME/Documents/i3-themes/THEME-NAME` and are then copied to `$HOME/.config/`

If you wish to change that to better suit your needs, scroll until you find `function change_theme ()` and start editing the code as you wish. 

### Flag Usage
Command Used:
![paper theme image](https://raw.githubusercontent.com/sanicsquirtle420/rofi-theme-menu/main/pictures/rofi-theme-paper.png)
```
rofi -show p -modi p:~/.config/rofi/rofi-theme-menu.rasi \
-theme Paper   \
-font "Arimo Nerd Font 16"
```
