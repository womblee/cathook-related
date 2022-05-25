# Installing cathook (Manjaro)

1. Install cathook via the appimage: https://nullworks.gitlab.io/cathook/cathook-gui/cathook-gui.tar.gz
2. (For this you need TF2 installed)
   - "git clone --recursive https://github.com/nullworks/catbot-database;cd catbot-database;sudo cp -R nav\ meshes/* ~/.steam/steam/steamapps/common/Team\ Fortress\ 2/tf/maps;sudo chmod 755 -R ~/.steam/steam/steamapps/common/Team\ Fortress\ 2/tf/maps;cd ..;sudo rm -r catbot-database"
3. Install dependencies:
   - "sudo pacman -Syu nodejs npm firejail net-tools xorg-xhost"
4. Clone setup:
   - "git clone https://github.com/nullworks/catbot-setup"
   - After cloning, run the ./install-catbots script.
5. Go to "/opt/cathook/data" and delete the configs folder, after deleting, create a folder with the same name.
6. Type this into the terminal to avoid config saving issues:
   - "sudo chown -R $USER /opt/cathook"
   - "sudo chmod 755 /opt/cathook"
7. Create accounts.txt in catbot-setup and paste via the following format - username:password
8. Use ./start and ./stop to start and stop the bots.
