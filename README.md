# Заблоковані на мережі провайдера "УКРКОМ" ресурси, станом на четвер, 27 квітня 2023 09:43:19 +0300.
Список ресурсів, які заблоковано в на мережі провайдера "УКРКОМ" (AS12593).

## <b>AS.list</b> - список ворожих автономних систем, анонси яких не приймаються.

Сюди включено учасників наборів AS-MAILRU, AS-VKONTAKTE, AS-YANDEX та
AS-M100. Окрім того, містить автономні системи що супроводжуються
YANDEX-MNT, KL-MNT, MNT-QRATOR-LIR, MNT-NETBRIDGE, VKONTAKTE-NET-MNT та
MNT-M100. Додаються також автономні системи які “випадково” змінили
дислокацію (наприклад, були Yandex Cloud, а стали якимось маловідомим
провайдером в Мухосранську терористичної федерації).

## <b>networks.list</b> - cписок мереж, трафік до яких блокується на транзиті.

В цьому списку представлено мережі, які однозначно відносяться до списку
автономних систем, що наведено вище, і визначаються у whois ключами _-K
-r -i origin_.

Наприклад, маємо AS20870 (KAVKAZ-TRANSTELECOM-AS):

<pre><b>~$ whois -r AS20870</b>
as-block:       AS20859 - AS20927
descr:          RIPE NCC ASN block
remarks:        These AS Numbers are assigned to network operators in the RIPE NCC service region.
mnt-by:         RIPE-NCC-HM-MNT
created:        2018-11-22T15:27:27Z
last-modified:  2018-11-22T15:27:27Z
source:         RIPE

aut-num:        AS20870
as-name:        KAVKAZ-TRANSTELECOM-AS
org:            ORG-CJSC19-RIPE
admin-c:        SKS15-RIPE
tech-c:         SKS15-RIPE
status:         ASSIGNED
mnt-by:         RIPE-NCC-END-MNT
mnt-by:         TRANSTELECOM-MNT
created:        1970-01-01T00:00:00Z
last-modified:  2019-12-04T11:17:25Z
source:         RIPE</pre>

Для цієї AS блокуються наступні мережі:

<pre>~$ whois -K -r -i origin AS20870
route:          80.72.224.0/20
origin:         AS20870

route:          83.69.64.0/19
origin:         AS20870

route:          83.69.65.0/24
origin:         AS20870

route:          89.16.96.0/19
origin:         AS20870

route6:         2a03:5b80::/32
origin:         AS20870</pre>



## <b>domains.list</b> - список доменів які блокуються на рівні DNS, рекурсивними серверами. 

Список заблокованих , за відповідними розпорядженнями, доменних імен, на
рекурсивних серверах провайдера. Окрім наведених у списку доменів, 
рекурсивними серверами блокуються також домени, що містять посилання на
yandex, kaspersky, drweb, dr-web, webmoney, odnoklassniki, sharij, strana
та wildberries.

## <b>fraud.list</b> - список доменів Response Policy Zones для fraud-rpz.ua.db, що блокуються на рівні DNS, на виконання Розпорядження НЦУ №67/850.

В списку наведено доменні імена, які блокуються за технологією rpz для
зони fraud-rpz.ua.db.
Наведено останній знятий зріз, станом на четвер, 27 квітня 2023 09:43:19 +0300.
Актуальний поточний стан можна подивитися лише й виключно на ресурсі
ведення зони fraud-rpz.ua.db.
