---
title: "Install Guide"
author: "Fizz VPN"
showToc: true
TocOpen: true
draft: false
hidemeta: false
hideAuthor: true
comments: false
description: "Installation and configuration guide"
#canonicalURL: "https://canonical.url/to/page"
disableShare: false
disableHLJS: false
hideSummary: false
searchHidden: true
ShowReadingTime: false
ShowBreadCrumbs: true
ShowPostNavLinks: true
ShowWordCount: false
ShowRssButtonInSectionTermList: false
UseHugoToc: false
#cover:
#    image: "<image path/url>" # image path/url
#    alt: "<alt text>" # alt text
#    caption: "<text>" # display caption under cover
#    relative: false # when using page bundles set this to true
#    hidden: true # only hide on current single page
---

# ❗️IMPORTANT INFO❗️

1. **Subscription is a key-link** that you receive, like *https://xfizz...*
	>***You don't need to click on it***

2. All information about new locations, server changes, the need to update your subscription, etc. is here:
	>[Our Telegram Channel](https://t.me/FizzVPN)

3. Receiving a subscription may take **up to 10 seconds.**

4. If instead of one of the servers the following message appears:  

	> ⛔ **XX UNAVAILABLE** ⛔

	then you need to update your subscription again in 5 minutes. If it doesn’t help, it means the server is currently unavailable.

# Windows 10/11, Linux

## NekoRay

1. **Install the latest release for your OS.**

	![NekoRay Github](/install-guide/nekoray-github.png)

	**Download:** {{< rawhtml >}}
<a href="https://github.com/Mahdi-zarei/nekoray/releases" target="_blank" title="GitHub">GitHub</a><br><br>
{{< /rawhtml >}}

2. **Run the program according to your OS. On Windows it is `nekoray.exe` with a "cats in a box" icon.**

	>**Important!** Run ***with administrator rights*** *(required for VPN mode)*.

	> After starting in the Windows ***firewall window, be sure to put two ticks (private and public network)***.
	>> If the antivirus **DRWEB** is installed, then you need to add a folder for the program, **as well as nekoray.exe and nekobox_core.exe in the exception of antivirus.**    

	>**In the case of problems with the launch on Windows, you need to install two official packages from Microsoft:**  
	**1:** {{< rawhtml >}}
<a  href="https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170#latest-microsoft-visual-c-redistributable-version" target="_blank" title="Redist Visual C++ for Visual Studio 2015-2022">Redist Visual C++ for Visual Studio 2015-2022</a>
{{< /rawhtml >}}  
	**2:** {{< rawhtml >}}
<a  href="https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170#visual-studio-2013-vc-120--no-longer-supported" target="_blank" title="Redist Visual C++ for Visual Studio 2013">Redist Visual C++ for Visual Studio 2013</a><br>
{{< /rawhtml >}}

3. **Copy the subscription and select “Program” -> “Add profile from a clipboard” from the menu. In the window that opens, select “As a subscription (add a new group)” and click OK. Next "Settings" -> Groups and delete the default group.**

	![NekoRay-2](/install-guide/nekoray-2-1.gif)

4. **Select “Program” -> “Remember last profile” from the menu. Next, be sure to check the “TUN Mode” checkbox in the upper right corner, then select the server, “RMB” -> “Run”.** Further in the Windows firewall window (if you use it) ***be sure to put two checkmarks (private and public network) ***, otherwise the program ***will not work ***.  


	>If you only need a VPN for the browser, you can select the “System Proxy” mode.  

	> **Important!** After disconnecting, it is necessary to remove the checkmark **“System proxy”**, otherwise **the Internet will not work**.  

	![NekoRay-2](/install-guide/nekoray-3.gif)

-------------

{{< rawhtml >}} <center> {{< /rawhtml >}} 
### Split tunneling: Whitelist
{{< rawhtml >}} </center> {{< /rawhtml >}}
***Selected programs through VPN, everything else without VPN***  

>**Before setting up, make sure that the VPN is working!**

1.  Open **Settings -> Route settings -> Route** tab. Press New.  

	![NekoRay-Whitelist-1](/install-guide/nekoray-whitelist-1.png)  

2.  In the window opened, enter **any name of the profile**, press **New**, select *attribute*: **Process_name** and *outbound*: **proxy**. In the window from the bottom right, enter **processes that you want to work through VPN, one on the line**.

	![NekoRay-Whitelist-2](/install-guide/nekoray-whitelist-2.png)  

3.  Press twice **OK**, and after that **restart the program through the tray (this is important)**. Next, open **Settings -> Route settings -> General tab**. Select the newly created profile in the **routing profile** field, below **Default outbound** select **Direct**.

	![NekoRay-Whitelist-3](/install-guide/nekoray-whitelist-3.png)  


--------
  
{{< rawhtml >}} <center> {{< /rawhtml >}} 
### Split tunneling: Blacklist    
{{< rawhtml >}} </center> {{< /rawhtml >}}
***All through VPN, except for selected programs***  

>**Before setting up, make sure that the VPN is working!** 

1.  Open **Settings -> Route settings -> Route** tab. Press New.  

	![NekoRay-Whitelist-1](/install-guide/nekoray-whitelist-1.png)  

2.  In the window opened, enter **any profile name**, press **New**, select *attribute*: **Process_name** and *outbound*: **Direct**. In the window from the bottom right, enter **processes that you want to work without VPN, one on the line**.

	![NekoRay-Blacklist-1](/install-guide/nekoray-blacklist-1.png)  

3.  Press twice **OK**, and after that **restart the program through the tray (this is important)**. Next, open **Settings -> Route settings -> General tab**. Select the newly created profile in the **routing profile** field.

	![NekoRay-Blacklist-2](/install-guide/nekoray-blacklist-2.png)  

-------------

## Hiddify Next

1. **Install latest release for your OS.**

	![Hiddify Next Github](/install-guide/hiddify-github-pc.png)

	**Download:** {{< rawhtml >}}
<a href="https://github.com/hiddify/hiddify-next/releases" target="_blank" title="GitHub">GitHub</a>
{{< /rawhtml >}}
	
2. **Run the program according to your OS. On Windows it is `Hiddify.exe`**

	>**Important!** Run ***with administrator rights*** *(required for VPN mode)*.
	>> If the antivirus **DRWEB** is installed, then you need to add a folder for the program, **as well as Hiddify.exe and HiddifyCli.exe in the exception of antivirus.**    

	>**In the case of problems with the launch on Windows, you need to install two official packages from Microsoft:**  
	**1:** {{< rawhtml >}}
<a  href="https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170#latest-microsoft-visual-c-redistributable-version" target="_blank" title="Redist Visual C++ for Visual Studio 2015-2022">Redist Visual C++ for Visual Studio 2015-2022</a>
{{< /rawhtml >}}  
	**2:** {{< rawhtml >}}
<a  href="https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170#visual-studio-2013-vc-120--no-longer-supported" target="_blank" title="Redist Visual C++ for Visual Studio 2013">Redist Visual C++ for Visual Studio 2013</a><br>
{{< /rawhtml >}}

	![Hiddify-1](/install-guide/hiddify-1.png)

	**Region**:
	For the Russian Federation, we recommend choosing the region “Russia”, in all other cases “Other”.
	> **When selecting the “Russia” region, access to all .RU sites and all IP addresses of the Russian Federation will be “direct” (without VPN).**
	Therefore, do not use 2ip.ru to check the location.

	>***Analytics collection***: we recommend disabling it.

3. **Copy the subscription and click “New Profile” on the screen that opens. Next "Add profile from clipboard".**

	![Hiddify-1](/install-guide/hiddify-2.gif)


4. **In the upper right corner, click on the “Settings” icon and select the “VPN" mode.**
	
	>If you only need VPN for browsing, you can keep it at "System Proxy."
	
	![Hiddify-4](/install-guide/hiddify-3.png)

5. **Connect, go to the ***Proxy*** tab and ***Select a server***.**

	>If you get **Timeout** when connecting, and in the **Proxies** tab all or almost all servers show ❌, then you need to:
	Go to the **Configuration Options** tab, find the **Direct DNS** item and change it to:

	>>***https://8.8.8.8/dns-query***
	
	>Changing a server can take up to 10 seconds.

	>It is recommended to check the server latency again by clicking on the Lightning icon at the bottom right. Hiddify always “overestimates” the delay by several times and can even show that the server is unavailable, although this is not the case.

	![Hiddify-5](/install-guide/hiddify-4.png)

-------------

## Other clients

**Invisible Man - XRay**:  
{{< rawhtml >}}
<a  href="https://github.com/InvisibleManVPN/InvisibleMan-XRayClient/releases" target="_blank" title="GitHub">https://github.com/InvisibleManVPN/InvisibleMan-XRayClient/releases</a>
{{< /rawhtml >}}

-------------

# iOS/Mac

## Streisand

**Download:** {{< rawhtml >}}
<a href="https://apps.apple.com/app/streisand/id6450534064" target="_blank" title="App Store">App Store</a>
{{< /rawhtml >}}

Copy the received subscription and then follow the instructions:

![Streisand](/install-guide/streisand.png)

*To update an existing subscription, you need to long-tap on “Subscription”, there will be an “Update” button inside.*

-------------

## Hiddify (AppStore)

**Скачать:** {{< rawhtml >}}
<a  href="https://apps.apple.com/ru/app/hiddify-proxy-vpn/id6596777532" target="_blank" title="App Store">App Store</a>
{{< /rawhtml >}}

Next, copy the resulting subscription and add as shown below.After adding, switch to the "proxy" tab and select the desired location.  

![Hiddify](/install-guide/hiddify-android.png)

-------------

## Shadowrocket [2.99 $]

**Buy:** {{< rawhtml >}}
<a href="https://apps.apple.com/app/shadowrocket/id932747118" target="_blank" title="App Store">App Store</a>
{{< /rawhtml >}}

Copy the received subscription and then follow the instructions:

![Shadowrocket](/install-guide/shadowrocket.png)

-------------

## Happ

**Скачать:** {{< rawhtml >}}
<a  href="https://apps.apple.com/ru/app/happ-proxy-utility/id6504287215" target="_blank" title="App Store">App Store</a>
{{< /rawhtml >}}

Next, copy the received subscription and add by analogy with other applications above. 

-------------

## V2Box

**This application is tired only if others do not work! (For example Mac on Intel processors)**  

>For MacOS there is an alternative to GitHub according to the Hiddify Next instructions for Win 10/11, just download the DMG package.

**Download:** {{< rawhtml >}}
<a href="https://apps.apple.com/app/v2box-v2ray-client/id6446814690" target="_blank" title="App Store">App Store</a>
{{< /rawhtml >}}

Copy the received subscription and then follow the instructions:

![v2box](/install-guide/v2box.png)

-------------

# Android

## Hiddify

**Download:** {{< rawhtml >}}
<a href="https://github.com/hiddify/hiddify-next/releases/tag/v2.0.5" target="_blank" title="GitHub">GitHub</a>
{{< /rawhtml >}}(APK Universal)  

>**Do not download from Play Store! That version is broken.**  

**Region**:
For the Russian Federation, we recommend choosing the region “Russia”, in all other cases “Other”.
>**When selecting the “Russia” region, access to all .RU sites and all IP addresses of the Russian Federation will be “direct” (without VPN).**
Therefore, do not use 2ip.ru to check the location.

>Next, copy the received subscription and add it as shown below. After adding, switch to the "Proxy" tab and select the desired location.

![Hiddify](/install-guide/hiddify-android.png)

--------------

## v2rayNG

**Download:** {{< rawhtml >}}
<a href="https://play.google.com/store/apps/details?id=com.v2ray.ang" target="_blank" title="Play Store">Play Store</a>
{{< /rawhtml >}}

Copy the received subscription and then follow the instructions:

![v2rayNG](/install-guide/v2rayNG.png)

--------------

# Update subscription

## Hiddify

![Hiddify](/install-guide/hiddify-update.png)

## NekoRay

![NekoRay](/install-guide/nekoray-update-1.png)

## Streisand 

![Streisand](/install-guide/streisand-update.png)

## V2Box

![V2box](/install-guide/v2box-update.png)

## v2rayNG

![V2rayNG](/install-guide/v2rayng-update.png)

{{< rawhtml >}}<center><b>The End :)</b></center>{{< /rawhtml >}}