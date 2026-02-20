
Скрипт установки [Passwall](https://github.com/amirhosseinchoghaei/Passwall) для OpenWRT, выбирать PasswallV2

## Настройка
1. Во вкладке Rule Manage, указать
  GeoIP Update URL - https://cdn.jsdelivr.net/gh/hydraponique/roscomvpn-geoip@release/geoip.dat
  Geosite Update URL - https://cdn.jsdelivr.net/gh/hydraponique/roscomvpn-geosite@release/geosite.dat
![Шаг 2_2](https://raw.githubusercontent.com/kireevm96/passwiki/refs/heads/main/2_2.png)
  и запустить Manually update

2. Добавим правила для машрутизации в блок Sing-Box/Xray Shunt Rule 
  - [DEFAULT.JSON от hydraponique](https://github.com/hydraponique/roscomvpn-routing/blob/main/HAPP/DEFAULT.JSON)
  - Требуеться создать 3 правила Direct, Proxy, Block
![Шаг 2_3](https://raw.githubusercontent.com/kireevm96/passwiki/refs/heads/main/2_3.png)
  - Заполнить каждое правило по примеру DEFAULT.JSON
![Шаг 3](3.png)

3. Добавим подписку во вкладке Node Subscribe, и запустим сихронизацию кнопкой Manual subscription
![Шаг 4](4.png)

![Шаг 5](5.png)

![Шаг 6](6.png)

4. Добавим Xray Balancing, он нужен для балансировки и в случае недоступности одного из узлов.
![Настройка 1](7.png)

![Настройка 4](10.png)

![Настройка 5](11.png)

2. Добавим Xray Shunt, он требуеться для работы списков машрутизации, и сразу применим правила.
![Настройка 2](8.png)

![Настройка 6](12.png)

- Не забыть указать, сотвествие куда какой трафик машрутизировать

![Настройка 7](13.png)

8. Переходим Basic Settings, и выбираем наш Xray Shunt и включаем Main switch
![Настройка 8](14.png)


Скрипт установки [Passwall](https://github.com/amirhosseinchoghaei/Passwall) для OpenWRT, выбирать PasswallV2

## Настройка
1. Во вкладке **Rule Manage**, указать
   **GeoIP Update URL** - https://cdn.jsdelivr.net/gh/hydraponique/roscomvpn-geoip@release/geoip.dat
   **Geosite Update URL** - https://cdn.jsdelivr.net/gh/hydraponique/roscomvpn-geosite@release/geosite.dat
![Шаг 2_2](https://raw.githubusercontent.com/kireevm96/passwiki/refs/heads/main/2_2.png)
   и запустить **Manually update**

2. Добавим правила для машрутизации в блок **Sing-Box/Xray Shunt Rule** 
    [DEFAULT.JSON от hydraponique](https://github.com/hydraponique/roscomvpn-routing/blob/main/HAPP/DEFAULT.JSON)
  Требуется создать 3 правила **Direct**, **Proxy**, **Block**
![Шаг 2_3](https://raw.githubusercontent.com/kireevm96/passwiki/refs/heads/main/2_3.png)
  Заполнить каждое правило по примеру **DEFAULT.JSON**
![Шаг 3](https://raw.githubusercontent.com/kireevm96/passwiki/refs/heads/main/3.png)

4. Добавим подписку во вкладке **Node Subscribe**, и запустим сихронизацию кнопкой **Manual subscription**
![Шаг 4](https://raw.githubusercontent.com/kireevm96/passwiki/refs/heads/main/4.png)

![Шаг 5](https://raw.githubusercontent.com/kireevm96/passwiki/refs/heads/main/5.png)

![Шаг 6](https://raw.githubusercontent.com/kireevm96/passwiki/refs/heads/main/6.png)

4. Добавим **Xray Balancing**, он нужен для балансировки и в случае недоступности одного из узлов.
![Настройка 1](https://raw.githubusercontent.com/kireevm96/passwiki/refs/heads/main/7.png)

![Настройка 4](https://raw.githubusercontent.com/kireevm96/passwiki/refs/heads/main/10.png)

![Настройка 5](https://raw.githubusercontent.com/kireevm96/passwiki/refs/heads/main/11.png)

2. Добавим **Xray Shunt**, он требуется для работы списков маршрутизации, и сразу применим правила**.!!! Без него не будет работать маршрутизация!!!** 
![Настройка 2](https://raw.githubusercontent.com/kireevm96/passwiki/refs/heads/main/8.png)

![Настройка 6](https://raw.githubusercontent.com/kireevm96/passwiki/refs/heads/main/12.png)

Не забыть указать, соответствие куда какой трафик маршрутизировать

![Настройка 7](https://raw.githubusercontent.com/kireevm96/passwiki/refs/heads/main/13.png)

8. Переходим **Basic Settings**, и выбираем наш **Xray Shunt** и включаем **Main switch**
![Настройка 8](https://raw.githubusercontent.com/kireevm96/passwiki/refs/heads/main/14.png)


