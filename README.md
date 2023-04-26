# i3wm-config

Using Bumblebee https://github.com/tobi-wan-kenobi/bumblebee-status

Mix of Iceberg-Rainbow and Catpuccin

![example](https://user-images.githubusercontent.com/77973084/233843270-b7029786-cdd4-48a8-8d18-418bc70fb7ab.png)

## To get started:

Assuming you have compeleted the base i3wm installation process. Do the following to apply this configuration:

### Install Bumblebee-status:

```
git clone https://aur.archlinux.org/bumblebee-status.git

cd bumblebee-status

makepkg -sicr
```

Great now clone this repository by:

```
git clone https://github.com/ElmeriVincent/i3wm-config.git
```
Now open it (i3wm-config folder) and copy everything inside it and replace everything inside the `.config/i3` the filepath to that should be something like this: `/home/<username>/.config/i3/` once you have done that now press `$mod+Shift+c reload`to refresh your window manager with these changes.

Good job!! Now you should see the beautifully colored top bar and other stuff like purple border on your opened windows. You may wonder why the wallpaper has not changed.. well I haven't added to my configuration due me often changing my wallpaper but you can put it to yours if you want.

### Additional
I also like to use gnome-screenshots so my PrtSc binding uses it. To install it do:

`sudo pacman -S gnome-screenshot`

if you do not want to install it that's ok just disable or replace the binding with what you want. I prefer to use mostly the default keybindings because it's just simpler. Remember that you can customize this how you want. 

#### My prefered shell setup

Fish shell with starship:
`sudo pacman -S fish`
after that `chsh` put your password and `/bin/fish` then hit **enter** and
now do `curl -sS https://starship.rs/install.sh | sh` to install https://starship.rs/ then **logout** once you are logged back in do `nano ~/.config/fish/config.fish` and paste this in 

```
if status is-interactive
    # Commands to run in interactive sessions can go here
        set fish_greeting
        starship init fish | source
end
```

Great! Just exit the terminal and relaunch it to see your fish shell with starship enabled.

### Need Help
Just do a new issue with good explanation of your problem and I or someone else will help you out.
