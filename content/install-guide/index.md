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

## NekoRay  

1. Установите последний релиз для **своей ОС**. 

> **Скачать:** {{< rawhtml >}}
<a  href="https://github.com/Mahdi-zarei/nekoray/releases" target="_blank" title="GitHub">GitHub</a><br>
{{< /rawhtml >}}

![NekoRay Github](/install-guide/nekoray-github.png)


2. Запускаете программу согласно своей ОС. На Windows это **`nekoray.exe`**

	>**Важно!** Запускайте ***с правами администратора*** *(потребуются для режима VPN)*.

	>**В случае проблем с запуском на Windows, необходимо установить два официальных пакета от Microsoft:**  
	**1:** {{< rawhtml >}}
<a  href="https://learn.microsoft.com/ru-ru/cpp/windows/latest-supported-vc-redist?view=msvc-170#latest-microsoft-visual-c-redistributable-version" target="_blank" title="Распространяемый компонент Visual C++ для Visual Studio 2015-2022">РК Visual C++ для Visual Studio 2015-2022</a>
{{< /rawhtml >}}  
	**2:** {{< rawhtml >}}
<a  href="https://learn.microsoft.com/ru-ru/cpp/windows/latest-supported-vc-redist?view=msvc-170#visual-studio-2013-vc-120--no-longer-supported" target="_blank" title="Распространяемый компонент Visual C++ для Visual Studio 2013">РК Visual C++ для Visual Studio 2013</a><br>
{{< /rawhtml >}}
	
	
3.	Копируете подписку и выбираете в меню **"Программа" -> "Добавить профиль из буфера обмена"**.  
В открывшемся окне выбираете **"Как подписку (добавить новую группу)"** и нажимаете **OK**.  
Далее **"Настройки" -> "Группы"** и удаляете группу **По умолчанию**.

	> **Данные шаги на отображены на GIF ниже:** 

	![NekoRay-2](/install-guide/nekoray-2-1.gif)
	
4.  Обязательно ставите галочку **"Режим TUN"** в правом верхнем углу, затем выбираете сервер, **"ПКМ" -> "Запустить"**.

	>Если вам нужен VPN только для браузера, то можете выбрать режим в **«Системный прокси»**.

	>**Важно!** После отключения необходимо снимать галочку **«Системный прокси»**, иначе **интернета не будет**.

	![NekoRay-3](/install-guide/nekoray-3.gif)  

	>Если у вас возникают проблемы с подключением, то необходимо:
	Перейти в **"Настройки" -> "Настройки маршрутов" -> "DNS"** и изменить **DNS для "прямых" запросов на** на:  
	
	**`9.9.9.9`, если не поможет, то `https://9.9.9.9/dns-query`**


--------


{{< rawhtml >}} <center> {{< /rawhtml >}} 
### Раздельное туннелирование: Whitelist
{{< rawhtml >}} </center> {{< /rawhtml >}}
***Выбранные программы через VPN, все остальное без VPN***  

>**Перед настройкой убедитесь, что VPN работает!**

1.  Открываете **Настройки -> Настройки маршрутов -> вкладка Route**. Нажимаете New.  

	![NekoRay-Whitelist-1](/install-guide/nekoray-whitelist-1.png)  

2.  В открывшемся окне вводите **любое имя профиля**, нажимаете **New**, выбираете *Attribute*: **process_name** и *Outbound*: **proxy**. В окне снизу справа вводите **процессы, который хотите чтобы работали через VPN, по одному на строчке**.

	![NekoRay-Whitelist-2](/install-guide/nekoray-whitelist-2.png)  

3.  Дважды нажимаете **ОК**, и после этого **перезапускаете программу через трей (это важно)**. Далее Открываете **Настройки -> Настройки маршрутов -> вкладка Общие**. Устанавливаете новосозданный профиль в поле **Routing Profile**, ниже **Outbound по-умолчанию** выбираете **direct**.

	![NekoRay-Whitelist-3](/install-guide/nekoray-whitelist-3.png)  


--------
  
{{< rawhtml >}} <center> {{< /rawhtml >}} 
### Раздельное туннелирование: Blacklist    
{{< rawhtml >}} </center> {{< /rawhtml >}}
***Все через VPN, кроме выбранных программ***  

>**Перед настройкой убедитесь, что VPN работает!** 

1.  Открываете **Настройки -> Настройки маршрутов -> вкладка Route**. Нажимаете New.  

	![NekoRay-Whitelist-1](/install-guide/nekoray-whitelist-1.png)  

2.  В открывшемся окне вводите **любое имя профиля**, нажимаете **New**, выбираете *Attribute*: **process_name** и *Outbound*: **direct**. В окне снизу справа вводите **процессы, который хотите чтобы работали без VPN, по одному на строчке**.

	![NekoRay-Whitelist-2](/install-guide/nekoray-blacklist-1.png)  

3.  Дважды нажимаете **ОК**, и после этого **перезапускаете программу через трей (это важно)**. Далее Открываете **Настройки -> Настройки маршрутов -> вкладка Общие**. Устанавливаете новосозданный профиль в поле **Routing Profile**.

	![NekoRay-Whitelist-3](/install-guide/nekoray-blacklist-2.png)  

-------------

## Hiddify Next

1. **Установите последний релиз для своей ОС.**

	![Hiddify Next Github](/install-guide/hiddify-github-pc.png)

    **Скачать:** {{< rawhtml >}}
<a  href="https://github.com/hiddify/hiddify-next/releases" target="_blank" title="GitHub">GitHub</a>
{{< /rawhtml >}}
	> Для Windows рекомендуем версию **Portable** (достаточно распаковать и запустить) или **Setup** (с установкой).   

