# Crunchyroll iFrame Player [![Built with love](https://img.shields.io/badge/made%20with-javascript-yellow?style=for-the-badge)](https://github.com/ mateus7g/crp-iframe-player/releases/latest) [![Downloads](https://img.shields.io/github/downloads/mateus7g/crp-iframe-player/total.svg?style=for-the- badge)](https://github.com/mateus7g/crp-iframe-player/releases/latest)

This is a community extension that allows you to watch all Crunchyroll content.  
Originally created by [itallolegal](https://github.com/itallolegal) (deactivated) and [Hyper-Tx](https://github.com/Hyper-Tx), currently maintained by [Mateus7G](https:/ /github.com/Mateus7G).  
A special thanks to all contributors.

Thanks for using. :)

## Download
You can find the latest available versions below:  


<a href="https://github.com/mateus7g/crp-iframe-player/releases/latest" target="_blank"><img align="right" alt="Desktop" src="https:// img.shields.io/badge/desktop-v1.3.0-violet?style=for-the-badge&logo=windows"></a>

#### Desktop (PC)

Currently the Desktop version is available [here](https://github.com/Mateus7G/crp-iframe-player/releases/latest).  
To install see the step by step [for pc](#%EF%B8%8F-how-to-install-desktop).

<a href="https://github.com/Mateus7G/crp-iframe-player/releases/latest" target="_blank"><img align="right" alt="Android" src="https:// img.shields.io/badge/android-v1.3.0-violet?style=for-the-badge&logo=android"></a>

#### Android (Kiwi)

Latest version for Kiwi Browser is available [here](https://github.com/Mateus7G/crp-iframe-player/releases/latest).  
To install see the step by step [for android](#-how-to-install-android).     


## 🖥️ How to install? (desktop)
The Desktop extension only works on **Chromium-based** browsers such as: Google Chrome, Opera, etc.  
Make sure your browser is up to date and proceed:


<img align="right" width="350" height="124" alt="Extracting downloaded file" src="https://raw.githubusercontent.com/mateus7g/crp-iframe-player/master/Screenshots/installation -3.png?raw=true">

**1** ➜ [download](#download) the `Crunchyroll_Premium.zip` file, and extract it:

**2** ➜ Enter the [extensions](https://raw.githubusercontent.com/mateus7g/crp-iframe-player/master/Screenshots/instalacao-1.png?raw=true) tab of your browser ( or go directly to [`chrome://extensions`](chrome://extensions))
 
**3** ➜ Enable the **Programmer Mode**, and then click the **Load Expanded** button:

 ![Enabling developer mode, and loading extension](https://raw.githubusercontent.com/mateus7g/crp-iframe-player/master/Screenshots/instalacao-2.png?raw=true)
 
**4** ➜ Select the folder [which was extracted](https://raw.githubusercontent.com/mateus7g/crp-iframe-player/master/Screenshots/instalacao-4.png?raw=true) at the beginning of the tutorial

<img align="right" width="350" height="190" alt="Details of installed extension" src="https://raw.githubusercontent.com/mateus7g/crp-iframe-player/master/Screenshots/ install-5.png?raw=true">

**5** ➜ If you did everything right, you should see a card like this in your browser.
 
**6** ➜ Now just watch 😉

<br /><br /><br />

## 📱 How to install? (android)
The Android extension only works in Kiwi Browser.  
Make sure your browser is up to date and proceed:

<img align="right" width="350" height="233" alt="Kiwi Browser on Play Store" src="https://raw.githubusercontent.com/mateus7g/crp-iframe-player/master/Screenshots /installation-kiwi-1.png?raw=true&v=2">

**1** ➜ Please [download](#download) the `Crunchyroll_Premium_Kiwi-Browser.zip` file, no need to extract.

**2** ➜ Download and open Kiwi Browser, available on [Google Play Store](https://play.app.goo.gl/?link=https://play.google.com/store/apps /details?id=com.kiwibrowser.browser&ddl=1&pcampaignid=web_ddl_1):  

**3** ➜ Enter the [extensions](https://raw.githubusercontent.com/mateus7g/crp-iframe-player/master/Screenshots/instalacao-kiwi-2.png?raw=true) tab of your browser (or go directly to [`chrome://extensions`](chrome://extensions))

**4** ➜ Enable **Developer Mode**, then click **Load**  

![Enabling developer mode and loading the extension](https://raw.githubusercontent.com/mateus7g/crp-iframe-player/master/Screenshots/instalacao-kiwi-3.png?raw=true)

**5** ➜ Choose the `.zip` file downloaded at the beginning of the tutorial

<img align="right" width="350" height="190" alt="Details of installed extension" src="https://raw.githubusercontent.com/mateus7g/crp-iframe-player/master/Screenshots/ kiwi-4.png installation?raw=true">

**6** ➜ If you did everything right, you should see a card like this on your screen.  

**7** ➜ Now just watch 😉

<br /><br /><br />

## 🦊 Firefox
If you use a browser based on Mozilla Firefox you can also test the version adapted by Rgern100 ([#38](https://github.com/Mateus7G/crp-iframe-player/issues/38#issuecomment-1193372108)) here:  
https://github.com/Rgern100/crp-iframe-player-Firefox

## 🙉 Tampermonkey
If you are using the player version of this repository (mateus7g.github.io), using the player through Tampermonkey (and not through the extension) can cause problems with CORS (and receive a [Code 232011](https://greasyfork.org /en-US/scripts/411391-crunchyroll-iframe-player/discussions/142287), see [#50](https://github.com/Mateus7G/crp-iframe-player/issues/50)).  
To solve this, just pass in the `ifrm.contentWindow.postMessage({ ... })` function the key `'tampermonkey'` with the value `true`.  

UserScript 1 (by luiz-lp): https://github.com/luiz-lp/crpiframeplayer  
UserScript 2 (by JarEdMaster): https://greasyfork.org/en-US/scripts/411391-crunchyroll-iframe-player  
**Note:** I am not responsible for maintaining these scripts  

**Messages that can currently be sent to the player via script:**

```yml
tampermonkey: use a proxy to make requests
lang: default locale/language code
playback: not currently used
beta: if using crunchyroll in beta (requires passing old_url)
old_url: url of the video in the old version of the site
up_next_enable: Automatically skip episodes (when up_next is informed)
up_next_cooldown: seconds to end and show next episode popup (0 to disable popup)
up_next: url of next video to be played/redirected (requires up_next_enable)
force_mp4: force videos to play in mp4 and not m3u8 (enabling this option will slow down loading, recommended for chromecasting only)
webvideocaster: swap download button for WebVideoCaster casting
```

## 📝 Crunchyroll Beta Warning
The new Crunchyroll site **completely breaks** the extension: [26#issuecomment-1006569041](https://github.com/Mateus7G/crp-iframe-player/issues/26#issuecomment-1006569041)  

The new versions (v1.1.0+) are **still** compatible because when you access the new site, your browser pulls the video data from the old site.  
This means that if the old version of Crunchyroll is **completely replaced** the extension will stop working permanently.
