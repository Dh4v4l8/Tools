## Nessus installation command :

1. `https://www.tenable.com/downloads/nessus` yaha se nessus download karo.
2. download kiye gaye nessus ko install karo
```
sudo apt install ./Nessus-10.11.0-ubuntu1604_amd64.deb
```
3. nessus ko start karo
```
sudo systemctl start nessusd
```
4. is commanad se status dekho ki chalu hey nessus ya nahi
```
sudo systemctl status nessusd
```
5. yaha se access karo.
```
https://127.0.0.1:8834/
```
## Nessus key genrate :
1. is tool se nessus ki key genrate kar sakte ho free ke liye.
```
https://github.com/harshdhamaniya/nessuskeygen
```

## Nessus uninstallation command :
1. `sudo systemctl start nessusd`
2. `sudo dpkg -r Nessus`
   Agar NessusAgent use kar rahe ho to:
   `sudo dpkg -r NessusAgent`
3. `sudo rm -rf /opt/nessus`   
