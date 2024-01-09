
<h1 align="center">
  <br>
  <a href="https://play.google.com/store/apps/details?id=com.banglalink.toffee"><img src="https://github.com/Jeshan-akand/Toffee-Channels-Link-Headers/blob/main/images/toffee_logo.jpeg" alt="🔥 Toffee 🔥" width="200"></a>
  <br>
  🔥 Toffee 🔥
  <br>
</h1>

<p align="center">
<a href="#"><img title="Made in BANGLADESH" src="https://img.shields.io/badge/MADE%20IN-BANGLADESH-SCRIPT?colorA=%23ff0000&colorB=%23017e40&colorC=%23ff0000&style=for-the-badge"></a>
</p>
<p align="center">
<a href="#"><img title="Tool Name" src="https://img.shields.io/badge/Toffee channel bypass-green.svg"></a>
<a href="#"><img title="Maintainence" src="https://img.shields.io/badge/Maintained%3F-yes-green.svg"></a>
</p>
</p>
<p align="center">
<a href="https://github.com/Gtajsan"><img title="Github" src="https://img.shields.io/badge/Gtajisan-brightgreen?style=for-the-badge&logo=github"></a>
<a href="https://gmail.google.com/gmail/?view=cm&fs=1&to=ffjisan804@gmail.com"><img title="Gmail" src="https://img.shields.io/badge/Gmail-FARHAN MUH TASIM-green?style=for-the-badge&logo=Gmail"></a>
</p>
<p align="center">
<a href="https://github.com/Gtajisan"><img title="Followers" src="https://img.shields.io/github/followers/Gtajisan?color=blue&style=flat-square"></a>
<a href="https://github.com/Gtajisan"><img title="Stars" src="https://img.shields.io/github/stars/Gtajisan/Toffee-channel-bypass?color=red&style=flat-square"></a>
<a href="https://github.com/Gtajisan"><img title="Forks" src="https://img.shields.io/github/forks/Gtajisan/Toffee-channel-bypass?color=red&style=flat-square"></a>
<a href="https://github.com/Gtajisan"><img title="Watching" src="https://img.shields.io/github/watchers/Gtajisan/Toffee-channel-bypass?label=Watchers&color=blue&style=flat-square"></a>

<p align="center">  
<a href="#"><img title="Language" src="https://img.shields.io/badge/Language-black?style=for-the-badge&logo=termux"></a>
</p>

<p align="center">
 <img src="https://img.shields.io/badge/Python-FFDD00?style=for-the-badge&logo=python&logoColor=blue"/>
 </div>
</p>
<p align="center">  <a href="https://t.me/teamrxs"><img width="160" height="50" src="https://i.imgur.com/N7AK7XY.png"></a></p>
<h1 align="center">
 <a href="https://play.google.com/store/apps/details?id=com.banglalink.toffee"><img src="https://github.com/Jeshan-akand/Toffee-Channels-Link-Headers/blob/main/images/banner.jpeg"></a>
</h1>


<h2 align="center">A Script to trigger the GitHub Actions every day to update the Toffee App Channels Link and Cookie </h2>

<h1 align="center">
 <a href="https://i.postimg.cc/pLKB1yDS/toffee-logo.jpg"><img src="![image](https://github.com/Gtajisan/Toffee-channel-bypass/assets/124022055/308b16cf-5017-4e1c-a649-4bc5acaf9195)"></a>
</h1> src="" alt="🔥 Toffee 🔥" width="200"></a>
  <br>
  🔥 Toffee 🔥
  <br>
</h1>




