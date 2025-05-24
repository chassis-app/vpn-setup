# vpn-setup

## 1. Check your IP address
Start by checking your IP address at https://www.myip.com/, if you are using Regus WIFI, you should see the host name display regusnet.com

![image](https://github.com/user-attachments/assets/fb007113-c128-4c43-938a-ed5dfd5ba4ba)

## 2. Download the proxy tool (Shadowsocks)
https://github.com/shadowsocks/shadowsocks-windows/releases <--- for Windows

https://github.com/shadowsocks/ShadowsocksX-NG/releases <--- for Mac

## 3. Extract the ZIP / DMG file and run Shadowsocks.exe
![image](https://github.com/user-attachments/assets/b0bbd2cf-ce5d-497e-831d-a1486da02c68)

For Mac you may face error loading the app as the app is unsigned.
![image](https://github.com/user-attachments/assets/0430de74-9a80-4851-8b37-39af3963792d)

In this case Go to System Settings > Privacy and Security, scroll down
![image](https://github.com/user-attachments/assets/ea5f41ea-9fba-4c68-82a1-9de6613d0ec0)
Click "Open Anyway"

## 4. Open Shadowsocks menu
When Shadowsocks is running, locate it in the system tray at the bottom right of your screen, and right click the app icon to open its menu
For Windows:
![image](https://github.com/user-attachments/assets/93871f3a-81ed-4709-86c0-3cbbb0294700)

For Mac:
![image](https://github.com/user-attachments/assets/38af41f8-b5ef-46ca-adff-b7d4918ce33d)


## 5. Enable “Start on Boot” and “Associate ss:// Links”.
For Windows
![image](https://github.com/user-attachments/assets/6b85afbf-f1cc-4a9b-a43f-7889dbe4b6e6)

For Mac, choose Preference from dropdown menu, tick Launch at Login
![image](https://github.com/user-attachments/assets/8254e9df-8d7f-423d-b951-191b03ecba59)
![image](https://github.com/user-attachments/assets/0a062c86-c225-465a-a254-92655ef6f2d1)

Then import server URL:
![image](https://github.com/user-attachments/assets/2bda01ba-b81a-4939-89aa-50409651f197)



## 6. Hover to "System Proxy" and choose "PAC". 
(Avoid Global, it will direct all traffic thru proxy which is slow)

![image](https://github.com/user-attachments/assets/39c447f2-63b9-447c-8773-a910eef683f9)

## 7. Add a server by import URL
Ask Ross for the Shadowsocks URL separately.

![image](https://github.com/user-attachments/assets/18f17582-26c5-4f47-a867-eae1ce951809)

## 8. Click the URL to import server
Windows may ask you to confirm the action, simply click Open Link to continue.

![image](https://github.com/user-attachments/assets/3c1a04a6-9f2c-4def-b4a9-29a2306202dd)

## 9. Confirm import
Shadowsocks will prompt and ask you to confirm to import URL, click Yes.

![image](https://github.com/user-attachments/assets/4d6017c3-b931-44fb-96bd-caeb7db7bed5)

## 10. Restart Shadowsocks and verify your IP
Restart Shadowsocks, then go to https://www.myip.com/ and check your IP before proceeding to ensure the proxy is working correctly. You should see a completely different set of IP if the setup is done correctly.

![image](https://github.com/user-attachments/assets/5c3c523f-fdc6-4361-9948-b87b3aa6f7be)

## 11. Start working.

## 12. Make changes to the PAC file (Optional)
This is the rule for setting up a blacklist that needs to go thru proxy.  For now we set Claude related domains to all use proxy.

Source is here: https://github.com/chassis-app/vpn-setup/blob/main/pac.txt

Feel free to update **__RULES__** of the file row 2.  Feel free to submit your changes to include more service we need to use.

![image](https://github.com/user-attachments/assets/d818199a-5a8e-49eb-ade0-7b678cb1041e)
