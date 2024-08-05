---
title: "Инструкция"
author: "Fizz VPN"
showToc: true
TocOpen: true
draft: false
hidemeta: false
hideAuthor: true
comments: false
description: "Инструкция по установке и настройке"
#canonicalURL: "https://canonical.url/to/page"
disableShare: false
disableHLJS: false
hideSummary: false
searchHidden: true
ShowReadingTime: true
ShowBreadCrumbs: true
ShowPostNavLinks: true
ShowWordCount: true
ShowRssButtonInSectionTermList: false
UseHugoToc: false
#cover:
#    image: "<image path/url>" # image path/url
#    alt: "<alt text>" # alt text
#    caption: "<text>" # display caption under cover
#    relative: false # when using page bundles set this to true
#    hidden: true # only hide on current single page
---

# ❗️ВАЖНАЯ ИНФОРМАЦИЯ❗️

1. **Подписка — это ключ-ссылка**, которую вы получаете, вида *https://get...*
	>***Переходить по ней не надо!***

2. Вся информация о новых локациях, изменении серверов, необходимости обновить подписку и т.д. тут:
	>[Наш Telegram Канал](https://t.me/FizzVPN)

3. Получение подписки может занимать **до 10 секунд.**

4. В случае, если вместо какого-то из серверов появилась надпись:  

	> ⛔ **XX UNAVAILABLE** ⛔
	
	то необходимо повторно обновить подписку. Если не помогло, то значит в данный момент сервер недоступен.

# Windows 10/11, Linux

## Hiddify Next

1. **Установите последний релиз для своей ОС.**

	![Hiddify Next Github](/install-guide/hiddify-github-pc.png)

    **Скачать:** {{< rawhtml >}}
<a  href="https://github.com/hiddify/hiddify-next/releases" target="_blank" title="GitHub">GitHub</a>
{{< /rawhtml >}}
	> Для Windows рекомендуем версию **Portable** (достаточно распаковать и запустить) или **Setup** (с установкой).   

2. **Запускаете программу согласно своей ОС. На Windows это `Hiddify.exe`**

	>**Важно!** Запускайте ***с правами администратора*** *(потребуются для режима VPN)*.

	![Hiddify-1](/install-guide/hiddify-1.png)
	
	**Регион**:
	Для РФ рекомендуем выбрать регион "Россия", во всех остальных случаях "Другой".
	> **При выборе региона "Россия" доступ ко всем .RU и .РФ сайтам, сервисам VK и Yandex будет "напрямую"(без VPN).**  
	Поэтому для проверки локации не используйте 2ip.ru.
	
	>***Сбор аналитики***: рекомендуем отключить.
	
3.	**Копируете подписку и нажимаете "Новый профиль" на открывшемся экране. Далее "Добавить профиль из буфера обмена".**

	![Hiddify-1](/install-guide/hiddify-2.gif)
	
	
4.  **В правом в верхнем углу нажимаете на иконку "Настройки" и выбираете режим "VPN".**

	>Если вам нужен VPN только для браузера, то можете оставить его в «Системном прокси».

	![Hiddify-4](/install-guide/hiddify-3.png)

5. **Подключаетесь, переходите на вкладку ***Прокси*** и ***Выбираете сервер***.**
	
	>Если у вас возникают проблемы с подключением, то необходимо:
	Перейти во вкладку **Параметры конфигурации**, найти пункт **Прямой DNS** и изменить его на:
	
	>>***https://8.8.8.8/dns-query***

	>Смена сервера может занимать до 10 секунд.
	
	>Рекомендуется проверить задержку серверов повторно, нажав на иконку Молнии справа внизу. Hiddify всегда "завышает" задержку в разы и даже может показать что сервер недоступен, хотя это не так.

	![Hiddify-5](/install-guide/hiddify-4.png)

-------------

## NekoRay
1. **Установите последний релиз для своей ОС.**

	![NekoRay Github](/install-guide/nekoray-github.png)

    **Скачать:** {{< rawhtml >}}
<a  href="https://github.com/Mahdi-zarei/nekoray/releases" target="_blank" title="GitHub">GitHub</a><br><br>
{{< /rawhtml >}}

2. **Запускаете программу согласно своей ОС. На Windows это `nekoray.exe` c иконкой "кошки в коробке".**

	>**Важно!** Запускайте ***с правами администратора*** *(потребуются для режима VPN)*.

3. **После запуска необходимо подкорректировать настройки** *(для устранения утечки DNS)*.  
	Для этого выбираете в меню "Настройки" -> "Настройки TUN-режима". В открывшемся окне необходимо поставить галочку "Strict Route" и нажать OK.

	>В случае, если подключиться в конце не удастся, то попробуйте убрать эту галочку и попробуйте подключиться снова.
	
	![NekoRay-1](/install-guide/nekoray-1.gif)
	
4.	**Копируете подписку и выбираете в меню "Программа" -> "Добавить профиль из буфера обмена". В открывшемся окне выбираете "Как подписку (добавить новую группу)" и нажимаете OK. Далее "Настройки" -> Группы и удаляете группу по умолчанию.**

	![NekoRay-2](/install-guide/nekoray-2-1.gif)
	
5.  **Выбираете в меню "Программа" -> "Запомнить последний профиль". Далее обязательно ставите галочку "Режим TUN" в правом верхнем углу, затем выбираете сервер, "ПКМ" -> "Запустить".**

	>Если вам нужен VPN только для браузера, то можете выбрать режим в «Системный прокси».

	![NekoRay-2](/install-guide/nekoray-3.gif)

-------------

# iOS/Mac

-------------

## Streisand

**Скачать:** {{< rawhtml >}}
<a  href="https://apps.apple.com/ru/app/streisand/id6450534064" target="_blank" title="App Store">App Store</a>
{{< /rawhtml >}}

Копируете полученную подписку и далее по инструкции:

![Streisand](/install-guide/streisand.png)

*Для обновления существующей подписки необходимо сделать долгий тап по "Subscription", внутри будет кнопка "Обновить".*

-------------

## Shadowrocket [249 ₽]

**Купить:** {{< rawhtml >}}
<a  href="https://apps.apple.com/ru/app/shadowrocket/id932747118" target="_blank" title="App Store">App Store</a>
{{< /rawhtml >}}

Копируете полученную подписку и далее по инструкции:

![Shadowrocket](/install-guide/shadowrocket.png)

-------------

## V2Box

**Скачать:** {{< rawhtml >}}
<a  href="https://apps.apple.com/ru/app/v2box-v2ray-client/id6446814690" target="_blank" title="App Store">App Store</a>
{{< /rawhtml >}}

Копируете полученную подписку и далее по инструкции:

![v2box](/install-guide/v2box.png)

-------------

# Android

-------------

## v2rayNG

**Скачать:** {{< rawhtml >}}
<a  href="https://play.google.com/store/apps/details?id=com.v2ray.ang" target="_blank" title="Play Store">Play Store</a>
{{< /rawhtml >}}

Копируете полученную подписку и далее по инструкции:

![v2rayNG](/install-guide/v2rayNG.png)

--------------

## Hiddify

**Скачать:** {{< rawhtml >}}
<a  href="https://github.com/hiddify/hiddify-next/releases/tag/v2.0.5" target="_blank" title="GitHub">GitHub</a>
{{< /rawhtml >}}(APK Universal)

>**Не устанавливайте версию из Play Маркет! В данный момент она не работает.**  

**Регион**: Для РФ рекомендуем выбрать регион "Россия", во всех остальных случаях "Другой".
	> **При выборе региона "Россия" доступ ко всем .RU и .РФ сайтам, сервисам VK и Yandex будет "напрямую"(без VPN).**  
	Поэтому для проверки локации не используйте 2ip.ru.  
	
	>Далее копируете полученную подписку и добавляете как показано ниже. После добавления переключитесь на вкладку "Прокси" и выберите желаемую локацию.  
	Если у вас возникают проблемы с подключением, то необходимо:
	Перейти в меню **Параметры конфигурации**, найти пункт **Прямой DNS** и изменить его на:
	
	>>***https://8.8.8.8/dns-query***

![Hiddify](/install-guide/hiddify-android.png)

--------------

# Обновление подписки

## Hiddify

![Hiddify](/install-guide/hiddify-update.png)

## NekoRay

![NekoRay](/install-guide/nekoray-update.png)

## Streisand 

![Streisand](/install-guide/streisand-update.png)

## V2Box

![V2box](/install-guide/v2box-update.png)

## v2rayNG

![V2rayNG](/install-guide/v2rayng-update.png)

{{< rawhtml >}}<center><b>Все готово!</b></center>{{< /rawhtml >}}