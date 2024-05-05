Ubuntu or Fedora - good choices.

Ubuntu:
1. Install Flatpak and Flathub
2. Enable additional Repos in Software & Updates
3. gnome-tweaks, gnome-extensions-app, dconf-editor, synaptic. Center new windows etc.
4. flatpak flatseal, extensionmanager
5. VSCode from Microsoft, install .deb and it adds the ppa and autoupdates. Additionally Reaper. Both also are in Flathub.

Fedora:
1. Flatpak and Flathub already installed.
2. gnome-tweaks, gnome-extensions-app
3. flatpak flatseal, extensionmanager, seahorse (keyring gnome app)
4. Install extensions: Desktop Icons, Dash to Dock, AppIndicator and KStatusNotifierItem. Manually can be copied to user folder somewhere
and the name has to match the metadata.json file's UUID. home/username/.local/share/gnome-shell/extensions/. Show hidden files.
5. Install snapd and snap-store to get RiseupVPN
6. Install RPMFusion repo from the Quick Docs section of Fedora documentation or rpmfusion website but replace mirrors with download1
if the polish server is offline as it often is. Enable AppStream metadata.
7. Install multimedia codecs, AMD drivers and firmware from rpmfusion website.
8. Install VSCode using Microsoft's website but don't download the rpm package, instead use the script and add a repo to have it in dnf.
9. Set the dark theme and in gnome-tweaks set the adwaita legacy dark theme. Center new windows etc.

Both are good to go. Fedora has a lifecycle of about 13 months and Ubuntu of about 9 months. Ubuntu LTS 5 years.

So many apps to download, stability may vary of course, it's linux after all...

gnome-terminal shortcut
gnome-system-monitor shortcut
nautilus or home folder shortcut

sudo Nautilus if necessary

sudo nano if necessary

copr repos might be worth looking into but often don't work properly because they are outdated too soon...
sudo dnf copr enable kwizart/fedy
sudo dnf install fedy -y
