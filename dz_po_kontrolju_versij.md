# <p align="center" style='color:green'>Краткий гайд по использованию Git</p>
## <p align="center">Материалы</p>

Для того чтобы использовать Git максимально эффективно нам потребуется воспользоваться следующими материалами:

1. <p><a href="https://git-scm.com/book/ru/v2">Книга по использованию Git</a></p> 
<p><img src="1.jpg"></p>

2. <p><a href="https://gb.ru/courses/1117">Бесплатный курс от GB по использованию Git</a></p>
<p><img src="2.jpg"></p> 

## <p align="center">Как начать работать?</p>

* Скачиваем Git
* Скачиваем Visualstudio

### <p style='color:red'> Важно!!!</p>

Перед началом работы нам требуется «представиться» системе контроля версий. Это нужно сделать всего один раз, и git запомнит вас. Для этого нужно ввести в терминале 2 команды:
1. `git config --global user.name «Ваше имя англ буквами»`
2. `git config --global user.email ваша_почта@example.com`

## <p align="center">Основные команды</p>

<p align="center">
<body>
  <table border="1">
   <tr>
     <td>Начало команды</td>
     <td>Конец команды</td>
     <td>Значение команды</td>
   </tr>
   <tr>
     <td>git</td>
     <td>add "Название файла"</td>
     <td>Сохраняет/добавляет наш файл</td>
  </tr>
  <tr>
     <td>git</td>
     <td>log</td>
     <td>Выводит журнал изменений </td>
  </tr>
  <tr>
     <td>git</td>
     <td>commit -m " "</td>
     <td>Сохраняет изменения </td>
  </tr>
  <tr>
     <td>git</td>
     <td>checkout</td>
     <td>Команда для возврата к прошлому сохранению</td>
  </tr>
  <tr>
     <td>git</td>
     <td>checkout master</td>
     <td>Возврат к актуальному состоянию</td>
  </tr>
   <tr>
     <td>git</td>
     <td>diff</td>
     <td>Показывает разницу между текущим файлом и сохраненным</td>
  </tr>
    <tr>
     <td>git</td>
     <td>init</td>
     <td>Инициализация</td>
  </tr>
    <tr>
     <td>git</td>
     <td>status</td>
     <td>Показывает сохранен наш файл или нет</td>
    </tr>
 </table>
 </body>
</p>

## <p align="center">**Отдельные замечания**</p>

При работе с Git у нас могут возникнуть некоторые сложности, но все они решаемы!

Для того чтобы облегчить нашу работу можно пользоваться следующими "Лайфхаками":

1. Постоянно сохранять прогресс, для этого требуется нажимать сочетание клавиш ctrl+S, после того как мы замечаем белый кружок около названия нашего файла.
2. Работу в Visualstudio можно облегчить. Для этого когда вы пишите команды в терминале, особенно если это название файлов можно и нужно использовать tab. Благодаря этому название файла/команды будет дописываться автоматически. 
3. Бывают случаи, когда терминал говорит нам о том что он закончил работу (надпись end на белом фоне), чтобы не перезагружать/выключать терминал можно просто нажать на букву Q в английской раскладке.
4. Для упрощения работы с терминалом следует использовать стрелочки вверх/вниз для того чтобы не набирать команды каждый раз заново.

В заключение хотелось бы привести цитату великого человека Натана Ротшильда:

**<p align="center"> «Кто владеет информацией - тот владеет миром»</p>**

## <p align="center">Продолжение работы с системой Git</p>

Разбираемые следующие вопросы:
1. Как создать новую ветку?
2. Как создать игнорирование файлов?
3. Что делать в случаях конфликта версий?

**<p align="center"> Создание новых веток</p>**

Для создания новых веток в программе Git требуется произвести пару простых действий:

* Первым действием нам требуется ввести команду git branch для того чтобы ухнать в какой ветке мы работаем ( наша ветка будет помечана *)
* После этого воспользуемся командой git branch #### (где # это название нашей новой ветки) с помощью данной команды можно создать новую ветку
* После создания новой ветки нам надо начать в ней работу, для этого воспользуемся командой git checkout #### (где # это название нашей новой ветки), данная команда позволяет переходить с одной ветки на другую

**<p align="center"> Создание игнорирования файлов</p>**

Для того чтобы git игнорировал некоторые файлы, например такие как картинки нам потребуется сдеть одно простое действие.

Создаем файл с названием .gitignore и в этом файле записываем название файлов которые требуется игнорировать.

**<p align="center"> Разрешения конфликта версий</p>** 

Во время сливания нескольких веток в одну у нас может возникнуть конфликт версий который требуется разрешить.

Если происходит конфликт версий нам требуется выбрать одно изменение, другое изменение или же оставить и одно изменение и другое изменение, а потом в ручную вносить правки.

## <p align="center">Сливание и удаление веток</p>

Для того чтобы начать сливание веток нам потребуется перейти в ветку master(или же в другую ветку в которой мы хотим произвести сливание) и начать сливание с мопощью следующей команды:

git merche #### (где # это название ветки) - сливание веток

Если нам требуется удалить ветку, то требуется воспользоваться следующей командой:

git branch -d #### (где # это название ветки) - удаление веток

accept current change - оставить текущую версию

accept incoming change - оставить новую версию

accept both changes - оставить оба варианта

compare changes - сравнить варианты

## <p align="center">Начало третьего задания</p> 

GitHub- сервис, много полезных функций, огромный архив кода.

Git-программа.

Code позволяет нам увидить строку с адресом

Cd #### (где # это название папки)- поменять дерикторий

Как загрузить наш репозиторий в интернет?

Создаем репозиторий (git init), создаем файл, сохраняем его.

Нажимаем +, выбираем новый репозиторий, называем его и создаем его (зеленая кнопка).

git remote add origin адрес - добавление удаленного репозитория, связывает локальный репозиторий с удаленным

git branch -M main -какая ветка является основной

git push -u origin main - отправляет все что мы сделали в интернет 

git push- отправляет локальную копию в интернет
