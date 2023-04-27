# Заблоковані на мережі провайдера "УКРКОМ" ресурси, станом на четвер, 27 квітня 2023 09:40:49 +0300.
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

Наприклад, маємо AS20870

<pre>~$ whois -r AS20870
% This is the RIPE Database query service.
% The objects are in RPSL format.
%
% The RIPE Database is subject to Terms and Conditions.
% See http://www.ripe.net/db/support/db-terms-conditions.pdf

% Note: this output has been filtered.
%       To receive output for a database update, use the "-B" flag.

% Information related to 'AS20859 - AS20927'

as-block:       AS20859 - AS20927
descr:          RIPE NCC ASN block
remarks:        These AS Numbers are assigned to network operators in the RIPE NCC service region.
mnt-by:         RIPE-NCC-HM-MNT
created:        2018-11-22T15:27:27Z
last-modified:  2018-11-22T15:27:27Z
source:         RIPE

% Information related to 'AS20870'

% Abuse contact for 'AS20870' is 'abuse@ttk.ru'

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
source:         RIPE

% This query was served by the RIPE Database Query Service version 1.106.1 (ABERDEEN)</pre>


## <b>domains.list</b> - список доменів які блокуються на рівні DNS, рекурсивними серверами. 

Список заблокованих , за відповідними розпорядженнями, доменних імен, на
рекурсивних серверах провайдера. Окрім наведених у списку доменів, 
рекурсивними серверами блокуються також домени, що містять посилання на
yandex, kaspersky, drweb, dr-web, webmoney, odnoklassniki, sharij, strana
та wildberries.

## <b>fraud.list</b> - список доменів Response Policy Zones для fraud-rpz.ua.db, що блокуються на рівні DNS, на виконання Розпорядження НЦУ №67/850.

В списку наведено доменні імена, які блокуються за технологією rpz для
зони fraud-rpz.ua.db.
Наведено останній знятий зріз, станом на четвер, 27 квітня 2023 09:40:49 +0300.
Актуальний поточний стан можна подивитися лише й виключно на ресурсі
ведення зони fraud-rpz.ua.db.
