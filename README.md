# Evil Twin WiFi Awareness using ESP8266

This repository contains a cybersecurity awareness demonstration explaining how Evil Twin attacks work and how attackers can misuse rogue access points. Educational + defensive research only.

## About the Project
This project explains the concept of Evil Twin attack and creates awareness for beginners in cybersecurity about Wi-Fi threats.

## Hardware / Modules Used
- ESP8266
- WiFi compatible module
- Laptop / Target test environment (Lab only)

## Disclaimer
This project is strictly for **Educational & Research purposes only**.  
Never perform unauthorized penetration testing on real networks.

## Install using Arduino IDE
1. Install Arduino IDE
2. In Arduino go to File -> Preferences add this URL to Additional Boards Manager URLs -> https://raw.githubusercontent.com/SpacehuhnTech/arduino/main/package_spacehuhn_index.json
3. In Arduino go to Tools -> Board -> Boards Manager search for and install the deauther package
4. Download and open [eviltwinattack.ino](https://github.com/cyberwolf6938/evil-twin-attack/blob/main/eviltwinattack.ino) with Arduino IDE.
5. Select an ESP8266 Deauther board in Arduino under tools -> board
6. Connect your device and select the serial port in Arduino under tools -> port
7. Click Upload button

## How to use:
- Connect to the AP named CyberWolf with password 33669999 from your phone/PC.
- Select the target AP you want to attack (list of available APs refreshes every 30secs - page reload is required).
- Click the Start Deauthing button to start kicking devices off the selected network.
- Click the Start Evil-Twin button and optionally reconnect to the newly created AP named same as your target (will be open).
- You can stop any of the attacks by visiting 192.168.4.1/admin while conected to Evil-Twin AP or by resetting the ESP8266.
- Once a correct password is found, AP will be restarted with default ssid CyberWolf / 33669999 and at the bottom of a table you should be able to see something like Successfully got password for - TARGET_SSID - PASSWORD
- If you power down / hard reset the gathered info will be lost

## Important Point:
You can change username(CyberWolf) and password(33669999) in code with arduino ide and also ip address(192.168.4.1) with your choice.

## Author
CyberWolf6938

## Follow Me
If you want to see evil twin attack demo go to my medium account [Evil Twin Wi-Fi Attacks: How to Perform, What the Risks Are, and How to Protect Yourself (Non-Technical, 2025)](https://medium.com/@falolopopololopopo/evil-twin-wi-fi-attacks-how-to-spot-what-the-risks-are-and-how-to-protect-yourself-3a3db86e4beb)  

## License
[LICENSE](LICENSE)