## 📒 ABOUT TOOL : 
* [Toffee](https://play.google.com/store/apps/details?id=com.banglalink.toffee) Live is the number 1 entertainment app in Bangladesh, boasting over 10 million downloads on the Google Play Store.


## 💥Key Features

* All The Channel Links and Cookies Are Updated Every 30 Minutes
* Premium Channels Are Also Working
* Contains Link With Headers (Host, Cookie)
* In JSON Format
* You Can Easily Use This on a Website or in an App for Restreaming TV Channels 



## 🕹️How To Use
**For Developers**
* 👉 **[Auto Updated Channels Json File](https://raw.githubusercontent.com/Gtajisan/Toffee-channel-bypass/main/toffee_channel_data.json)**
* Use Get Request




```python
import requests
#Get updated the Link and Headers 
link="https://raw.githubusercontent.com/Gtajisan/Toffee-channel-bypass/main/toffee_channel_data.json"
request=requests.get(link).json()

name=request["name"]
owner=request["owner"]
channels_amount=request["channels_amount"]
channels_data=request["channels"]
for channel in channels_data:
    link=channel["link"]
    headers=channel["headers"]
    


print("✓ channel link :"+link)
print("✓ channel Headers :",headers)
#Request Toffee Main Api With Headers
request_server=requests.get(link,headers=headers)
#Get the Live m3u3 Link
print("✓ Response From Toffee Server : "+request_server.text)


```

> **Note**
> I'm using Python 3.You can use other Languages.

# 🖥️Optput
> ✓ channel link :https://bldcmprod-cdn.toffeelive.com/cdn/live/comedy_central_hd/playlist.m3u8
✓ channel Headers : {'Host': 'bldcmprod-cdn.toffeelive.com', 'cookie': 'Edge-Cache-Cookie=URLPrefix=aHR0cHM6Ly9ibGRjbXByb2QtY2RuLnRvZmZlZWxpdmUuY29tLw:Expires=1698080619:KeyName=prod_linear:Signature=RY1grOoqltoX1yPO4WMzHCQk2xIp1zGvi03K2bdefb-_QErIqzbuBwytBNV5HiSHSsDslAS2gJsuRFT_MnNJCQ'}

> ✓ Response From Toffee Server :
#EXTM3U
#EXT-X-VERSION:3
#EXT-X-STREAM-INF:PROGRAM-ID=1,BANDWIDTH=1024000,RESOLUTION=1280x720
../slang/comedy_central_hd_576/comedy_central_hd_576.m3u8?bitrate=1000000&channel=comedy_central_hd_576&gp_id=
#EXT-X-STREAM-INF:PROGRAM-ID=1,BANDWIDTH=768000,RESOLUTION=854x480
../slang/comedy_central_hd_320/comedy_central_hd_320.m3u8?bitrate=768000&channel=comedy_central_hd_320&gp_id=
#EXT-X-STREAM-INF:PROGRAM-ID=1,BANDWIDTH=512000,RESOLUTION=640x360
../slang/comedy_central_hd_160/comedy_central_hd_160.m3u8?bitrate=512000&channel=comedy_central_hd_160&gp_id=


> [Program finished]
<h1 align="center">
 <a href="https://raw.githubusercontent.com/Gtajisan/Toffee-channel-bypass/main/toffee_channel_data.json"><img src="https://i.postimg.cc/BnKj0SPD/Screenshot-20240109-231801-Chrome.png"></a>
</h1>

# 🎬How To Play
**📱Android**
* Use Network Stream Player [Download](https://play.google.com/store/apps/details?id=com.genuine.leone)
* Add This PlayList [Playlist Link](https://raw.githubusercontent.com/Gtajisan/Toffee-channel-bypass/main/toffee_NS_Player.m3u)
*  Enjoy 😊

**🖥️ Android TV**
* Use OTT Navigator [Download](https://apkpure.com/ott-navigator-iptv/studio.scillarium.ottnavigator/amp)
* Add This PlayList [Playlist Link](https://raw.githubusercontent.com/Gtajisan/Toffee-channel-bypass/main/toffee_OTT_Navigator.m3u)
*  Enjoy 😊

<h1 align="center">
 <a href="https://raw.githubusercontent.com/Gtajisan/Toffee-channel-bypass/main/toffee_channel_data.json"><img src="https://github.com/Gtajisan/Toffee-channel-bypass/blob/main/images/ns_player.jpg"></a>
</h1>
<h1 align="center">
 <a href="https://raw.githubusercontent.com/Gtajisan/Toffee-channel-bypass/main/toffee_channel_data.json"><img src="https://github.com/Gtajisan/Toffee-channel-bypass/blob/main/images/ott_view.jpg"></a>
</h1>

## CONNECT WITH US :

[![Messenger](https://img.shields.io/badge/Messenger-Chat-blue?style=for-the-badge&logo=messenger)](https://m.me/j/AbZoOyGXJvl_zUrC/)
<a href="https://github.com/Gtajisan"><img title="Github" src="https://img.shields.io/badge/FARHAN MUH TASIM-brightgreen?style=for-the-badge&logo=github"></a>
[![Instagram](https://img.shields.io/badge/FACEBOOK-FOLLOW-red?style=for-the-badge&logo=facebook)](https://facebook.com/reyadbross)
[![Instagram](https://img.shields.io/badge/FACEBOOK-FOLLOW-red?style=for-the-badge&logo=facebook)](https://www.facebook.com/profile.php?id=100094924471568&mibextid=gik2fB)
[![Instagram](https://img.shields.io/badge/WHATSAPP-CHAT-red?style=for-the-badge&logo=whatsapp)](https://wa.me/+8801305057238)
[![Instagram](https://img.shields.io/badge/INSTAGRAM-FOLLOW-red?style=for-the-badge&logo=instagram)](https://www.instagram.com/gtajsan)
[![Instagram](https://img.shields.io/badge/WEBSITE-VISIT-yellow?style=for-the-badge&logo=blogger)](https://gtajisan.github.io/Web-view/?raw=true)
[![Instagram](https://img.shields.io/badge/TELEGRAM-CHANNEL-red?style=for-the-badge&logo=telegram)](https://t.me/farhan_muh_tasim)

#### 💰YOU CAN HELP ME BY DONATING 💖💣
<p align="center">

  [![BuyMeACoffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-ffdd00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black)](https://buymeacoffee.com/FARHAN-MUHTASIM) [![PayPal](https://img.shields.io/badge/PayPal-00457C?style=for-the-badge&logo=paypal&logoColor=white)](https://paypal.me/binodxd) [![Patreon](https://img.shields.io/badge/Patreon-F96854?style=for-the-badge&logo=patreon&logoColor=white)](https://patreon.com/binodxd) [![Ko-Fi](https://img.shields.io/badge/Ko--fi-F16061?style=for-the-badge&logo=ko-fi&logoColor=white)](https://ko-fi.com/binodxd)</a>
</p>

# Acknowledgements
## Special Thanks <span style='font-size:45px;'>&#128071;</span>
<a href="#"><img title="FARHAN-MUH-TASIM" src="https://img.shields.io/badge/FARHAN MUH TASIM-black?style=for-the-badge&logo=FARHAN MUH TASIM"></a>
## Thanks For Using This Tool <span style='font-size:45px;'>&#128536;</span> <span style='font-size:45px;'>&#128525;</span>
### thanks for these topics and supported 💖🤧
- `Reyad X Shipu`
- `source code` [source](https://github.com/BINOD-XD/Toffee-Channels-Link)
- `byte-capsul`  [source](https://github.com/byte-capsule/Toffee-Channels-Link-Headers)           
