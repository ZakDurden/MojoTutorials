# MojoTutorials
> _Официальная статья_

MojoLauncher это лаунчер, основанный на [PojavLauncher](https://github.com/PojavLauncherTeam/PojavLauncher), позволяющий играть в Minecraft: Java Edition на устройствах Android!  
На этой странице вы найдёте различные руководства, которые помогут вам с удовольствием играть в Minecraft через Mojo
- [Гитхаб моджо](https://github.com/MojoLauncher)
- [Дискорд сервер](https://discord.gg/pojavlauncher-sng-962263126647144449)
- [Телеграм канал](https://t.me/mojolauncher)
- [Телеграм группа](https://t.me/mojolauncher_chat)
- [Моджо в Google Play](https://play.google.com/store/apps/details?id=git.artdeell.mjlaunch)
- [MJLauncher?](https://t.me/MJLauncher)

## Оглавление
1. [Как ставить моды?](#1-как-ставить-моды) (а так же "[Зависимости модов](#зависимости-модов)", "[Как определить нужный инстанс?](#как-определить-нужный-инстанс)" и "[Что такое latestlog.txt?](#что-такое-latestlogtxt-и-где-мне-его-найти)")
2. [Как ставить ресурс паки?](#2-как-ставить-ресурс-паки)
3. [Как поставить карту/мир?](#3-как-поставить-картумир)
4. [Как ставить шейдеры?](#4-как-ставить-шейдеры)
5. [Как поставить плагин Angle?](#5-как-поставить-плагин-angle)
6. [Как поставить скин?](#6-как-поставить-скин)
7. [Как поставить сборку?](#7-как-поставить-сборку)

## 1. Как ставить моды?
Создайте новый профиль с нужной версией и загрузчиком модов. __Запустите его__. Это нужно для того, чтобы нужные папки сами создались  
<img width="500" alt="image" src="https://github.com/user-attachments/assets/4c6fa181-20bb-4fc4-aa56-665c26c3f26b" />  

Скачайте мод, который вам нужен (желательно с [Modrinth'a](https://modrinth.com/) или [CurseForge'a](https://www.curseforge.com/minecraft))  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/d8f66df3-100c-472f-8419-7fa371ef5a78" />  

Убедитесь, что версия Майнкрафта с загрузчиком модов, которые вы запускаете, совпадают с модом  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/411b15e2-1901-4244-9fcf-e4f17473eea3" />  

Зайдите в лаунчер и откройте папку игры через встроенный проводник  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/7645c354-5784-4a7f-b9e3-c7b58e763a5f" />  

В загрузках будет ваш мод (чтобы перейти в загрузки: нажмите на три полоски сверху-слева и «Загрузки») 
<img width="250" alt="image" src="https://github.com/user-attachments/assets/3dafacf2-c1b1-4cdc-a1d9-11d76daba684" />  

Выделите его и нажмите на три точки сверху-справа. Нажмите «Копировать в...»  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/bbf30f21-2d44-4450-86d2-1085758e7b74" />  

Нажмите на три полоски вверху-слева и выберите MojoLauncher (либо путь Android/data/git.artdeell.mojo/files)  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/f5eb6777-3e65-4119-93ec-6f84883a6a1c" />  

«instances»  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/65c7850c-27c3-4b40-9a37-d039db276627" />  

Выбираете вашу версию ([Как определить нужный инстанс?](#как-определить-нужный-инстанс))  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/6cfd2640-065b-42d7-8b55-527a7579552b" />  

«mods» (папка появляется при первом запуске игры)  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/d50433ac-bc1a-4d0e-af4e-0adae0837b2e" />  

Нажимаете «Копировать»  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/92b2a494-7bab-471e-8ba2-6c370e067a37" />  

> Если вы используете Fabric, то рекомендуется скачать [Mod Menu](https://modrinth.com/mod/modmenu) для меню модов

## Зависимости модов
Зависимости модов - это необходимые для работы модов файлы (обычно другие моды-библиотеки), без которых основной мод либо не запустится, либо будет работать некорректно  
Часто, именно недокачанные зависимости становятся причиной краша и ошибок игры. Основные способы их обнаружить на примере мода Veinminer:  

__Описание модов__  
Обычно в описании мода указаны все требования для его работы, поэтому старайтесь всегда читать его перед установкой.  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/12bffe4a-b9f1-4d41-bfde-54cba179ab23" />   

__latestlog.txt__  
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

__Другие способы обнаружения__  
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

## 2. Как ставить ресурс паки?
Скачайте нужный ресурс пак. Разные версии ресурс пака и Майнкрафта не всегда приводят к ошибкам, но рекомендуется чтобы они совпадали  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/ad4082aa-a0f1-4849-a6f8-f3686c7cafba" />  

Зайдите в лаунчер и откройте папку игры через встроенный проводник  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/a94125f0-484f-4474-a978-4fa7a2a74db4" />  

В загрузках будет ваш ресурс пак (чтобы перейти в загрузки нажмите на три полоски сверху-слева и «Загрузки»). Выделите его и нажмите на три точки сверху-справа. Нажмите «Копировать в...»  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/55be49bd-58f0-42bf-80e3-cc698adc558d" />  

Нажмите на три полоски вверху-слева и выберите MojoLauncher (либо путь Android/data/git.artdeell.mojo/files)  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/b26b5a93-fbb6-4768-88d8-28e874c35551" />  

«instances»  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/471f806c-90fe-418c-a194-486b8c75aaec" />  

Выбираете вашу версию ([Как определить нужный инстанс?](#как-определить-нужный-инстанс))  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/099d1c5a-bc1c-4c58-a64b-11144579493c" />  

«resourcepacks» (папка появляется при первом запуске игры)  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/b6908f06-a663-47bf-97e3-5ba69d0f7520" />  

Нажимаете «Копировать»  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/38d3cb66-3859-40e9-8e43-e61446fed2ba" />  

Поздравляю! Вы поставили ресурс пак.
> _[Вернуться к оглавлению](#оглавление)_

## 3. Как поставить карту/мир?
Скачайте нужную карту. Зайдите в Лаунчер и откройте папку игры через встроенный проводник  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/22bb87b9-346a-4449-883f-06c713daacbc" />  

В загрузках будет ваша карта (чтобы перейти в загрузки нажмите на три полоски сверху-слева и «Загрузки»). Она будет сжата в .zip, .rar или другой архив. Нажмите на него  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/34095c28-8a7c-4606-ab6d-ba50ab63c586" />  

Выделите содержимое, нажмите на три точки сверху-справа и «Извлечь»  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/f16f3752-f22b-4f74-bf54-757c32e8d54b" />  

Нажмите на три полоски вверху-слева и выберите MojoLauncher (либо путь Android/data/git.artdeell.mojo/files)  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/6f7106a8-9b5f-43e5-9e7f-fb2e3c1632ea" />  

«instances»  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/80b9a375-f9e6-45a0-9835-4afd5885fe56" />  

Выбираете вашу версию ([Как определить нужный инстанс?](#как-определить-нужный-инстанс))  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/53e3c1ba-ca8f-445b-b8a6-95ba5d438222" />  

«saves» (папка появляется при первом запуске игры)  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/42eec98f-a5ad-42ca-bffc-4288982483e9" />  

Нажимаете «Извлечь»  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/17cf3df3-6c86-49a9-b189-e1672c06ca2b" />  

> Если ваша версия игры новее, чем та, на которой создана карта, то, как правило, проблем не возникает. Однако при запуске карты в более старой версии игры возможны ошибки

Поздравляю! Вы поставили карту.
> _[Вернуться к оглавлению](#оглавление)_

## 4. Как ставить шейдеры?
Для начала убедитесь, что у вас скачана последняя версия Mojo. Далее, перед установкой шейдера необходимо скачать мод, который обеспечивает его работу:  
Для __Fabric__ - это __Iris__ (не забудьте Sodium).  
Для __Forge__ - это __OptiFine__ или __Oculus__ (для второго не забудьте Embedium).  
> Знайте, что работа шейдеров сильно зависит от вашего устройства, поскольку они разрабатываются преимущественно под архитектуру процессоров и видеокарт пк. Из-за этого шейдеры могут работать нестабильно или вовсе не запускаться - и помогать с их запуском вам мало кто будет.

Скачайте нужный шейдер  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/d47e8698-ffd6-4a03-a8d1-a426690e516a" />  

Зайдите в Лаунчер и откройте папку игры через встроенный проводник  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/f863f77b-a222-4f56-971a-6225b1a5088d" />  

В загрузках будет ваш шейдер (чтобы перейти в загрузки нажмите на три полоски сверху-слева и «Загрузки»). Выделите его и нажмите на три точки сверху-справа. Нажмите «Копировать в...»  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/868f8938-d4ae-48b3-a475-41368ea0c2f2" />  

Нажмите на три полоски вверху-слева и выберите MojoLauncher (либо путь Android/data/git.artdeell.mojo/files)  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/69d8a009-7d26-411b-a897-4ec0638d807f" />  

«instances»  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/cfceec00-62f3-43b2-8a6f-9269ef154d61" />  

Выбираете вашу версию ([Как определить нужный инстанс?](#как-определить-нужный-инстанс))  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/1fab903a-4f31-44eb-bdc0-27e18290d1be" />  

«shaderpacks» (папка появляется при первом запуске игры с модом Iris/Oculus/Optifine)  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/7a4eba50-bc9b-40d9-a45f-4da30bcbae3c" />  

Нажимаете «Копировать»  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/70b11743-9069-4c8a-b171-c6682ef2755d" />  

Поздравляю! Вы поставили шейдеры.
> _[Вернуться к оглавлению](#оглавление)_

## 5. Как поставить плагин Angle?
Angle плагин для LTW в Mojo. Полезен на кривых gles драйверах  

Скачайте [плагин](https://github.com/MojoLauncher/AnglePlugin/releases/download/) из официального гитхаба  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/7f7c16a9-7957-44fc-b380-b9c7915d6f7d" />  

Иногда может вылезти окно оповещения безопасности Google Play. Нажмите «Подробнее» и «Всё равно установить»  
<img width="500" alt="image" src="https://github.com/user-attachments/assets/bf7a8a6e-d1fd-4aec-ac6a-145efc538cff" />  

После установки самого плагина зайдите в Моджо и в настройки  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/a86f27d2-1303-483d-b0a1-7a47c86ddeb4" />  

«Настройки графики» и включаете «Использовать ANGLE»  
<img width="500" alt="image" src="https://github.com/user-attachments/assets/dd98c087-ecef-41f3-bfc4-1eb5264ae5ff" />  

Поздравляю! Вы поставили Angle плагин.
> _[Вернуться к оглавлению](#оглавление)_

## 6. Как поставить скин?
1. [Если есть лицензия](#если-куплена-лицензия)
2. [Если нет лицензии](#если-лицензии-нет)

### Если куплена лицензия:
Зайдите на [официальный сайт Майнкрафта](http://minecraft.net/)

Войдите в свой аккаунт Майкрософт, на котором куплена игра  
<img width="500" alt="image" src="https://github.com/user-attachments/assets/09849866-99b3-4ab4-82ec-6befe5fbb11b" />  

Загрузите свой скин  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/ef7db12a-f79a-4d21-9640-a7d11042c9df" />    

Зайдите в Майкрософт аккаунт через Моджо  
<img width="500" alt="image" src="https://github.com/user-attachments/assets/3112775e-223e-44bd-a545-47ccd534c2cb" />  

### Если лицензии нет:
Зайдите на сайт [Ely.by](http://ely.by/)  

Выберите «К авторизации», если у вас уже есть аккаунт. Выберите «Регистрация», если впервые зашли на сайт  
<img width="500" alt="image" src="https://github.com/user-attachments/assets/28aa9d63-0c48-4147-9483-2ca02695c276" />  

Когда зашли или создали свой аккаунт в меню выберите «Скины»  
<img width="500" alt="image" src="https://github.com/user-attachments/assets/de759e88-ed47-4369-b3ce-1aba38069762" />  

Выбираете скин из уже существующих на сайте или загружаете свой  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/415980da-980a-4056-a6dd-b205c8705a5d" />  

Зайдите в аккаунт через Моджо  
<img width="500" alt="image" src="https://github.com/user-attachments/assets/12d3abe9-817f-44c9-88f9-ed90310cb141" />  

> Важно отметить, что если сервер, на котором вы играете, не поддерживает скины ely by, то отображаться он не будет

Поздравляю! Вы поставили скин.
> _[Вернуться к оглавлению](#оглавление)_

## 7. Как поставить сборку?
1. [Если сборка из лаунчера](#если-сборка-из-лаунчера)
2. [Если сборка НЕ из лаунчера](#если-сборка-не-из-лаунчера)

### Если сборка из лаунчера
Зайдите в лаунчер. Нажмите на «Создать новую установку» и «Установка со сборкой модов»  
<img width="500" alt="image" src="https://github.com/user-attachments/assets/1ac818d3-1f49-4648-a831-e0e860823c45" />  

Ищите нужную сборку. Нажмите на нее, выберите нужную версию и установите  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/17566fbc-dfaa-4719-b716-57ec0bafafc9" />  

### Если сборка НЕ из лаунчера
Если вы скачали сборку с форматом .mrpack или .zip архива CurseForge, то зайдите в лаунчер, нажмите на "Создать новую установку" и "Установка со сборкой модов"  
<img width="500" alt="image" src="https://github.com/user-attachments/assets/f3763794-6d95-4298-af3d-c86acbddeaa6" />  

Нажимаете на "Импорт локальной сборки", выбираете свою скачанную сборку и готово  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/a628c4ae-5088-48f9-9a81-46d67bcaaf99" />  

Если вы скачали сборку в формате обычного .zip или .rar архива, то создайте установку с версией и загрузчиком модов как в сборке
<img width="500" alt="image" src="https://github.com/user-attachments/assets/5617b082-8fc2-482b-9d6a-541f0e6a3b23" />  

Найдите свою сборку. Если вы скачали её с браузера, то она будет загрузках. Если вы скачали её с Телеграма, то ищите в download→telegram. Нажмите на неё
<img width="250" alt="image" src="https://github.com/user-attachments/assets/0686d68c-a3dd-4d55-a5a2-d80242f890a1" />  

Выделите все файлы в архиве. Нажмите на три точки в верхнем-правом углу и «Извлечь».  
> (Если архив без папок и в нем только моды, то выделяйте их и извлекайте в папку «mods»)
<img width="250" alt="image" src="https://github.com/user-attachments/assets/3324b24c-1c50-441f-8be3-973df1061ef2" />  

Нажмите на три точки вверху-слева и выберите MojoLauncher (либо путь Android/data/git.artdeell.mojo/files)  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/91c36f43-7d11-48f6-bbb2-a822a508c60e" />  

«instances»  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/9aa5f3b2-4dd1-4baf-8049-1baba42683df" />  

Выбираете вашу версию ([Как определить нужный инстанс?](#как-определить-нужный-инстанс)). Убедитесь, что версия и загрузчик модов сборки совпадают с вашей запускаемой версией  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/3a3592ea-029b-4155-ab4b-add9656805ca" />  

Если в вашей версии уже есть папки, то их надо удалить. «Извлечь»  
<img width="250" alt="image" src="https://github.com/user-attachments/assets/164f3f1f-2e9e-4952-971e-f69bce5adf37" />  

Поздравляю! Вы поставили сборку.
> _[Вернуться к оглавлению](#оглавление)_
