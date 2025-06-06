# arch-hyprland-2
the hyprland on archlinux


## Load Basics - Sound

sudo pacman -S pipewire pipewire-alsa pipewire-jack pipewire-pulse wireplumber gstreamer gst-libav \ 
gst-plugins-good gst-plugins-bad gst-plugins-ugly ffmpeg

## Install Yay

sudo pacman -S git

git clone https://aur.archlinux.org/yay.git 
cd yay 
makepkg -si

rm -rf yay

## Load Hyprland

sudo pacman -S hyprland hyprlock hypridle hyprcursor hyprpaper hyprpicker waybar kitty rofi-wayland \
thumar dolphin dolphin-plugin ark kio-admin polkit-kde-agent qt5-wayland qt6-wayland xdg-desktop-portal-hyprland \
xdg-desktop-portal-gtk dunst cliphist mpv pavucontrol xdg-user-dirs-gtk

sudo pacman -S ttf-font-awesome ttf-jetbrains-mono-nerd ttf-opensans noto-fonts ttf-droid ttf-roboto

## Hablilita

systemctl --user enable pipewire pipewire-pulse wireplumbe

