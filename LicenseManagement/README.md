# License Management
This project aims to provide a licensing solution which includes:
* Single / Volume license 
* Offline / Online Activation
* Hardware-based UID 
* Selectable Features
* RSA signing method to protect license key
* Automatic licensing server

# Single/Volume license
Each time your app runs on a computer, it generates an uniqe UID based on Hardware ID which includes ProcessorID, HardDisk Serial Number, MotherboardID and a secret key.

Single license will tight to only one PC. Voluime license will count the number of activated PC. Both of two method provides Time Limitation too. So that you can use license as subcription.

# Offline/Online Activation
If the target machine has the Internet connection, license can be acquired automatically by sending a request to Activation Server. The activation process is fast and simple based on REST API and JSON. Key is sent directly to your app if custommer already purchased.

If there is no Internet, customer can activate app by offline \*.lic file which is sent via emails when they purchase a license.

# Selectable Features
License file includes direction to enable/disable a feature of application.

# RSA Signature license
Using RSA algorithm, the license is encrypted and signed to make sure that the license is not tamped by any outside incident.

# Automatic licensing server
Serving online activation, there is a server that responses to activating requests from applications on the air. The license is automatically generated after a purchase is made and then the license will be sent to customer directly.

# Video demo
[LicenseActivationOffline](./LicenseActivationOffline.mp4)

[LicenseActivationOnline](./LicenseActivationOnline.mp4)

![screenshot](screenshot.png)