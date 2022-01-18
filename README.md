# raspberryPrinter
Sammlung und Dokumentation von allem, was es zum Drucken auf und mit dem RaspberryPi braucht.

## Drucken mit CUPS
### Installation
```bash
sudo apt update
sudo apt install cups
sudo cupsctl --remote-admin
sudo cupsctl --share-printers
sudo cupsctl --remote-any
sudo usermod -aG lpadmin pi
sudo systemctl restart cups
sudo apt install printer-driver-gutenprint
```
### Konfiguration
https://_hostname_:631
### Quelle
https://www.elektronik-kompendium.de/sites/raspberry-pi/2007081.htm

## Mail 2 Print
Mit einem Python Tool werden neue Mails abgerufen und der Anhang anschließend gedruckt.
### Installation
```bash
sudo apt update
sudo apt install python3 python3-pip
sudo pip3 install imbox
sudo pip3 install jinja2
```
