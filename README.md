# Awesome-Google-Dorks
<div align="center">
	<img width="500" height="350" src="https://github.com/sindresorhus/awesome/raw/main/media/logo.svg" alt="Awesome">

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A collection of Awesome Google Dorks.
</div>

## Contents

- [Search Operators](#search-operators)
- [Documents and Files](#documents-and-files)
- [Cameras and Webcams](#cameras-and-webcams)
- [Control Panels](#control-panels)
- [Email](#email)
- [Google Drive](#google-drive)
- [IoT Devices](#iot-devices)
- [Login](#login)
- [Movies](#movies)
- [Network Devices](#network-devices)
- [WordPress](#wordpress)

# Search Operators
| Operator         | Description                                                                                                              | Syntax                               | Example                           |
| ---------------- | ------------------------------------------------------------------------------------------------------------------------ | ------------------------------------ | --------------------------------- |
| ()               | Group multiple terms or operators. Allows advanced expressions                                                           | (&lt;term> or &lt;operator>)         | inurl:(html \| php)               |
| *                | Wildcard. Matches any word                                                                                               | &lt;text> * &lt;text>                | How to * a computer               |
| ""               | The given keyword has to match exactly. *case-insensitive*                                                               | "&lt;keywords>"                      | "google"                          |
| m..n / m...n     | Search for a range of numbers. *n* should be greater than *m*                                                            | &lt;number>..&lt;number>             | 1..100                            |
| -                | Documents that match the operator are excluded. *NOT*-Operator                                                           | -&lt;operator>                       | -site:youtube.com                 |
| +                | Include documents that match the operator                                                                                | +&lt;operator>                       | +site:youtube.com                 |
| \|               | Logical *OR-Operator*. Only one operator needs to match in order for the overall expression to match                     | &lt;operator> \| &lt;operator>       | "google" \| "yahoo"               |
| ~                | Search for synonyms of the given word. Not supported by Google                                                           | ~&lt;word>                           | ~book                             |
| @                | Perform a search only on the given social media platform. Rather use **site**                                            | @&lt;socialmedia>                    | @instagram                        |
| after            | Search for documents published / indexed after the given date                                                            | after:&lt;yy(-mm-dd)>                | after:2020-06-03                  |
| allintitle       | Same as **intitle** but allows multiple keywords seperated by a space                                                    | allintitle:&lt;keywords>             | allintitle:dog cat                |
| allinurl         | Same as **inurl** but allows multiple keywords seperated by a space                                                      | allinurl:&lt;keywords>               | allinurl:search com               |
| allintext        | Same as **intext** but allows multiple keywords seperated by a space                                                     | allintext:&lt;keywords>              | allintext:math science university |
| AROUND           | Search for documents in which the first word is up to *n* words away from the second word and vice versa                 | &lt;word1> AROUND(&lt;n>) &lt;word2> | google AROUND(10) good            |
| author           | Search for articles written by the given author if applicable                                                            | author:&lt;name>                     | author:Max                        |
| before           | Search for documents published / indexed before the given date                                                           | before:&lt;yy(-mm-dd)>               | before:2020-06-03                 |
| cache            | Search on the cached version of the given website. Uses Google's cache to do so                                          | cache:&lt;domain>                    | cache:google.com                  |
| contains         | Search for documents that link to the given fileype. Not supported by Google                                             | contains:&lt;filetype>               | contains:pdf                      |
| date             | Search for documents published within the past *n* months. Not supported by Google                                       | date:&lt;number>                     | date:3                            |
| define           | Search for the definition of the given word                                                                              | define:&lt;word>                     | define:funny                      |
| ext              | Search for a specific filetype                                                                                           | ext:&lt;documenttype>                | ext:pdf                           |
| filetype         | Refer to **ext**                                                                                                         | filetype:&lt;documenttype>           | filetype:pdf                      |
| inanchor         | Search for the given keyword in a website's anchors                                                                      | inanchor:&lt;keyword>                | inanchor:security                 |
| index of         | Search for documents containing direct downloads                                                                         | index of:&lt;term>                   | index of:mp4 videos               |
| info             | Search for information about a website                                                                                   | info:&lt;domain>                     | info:google.com                   |
| intext           | Keyword needs to be in the text of the document                                                                          | intext:&lt;keyword>                  | intext:news                       |
| intitle          | Keyword needs to be in the title of the document                                                                         | intitle:&lt;keyword>                 | intitle:money                     |
| inurl            | Keyword needs to be in the URL of the document                                                                           | inurl:&lt;keyword>                   | inurl:sheet                       |
| link / links     | Search for documents whose links contain the given keyword. Useful for finding documents that link to a specific website | link:&lt;keyword>                    | link:google                       |
| location         | Show documents based on the given location                                                                               | location:&lt;location>               | location:USA                      |
| numrange         | Refer to **m..n**                                                                                                        | numrange:&lt;number>-&lt;number>     | numrange:1-100                    |
| OR               | Refer to **\|**                                                                                                          | &lt;operator> OR &lt;operator>       | "google" OR "yahoo"               |
| phonebook        | Search for related phone numbers associated with the given name                                                          | phonebook:&lt;name>                  | phonebook:"william smith"         |
| relate / related | Search for documents that are related to the given website                                                               | relate:&lt;domain>                   | relate:google.com                 |
| safesearch       | Exclude adult content such as pornographic videos                                                                        | safesearch:&lt;keyword>              | safesearch:sex                    |
| source           | Search on a specific news site. Rather use **site**                                                                      | source:&lt;news>                     | source:theguardian                |
| site             | Search on the given site. Given argument might also be just a TLD such as **com, net**, etc                              | site:&lt;domain>                     | site:google.com                   |
| stock            | Search for information about a market stock                                                                              | stock:&lt;stock>                     | stock:dax                         |
| weather          | Search for information about the weather of the given location                                                           | weather:&lt;location>                | weather:Miami                     |

From [chr3st5an](https://github.com/chr3st5an/Google-Dorking.git)

# Disclaimer
USE AT YOUR OWN RISK! 
Google Dorking can be used for Cybersecurity, Penetration, and Vulnerability testing. However, some things may lead to illegal activity or concern people's sensitive data.

To protect yourself use a Tor Browser and for even better protection use a VPN. 

# Documents and Files
- `filetype:pdf intitle:"Confidental"`
- `filetype:doc intitle:"Confidental"`
- `filetype:xls intitle:"Confidental"`
- `filetype:ppt intitle:"Confidental"`

# Cameras and Webcams
- `intitle:"D-Link" inurl:"/video.htm"`
- `intitle:"Linksys Viewer - Login" -inurl:mainFrame`
- `intitle:"Live View /-AXIS"`
- `intitle:"netcam watcher"`
- `intitle:"Network Camera NetworkCamera"`
- `intitle:"TP-LINK IP-Camera"`
- `intitle:"webcamXP 5"`
- `inurl:"axis-cgi/mjpg"`
- `inurl:"control/userimage.html"`
- `inurl:"/image/webcam.jpg"`
- `inurl:"/live/cam.html"`
- `inurl:"main.cgi?next_file=main_fs.htm"`
- `inurl:"/mjpg/video.mjpg"`
- `inurl:"MultiCameraFrame?Mode=Motion"`
- `inurl:"/out.jpg"`
- `inurl:"snapshot.cgi?user="`
- `inurl:top.htm inurl:currenttime`
- `inurl:"view/index.shtml"`
- `inurl:"view/indexFrame.shtml"`
- `inurl:"view/viewer_index.shtml"`
- `inurl:"viewerframe?mode=motion"`
- `inurl:"webcam.html"`
- `intitle:webcamxp inurl:8080`

# Control Panels
- `intitle:"Admin Login"`
- `intitle:"Control Panel" inurl:/admin`
- `intitle:"Control Panel" inurl:/login`

# Directories
- `intitle:"Browse Directory"`
- `intitle:index.of`
- `intitle:"Index of" inurl:/parent-directory`
- `intitle:"Index of" inurl:/admin`
- `intitle:"Index of" inurl:/backup`
- `intitle:"Index of" inurl:/config`
- `intitle:"Index of" inurl:/logs`

# Email
- `filetype:txt @gmail.com OR @yahoo.com OR @hotmail.com OR @aol.com`
- `filetype:xls inurl:"email.xls"`

# Google Drive
- `site:drive.google.com confidential`

# IoT Devices
- `intitle:"Amazon Echo" "setup"`
- `intitle:"Baby Monitor" inurl:"/live"`
- `intitle:"Doorbell Camera" inurl:"/setup"`
- `intitle:"Google Home" "setup"`
- `intitle:"Router Login" inurl:/login`
- `intitle:"Smart Lighting Control Panel"`
- `intitle:"Sonos - Google Chrome"`
- `intitle:"Thermostat" inurl:"/status"`
- `intitle:"Smart TV" inurl:/cgi-bin/login`
- `intext:"SMART TV" inurl:password.txt`
- `inurl:"description.xml" "Philips hue bridge"`
- `inurl:"/smartlock" intitle:"Login"`

# Login
- `intitle:login`
- `intitle:login inurl:/admin`
- `intitle:login inurl:/login`
- `inurl:login`
- `inurl:"/admin/login.php"`

# Movies
- `inurl:mkv+[movie name]`
- `inurl:mp4+[movie name]`

# Network Devices
- `intext:"printer meter"`
- `intitle:”Brother” intext:”View Configuration”`
- `intitle:"Device name" inurl:home.htm`
- `intitle:”Network Print Server” filetype:html`
- `intitle:”HP LaserJet” inurl:SSI/index.htm`
- `intitle:"open network devices"`

# WordPress
- `intext:”Powered by WordPress”`
- `intitle:”Login — WordPress”`
- `intitle:"powered by WordPress" version`
- `inurl:wp-content/plugins/`
- `inurl:/wp-content/plugins/revslider/`
