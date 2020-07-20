# Umístění skriptů

* /home/pi/custom_player.sh
* /home/pi/custom_player.py

# Automatický start po bootu

Nakopírovat z adresáře `/etc/systemd/system/`

`sudo cp custom_player.service /etc/systemd/system/custom_player.service`

Následně z konzole spustit, stejný příkaz, pouze s direktivou `stop` to zase vypne.

`sudo systemctl start custom_player.service`

A pak ještě aby to nabíhalo po každém bootu, stejný příkaz, pouze s direktivou `disable` to zase vypne.

`sudo systemctl enable custom_player.service`

