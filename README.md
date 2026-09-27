# MojoTutorials
> _Официальная статья_

MojoLauncher это Лаунчер, основанный на [PojavLauncher](https://github.com/PojavLauncherTeam/PojavLauncher), позволяющий играть в Minecraft: Java Edition на устройствах Android!\
На этой странице вы найдёте различные руководства, которые помогут вам с удовольствием играть в Minecraft через Mojo
- [Гитхаб моджо](https://github.com/MojoLauncher)
- [Дискорд сервер](https://discord.gg/pojavlauncher-sng-962263126647144449)
- [Телеграм канал](https://t.me/mojolauncher)
- [Телеграм группа](https://t.me/mojolauncher_chat)
- [Моджо в Google Play](https://play.google.com/store/apps/details?id=git.artdeell.mojo)
- [MJLauncher?](https://t.me/MJLauncher)
## Оглавление
1. [Как ставить моды?](#1-как-ставить-моды) (а так же "[Зависимости модов](#зависимости-модов)", "[Как определить нужный инстанс?](#как-определить-нужный-инстанс)" и "[Что такое latestlog.txt?](#что-такое-latestlogtxt-и-где-мне-его-найти)")
2. Как ставить ресурс паки?
3. Как поставить карту/мир?
4. Как ставить шейдеры?
5. Как поставить плагин Angle?
6. Как поставить скин?
7. Как поставить сборку?
## 1. Как ставить моды?
Создайте новый профиль с нужной версией и загрузчиком модов. __Запустите его__. Это нужно для того, чтобы нужные папки сами создались  
<img width="500" alt="image" src="https://github.com/user-attachments/assets/4c6fa181-20bb-4fc4-aa56-665c26c3f26b" />  

Скачайте мод, который вам нужен (желательно с [Modrinth'a](https://modrinth.com/) или [CurseForge'a](https://www.curseforge.com/minecraft))  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/d8f66df3-100c-472f-8419-7fa371ef5a78" />  

Убедитесь, что версия Майнкрафта с загрузчиком модов, которые вы запускаете, совпадают с модом  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/411b15e2-1901-4244-9fcf-e4f17473eea3" />  

Зайдите в Лаунчер и откройте папку игры через встроенный проводник  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/7645c354-5784-4a7f-b9e3-c7b58e763a5f" />  

В загрузках будет ваш мод (чтобы перейти в загрузки: нажмите на три полоски сверху-слева и «Загрузки») 
<img width="250" alt="image" src="https://github.com/user-attachments/assets/3dafacf2-c1b1-4cdc-a1d9-11d76daba684" />  

Выделите его и нажмите на три точки сверху-справа. Нажмите «Копировать в...»  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/bbf30f21-2d44-4450-86d2-1085758e7b74" />  

Нажмите на три полоски вверху-слева и выберите MojoLauncher (либо путь Android/data/git.artdeell.mojo/files)  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/f5eb6777-3e65-4119-93ec-6f84883a6a1c" />  

«instances»  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/65c7850c-27c3-4b40-9a37-d039db276627" />  

Выбираете вашу версию (Как определить нужный инстанс?)  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/6cfd2640-065b-42d7-8b55-527a7579552b" />  

«mods» (папка появляется при первом запуске игры)  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/d50433ac-bc1a-4d0e-af4e-0adae0837b2e" />  

Нажимаете «Копировать»  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/92b2a494-7bab-471e-8ba2-6c370e067a37" />  

Если вы используете Fabric, то рекомендуется скачать [Mod Menu](https://modrinth.com/mod/modmenu) для меню модов
## Зависимости модов
Зависимости модов - это необходимые для работы модов файлы (обычно другие моды-библиотеки), без которых основной мод либо не запустится, либо будет работать некорректно\
Часто, именно недокачанные зависимости становятся причиной краша и ошибок игры. Основные способы их обнаружить на примере мода Veinminer:
1. Описание модов

Обычно в описании мода указаны все требования для его работы, поэтому старайтесь всегда читать его перед установкой.  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/12bffe4a-b9f1-4d41-bfde-54cba179ab23" />  
 2. latestlog.txt  
После неудачного запуска Майнкрафта откройте latestlog.txt ([Где найти latestlog?](#что-такое-latestlogtxt-и-где-мне-его-найти)). Найдите строки:
```
A potential solution has been determined, this may resolve your problem:
  - Install silk-core, any version.
More details:
  - Mod 'Veinminer' (veinminer) 2.5.0 requires any version of silk-core, which is missing!
  
Перевод:

Возможное решение найдено, оно может решить вашу проблему:
  - Установите silk-core, любую версию.
Подробнее:
  - Мод 'Veinminer' (veinminer) 2.5.0 требует любую версию silk-core, которая отсутствует!
```
- __Veinminer__ - основной мод
- __silk-core__ - зависимость к основному моду
3. Другие способы обнаружения  
На Модринте рядом с кнопкой «Download» будет ещё одна кнопка. Нажмите на неё и пролистайте немного вниз. Там и будут зависимости  
<img width="500" alt="image" src="https://github.com/user-attachments/assets/83e4c081-947f-4245-bc31-320dbc181a5b" />

На КурсФордже нажмите на файл и пролистайте вниз. Нажмите на «Related Projects». Там и будут зависимости  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/b03a9b0d-67fc-414d-bd80-e3d0744b7ab7" />
## Как определить нужный инстанс?
1. [Если у вас Forge](#если-у-вас-forge)
2. [Если у вас Fabric](#если-у-вас-fabric)
3. [Если у вас NeoForge](#если-у-вас-neoforge)
4. [Если у вас сборка](#если-у-вас-сборка)
### Если у вас Forge
Если у вас Фордж, то название папки будет примерно такое:  
`1.20-46.0.14-382fb79b-bda9-4e16-bb7a-7f5c37152d38`  
- __1.20__ - версия Майнкрафта
- __46.0.14__ - версия Форджа
- __382fb79b-bda9-4e16-bb7a-7f5c37152d38__ - уникальный идентификатор
Сравнивайте название папки со своим профилем (уник. идентификатор сравнивать не нужно!)  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/83e659e3-86b3-4e5b-9e45-5474eef879d6" />

### Если у вас Fabric
Если у вас Фабрик, то название папки будет примерно такое:  
`fabric-loader-0.18.4-1.21.11-a99061de-3cc0-49c6-bdfc-c7e405df9312`  
- __fabric-loader__ - загрузчик модов  
- __0.18.4__ - версия Фабрика
- __1.21.11__ - версия Майнкрафта
- __a99061de-3cc0-49c6-bdfc-c7e405df9312__ - уникальный идентификатор
Сравнивайте название папки со своим профилем (уник. идентификатор сравнивать не нужно!)  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/aef41403-e1b2-4c9c-883f-04eafd0a9e5a" />

### Если у вас NeoForge
Если у вас НеоФордж, то название папки будет примерно такое:  
`20.6.139-b30598be-a804-4df2-bc21-2c29640fc416`  
- __20.6__ - версия Майнкрафта (например: версия 1.21.4 будет 21.4 и т.д.)
- __139__ - версия НеоФорджа
- __b30598be-a804-4df2-bc21-2c29640fc416__ - уникальный идентификатор
Сравнивайте название папки со своим профилем (уник. идентификатор сравнивать не нужно!)  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/aba37d08-c4a8-482c-9423-16e49e7aafc2" />

### Если у вас сборка
Если у вас сборка модов, скачанная с Лаунчера, то проблем возникнуть не должно, так как в названии папки есть название самой сборки. Например SimplyOptimized   будет называться:  
`simply_optimized-ec2d77b7-1861-4519-80e1-219f40566191`  
- __simply_optimized__ - название сборки
- __ec2d77b7-1861-4519-80e1-219f40566191__ - уникальный идентификатор
### Что такое latestlog.txt и где мне его найти?
__Latestlog.txt__ - журнал, записывающий историю запуска Minecraft, по которому, в случае вылета или ошибки, можно определить причину вылета/ошибки.
Просьба не путать с latest.log и подобными, в них меньше информации!  
В MojoLauncher найти его можно в корневом каталоге, однако для вашего удобства, лучше всего использовать кнопку "Поделиться журналом" в меню самого Mojo!  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/003a0109-a8ac-410b-8ae3-93442bb7e9e1" />  

Поздравляю! Вы поставили мод.
> _[Вернуться к оглавлению](#оглавление)_






