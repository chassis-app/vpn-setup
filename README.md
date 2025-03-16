# vpn-setup

## 1. Install the proxy tool
https://github.com/shadowsocks/shadowsocks-windows/releases <--- for Windows

https://github.com/shadowsocks/ShadowsocksX-NG/releases <--- for Mac

## 2. Add server

Add server by import URL.  Ask Ross for the URL separately.

![image](https://github.com/user-attachments/assets/18f17582-26c5-4f47-a867-eae1ce951809)


## 3. Make changes to the PAC file

This is the rule for setting up a blacklist that needs to go thru proxy.  For now we set Claude related domains to all use proxy.

Source is here: https://github.com/chassis-app/vpn-setup/blob/main/pac.txt

Feel free to update **__RULES__** of the file row 2.  Feel free to submit your changes to include more service we need to use.

![image](https://github.com/user-attachments/assets/d818199a-5a8e-49eb-ade0-7b678cb1041e)


Also remember to set the client to work in PAC mode (not global.  Global will direct all traffic thru proxy which is slow)

## 4. Restart Shadowsocks client


## 5. Test if the setup is functional.

Suggest go to whatismyipaddress.com and www.myip.com in browser.  they should give you different IP if all setup is correct.

## 6. Start working.
