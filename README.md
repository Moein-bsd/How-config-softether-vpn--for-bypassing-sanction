# How-config-softether-vpn--for-bypassing-sanction
In this repo, the steps of setting up vpn (Ethernet protocol over HTTPS) are taught step by step:


  <img alt="SoftEther_VPN" src="https://en.wikipedia.org/wiki/SoftEther_VPN#/media/File:Softethervpn_ss.jpg">


1.Run the following commands with your eyes closed:
```
apt-get update
apt-get upgrade -y
apt-get -y install build-essential wget make curl gcc  wget zlib1g-dev tzdata git libreadline-dev libncurses-dev libssl-dev

```
2.Go to the [this link](https://www.softether-download.com/en.aspx?product=softether/) and find Download link last version SoftEther_VPN_Server
and download it :

(for  example [SoftEther_VPN_Server for linux Intel CPU](https://https://www.softether-download.com/files/softether/v4.42-9798-rtm-2023.06.30-tree/Linux/SoftEther_VPN_Server/64bit_-_Intel_x64_or_AMD64/softether-vpnserver-v4.42-9798-rtm-2023.06.30-linux-x64-64bit.tar.gz/) )
```
wget "https://https://www.softether-download.com/files/softether/v4.42-9798-rtm-2023.06.30-tree/Linux/SoftEther_VPN_Server/64bit_-_Intel_x64_or_AMD64/softether-vpnserver-v4.42-9798-rtm-2023.06.30-linux-x64-64bit.tar.gz"

```
3.then:
```
ls
tar  xzf “downloaded file name”
cd vpnserver
Cd ..
mv vpnserver /usr/local
cd /usr/local/vpnserver/
chmod 600 *
chmod 700 vpnserver vpncmd
./vpnserver start
./vpncmd

###### In vpn server config
#1 for first question enter: 1
#2 for virtual hub question: just Push Enter Key3 then for command : "server :":
ServerPasswordSet
(Enter complex password)
then press ctrl+c to exit vpn config

```
4.