2. **Запускаете программу согласно своей ОС. На Windows это `Hiddify.exe`**

	>**Важно!** Запускайте ***с правами администратора*** *(потребуются для режима VPN)*.

	>**В случае проблем с запуском на Windows, а также при "Неожиданной ошибке подключения", необходимо установить два пакета от Microsoft:**  
	**1:** {{< rawhtml >}}
<a  href="https://learn.microsoft.com/ru-ru/cpp/windows/latest-supported-vc-redist?view=msvc-170#latest-microsoft-visual-c-redistributable-version" target="_blank" title="Распространяемый компонент Visual C++ для Visual Studio 2015-2022">РК Visual C++ для Visual Studio 2015-2022</a>
{{< /rawhtml >}}  
	**2:** {{< rawhtml >}}
<a  href="https://learn.microsoft.com/ru-ru/cpp/windows/latest-supported-vc-redist?view=msvc-170#visual-studio-2013-vc-120--no-longer-supported" target="_blank" title="Распространяемый компонент Visual C++ для Visual Studio 2013">РК Visual C++ для Visual Studio 2013</a><br>
{{< /rawhtml >}}

	![Hiddify-1](/install-guide/hiddify-1.png)
	
	**Регион**:
	Рекомендуем выбирать регион ***Другой***, но можно оставить и ***Россия***. **При выборе региона "Россия" доступ ко всем .RU и .РФ сайтам, сервисам VK и Yandex будет "напрямую"(без VPN).**
	> **Для корректной работы Discord необходимо выбрать регион "Другой".** 

	> **При выборе региона "Россия" НЕ ИСПОЛЬЗУЙТЕ 2ip.ru ДЛЯ ПРОВЕРКИ ЛОКАЦИИ**
	
	>***Сбор аналитики***: рекомендуем отключить.
	
3.	**Копируете подписку и нажимаете "Новый профиль" на открывшемся экране. Далее "Добавить профиль из буфера обмена".**

	![Hiddify-1](/install-guide/hiddify-2.gif)
	
	
4.  **В правом в верхнем углу нажимаете на иконку "Настройки" и выбираете режим "VPN".**

	>Если вам нужен VPN только для браузера, то можете оставить его в «Системном прокси».

	![Hiddify-4](/install-guide/hiddify-3.png)

5. **Подключаетесь, переходите на вкладку ***Прокси*** и ***Выбираете сервер***.**

	![Hiddify-5](/install-guide/hiddify-4.png)

	>Если у вас возникают проблемы с подключением, то необходимо:
	Перейти во вкладку **Параметры конфигурации**, найти пункт **Прямой DNS** и изменить его на:  
	
	**`9.9.9.9`, если не поможет, то `https://9.9.9.9/dns-query`**
	
	>Смена сервера может занимать до 10 секунд. Также рекомендуется проверить задержку серверов повторно, нажав на иконку Молнии справа внизу. Hiddify всегда "завышает" задержку в разы и даже может показать что сервер недоступен, хотя это не так.


--------

## Другие клиенты

**Invisible Man - XRay**:  
{{< rawhtml >}}
<a  href="https://github.com/InvisibleManVPN/InvisibleMan-XRayClient/releases" target="_blank" title="GitHub">https://github.com/InvisibleManVPN/InvisibleMan-XRayClient/releases</a>
{{< /rawhtml >}}

-------------

# iOS/Mac

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

**Данное приложение устаналивать, только если другие не работают!**  

> Для MacOS существует альтернатива по инструкции Hiddify Next для Win 10/11, только скачиваете пакет DMG.  

**Скачать:** {{< rawhtml >}}
<a  href="https://apps.apple.com/ru/app/v2box-v2ray-client/id6446814690" target="_blank" title="App Store">App Store</a>
{{< /rawhtml >}}

Копируете полученную подписку и далее по инструкции:

![v2box](/install-guide/v2box.png)

-------------

# Android

## Hiddify  

**Скачать:** {{< rawhtml >}}
<a  href="https://github.com/hiddify/hiddify-next/releases/tag/v2.5.7" target="_blank" title="GitHub">GitHub</a>
{{< /rawhtml >}}(APK Universal)  

>**Не устанавливайте версию из Play Маркет! В данный момент версия с Github работает лучше.** 

**Регион**: Для РФ рекомендуем выбрать регион "Россия", во всех остальных случаях "Другой".
> **При выборе региона "Россия" доступ ко всем .RU и .РФ сайтам, сервисам VK и Yandex будет "напрямую"(без VPN).**
Поэтому для проверки локации не используйте 2ip.ru.  

Далее копируете полученную подписку и добавляете как показано ниже. После добавления переключитесь на вкладку "Прокси" и выберите желаемую локацию.  

![Hiddify](/install-guide/hiddify-android.png)

>Если у вас возникают проблемы с подключением, то необходимо:
Перейти во вкладку **Параметры конфигурации**, найти пункт **Прямой DNS** и изменить его на:  
	
**`9.9.9.9`, если не поможет, то `https://9.9.9.9/dns-query`**  

--------------

## v2rayNG

**Скачать:** {{< rawhtml >}}
<a  href="https://play.google.com/store/apps/details?id=com.v2ray.ang" target="_blank" title="Play Store">Play Store</a>
{{< /rawhtml >}}

Копируете полученную подписку и далее по инструкции:

![v2rayNG](/install-guide/v2rayNG.png)

--------------


# Обновление подписки

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

{{< rawhtml >}}<center><b>Все готово!</b></center>{{< /rawhtml >}}