To install Kiosk
sudo apt-get install --no-install-recommends xserver-xorg
sudo apt-get install --no-install-recommends xinit
sudo apt-get install --no-install-recommends x11-xserver-utils
sudo apt-get install chromium-browser
sudo apt-get install matchbox-window-manager xautomation unclutter


sudo cp kiosk.service /lib/systemd/system/kiosk.service
sudo systemctl enable kiosk.service
sudo systemctl start kiosk.service
