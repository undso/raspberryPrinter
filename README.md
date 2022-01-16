# raspberryPrinter
Sammlung und Dokumentation von allem, was es zum Drucken auf und mit dem RaspberryPi braucht.

## Drucken mit CUPS
### Installation
```bash
sudo apt install cups
sudo cupsctl --remote-admin
sudo cupsctl --share-printers
sudo cupsctl --remote-any
sudo usermod -aG lpadmin pi
sudo systemctl restart cups
sudo apt install printer-driver-gutenprint
```
### Konfiguration
https://<<hostname>>:631
