# i3wm-config

Using Bumblebee https://github.com/tobi-wan-kenobi/bumblebee-status

Mix of Iceberg-Raibow and Catpuccin

![example](https://user-images.githubusercontent.com/77973084/233843270-b7029786-cdd4-48a8-8d18-418bc70fb7ab.png)

## To get started:

`cd .config/i3`

## Install Bumblebee-status:

`git clone https://aur.archlinux.org/bumblebee-status.git`

`cd bumblebee-status`

`makepkg -sicr`

### Additional
I also like to use gnome-screenshots so my PrtSc binding uses it
`sudo pacman -S gnome-screenshot`

Fish shell with starship:
`sudo pacman -S fish`
then logout.. after that `chsh` put your password and `/bin/fish` then hit **enter**
Now do `curl -sS https://starship.rs/install.sh | sh` then `nano ~/.config/fish/config.fish` and paste this in 

```
if status is-interactive
    # Commands to run in interactive sessions can go here
        set fish_greeting
        starship init fish | source
end
```

Great! Just exit the terminal and relaunch to see your fish shell with starship enabled
