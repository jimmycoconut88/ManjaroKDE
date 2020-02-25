# ManjaroKDE
Repository for my personal setting like dotfile and reminders XP
#PLEAZ READ THIS IN RAW UwU
initializing:
#grabbing update
sudo pacman -Syuu
#Nvidia grabbing
sudo mhwd -a pci nonfree 0300
sudo pacman -S networkmanager wpa_supplicant
systemtcl enable NetworkManager wpa_supplicant
systemtcl start NetworkManager wpa_supplicant
sudo pacman -S neofetch xwininfo (#or xdotool for neofetch) cmatrix ranger sxiv calcurse cmus wget mplayer mpv deadbeef mpd ncmpcpp mpc
mkdir ~/.config/mpd
nano  ~/.config/mpd/mpd.conf 
####### MPD CONFIG #######
# Required files
db_file            "~/.config/mpd/database"
log_file           "~/.config/mpd/log"
# Optional
music_directory    "~/Music"
playlist_directory "~/.config/mpd/playlists"
pid_file           "~/.config/mpd/pid"
state_file         "~/.config/mpd/state"
sticker_file       "~/.config/mpd/sticker.sql"
audio_output {  
      type  "alsa"  
      name  "mpd alsamixer-output"
      mixer_type "software"
}
audio_output {  
type               "fifo"  
name               "toggle_visualizer"
path               "/tmp/mpd.fifo"
format             "44100:16:2"
}
####### END MPD CONFIG #######
mkdir .config/mpd/playlists




yay -S nerd-fonts
