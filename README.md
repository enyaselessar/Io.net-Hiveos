# Io.net-Hiveos

## 1/.Download hiveOS version [0.6-224-beta@230911.img.xz] or latest img, from this link: https://download.hiveos.farm/history/
![image](https://github.com/enyaselessar/Io.net-Hiveos/assets/108255403/7c1dc202-0c35-45f6-9526-887cb7eae67d)

## 2/.Burn the hiveOS using Etcher.io into the hard drive of the machine you want to rent
![image](https://github.com/enyaselessar/Io.net-Hiveos/assets/108255403/5b981c77-7c3c-453d-9397-f9bef0ab89a7)

## 3/.Add a new worker in HiveOS
![image](https://github.com/enyaselessar/Io.net-Hiveos/assets/108255403/10f192c7-d2b5-4423-86d9-963538cee6c8)

## 4/. In Settings, Enter the Rig ID and Password in the rig
![image](https://github.com/enyaselessar/Io.net-Hiveos/assets/108255403/c881b22b-9e1f-46f8-9ce0-0ee8dd4ca238)

# Then enter the following commands in the rig hiveos terminal
1
```
sudo apt-get update -y
```
2
```
sudo apt-get install -y gnupg1
```
3
```
cd ~
```
4
```
wget https://raw.githubusercontent.com/ionet-official/io-net-official-setup-script/main/ionet-setup.sh
```
5
```
chmod +x ionet-setup.sh
```
6
```
./ionet-setup.sh
```
7
```
sudo reboot
```
8
##### (to check all your graphic cards are connected)
```
nvidia-smi
```

9
#### Get your device name, deviceid and user id from the workers page
![image](https://github.com/enyaselessar/Io.net-Hiveos/assets/108255403/18a40d16-ee49-4dca-8f7a-eb837c93e210)

```
docker run -d -v /var/run/docker.sock:/var/run/docker.sock -e DEVICE_NAME="yourdevicename" -e DEVICE_ID=yourdeviceid -e USER_ID=youruserid -e USEGPUS=true --pull always ionetcontainers/io-launch:v0.1
```

![image](https://github.com/enyaselessar/Io.net-Hiveos/assets/108255403/f39c3733-6a1d-432a-939e-3fbc49c9c21b)



