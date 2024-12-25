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

3. **After launch, you need to adjust the settings** *(to eliminate DNS leak)*.
	To do this, select “Settings” -> “TUN mode settings” in the menu. In the window that opens, check the "Strict Route" box and click OK.

	>If you fail to connect at the end, try unchecking this box and try connecting again.

	![NekoRay-1](/install-guide/nekoray-1.gif)

4. **Copy the subscription and select “Program” -> “Add profile from a clipboard” from the menu. In the window that opens, select “As a subscription (add a new group)” and click OK. Next "Settings" -> Groups and delete the default group.**

	![NekoRay-2](/install-guide/nekoray-2-1.gif)

5. **Select “Program” -> “Remember last profile” from the menu. Next, be sure to check the “TUN Mode” checkbox in the upper right corner, then select the server, “RMB” -> “Run”.**

	>If you only need a VPN for the browser, you can select the “System Proxy” mode.

	![NekoRay-2](/install-guide/nekoray-3.gif)

-------------

## Hiddify Next

1. **Install latest release for your OS.**

	![Hiddify Next Github](/install-guide/hiddify-github-pc.png)

	**Download:** {{< rawhtml >}}
<a href="https://github.com/hiddify/hiddify-next/releases" target="_blank" title="GitHub">GitHub</a>
{{< /rawhtml >}}
	
2. **Run the program according to your OS. On Windows it is `Hiddify.exe`**

	>**Important!** Run ***with administrator rights*** *(required for VPN mode)*.

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

# iOS/Mac

-------------

## Streisand

**Download:** {{< rawhtml >}}
<a href="https://apps.apple.com/app/streisand/id6450534064" target="_blank" title="App Store">App Store</a>
{{< /rawhtml >}}

Copy the received subscription and then follow the instructions:

![Streisand](/install-guide/streisand.png)

*To update an existing subscription, you need to long-tap on “Subscription”, there will be an “Update” button inside.*

-------------

## Shadowrocket [2.99 $]

**Buy:** {{< rawhtml >}}
<a href="https://apps.apple.com/app/shadowrocket/id932747118" target="_blank" title="App Store">App Store</a>
{{< /rawhtml >}}

Copy the received subscription and then follow the instructions:

![Shadowrocket](/install-guide/shadowrocket.png)

-------------

## V2Box

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

{{< rawhtml >}}<center><b>The End</b></center>{{< /rawhtml >}}