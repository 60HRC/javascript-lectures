# История и основы

### Введение
JavaScript – это интерпретируемый язык программирования с объектноориентированными возможностями. С точки зрения синтаксиса язык Jнапоминает C, C++ и Java, однако это подобие ограничивается синтаксической схожестью. JavaScript – это не типизированный язык, т.е. в нем не требуется определять типы переменных. Объекты в JavaScript отображают имена свойств на произвольные значения. Этим они больше напоминают ассоциативные массивы Perl, чем структуры C или объекты C++ или Java. Механизм объектноориентированного наследования JavaScript скорее похож на механизм прототипов в таких малоизвестных языках, как Self, и сильно отличается от механизма наследования в C++ и Java. Некоторые инструменты JavaScript, например регулярные выражения и средства работы с массивами, реализованы по образу и подобию языка Perl. Ядро языка JavaScript поддерживает работу с такими простыми типами данных, как числа, строки и булевы значения. Помимо этого он обладает встроенной поддержкой массивов, дат и объектов регулярных выражений.

### История создания
JavaScript появился из необходимости сделать веб страницы динамическими. Цель была в создании языка, который веб дизайнеры, люди без большого опыта программирования, могли использовать для добавления анимации или другой активности на свои веб страницы.
В 1995 Web был еще очень молод (HTML 3.2), еще не было такого массового опыта программирования. Java пришла в это же время, но для её использования необходимо было быть профессиональным программистом: написать код на столь мощном языке, скомпилировать его, упаковать в аплет и подключить - все это было непросто сделать. В то время как код на JavaSсript был просто небольшим снипетом, который легко подключить к своей странице или передать кому либо еще - не нужно было изучать целый язык, что бы воспользоваться таким снипетом.

Брэндон Айк разработал JavaScript для Netscape в 90ых, и он был включен в ранние версии Netscape 2 в 1995.
Во время разработки язык то и дело менял названия, были такие варианты как Mocha и LiveScript, и хотя люди
отмечали что язык не был разработан в Sun и он не в точности как Java, Брэндон продолжал продвигать его как младшего брата Java.

Работа над стандартизацией языка началась в ноябре 1996 (ECMA-262), после того как Netscape представила JavaScript в Ecma International. Стандартизованным именем языка стало ECMAScript (*ECMAScript sounds a little like a skin disease. Nobody really wants it.* ©Брэндон Айк), поскольку не удалось договориться с Sun о предоставлении товарного знака - в итоге все уперлось в вопросы маркетинга.
JavaScript было бы идеальным именем стандарта, потому что каждый его так называл. Микрософт не смогла получить лицензию на это имя от Sun, поэтому они назвали свою реализацию JScript. Так вот и сложилась эта забавная ситуация: есть стандарт с забавным названием, и несколько его реализаций с разными торговыми названиями, которые не имеют большой ценности, кроме JavaScript разумеется, которое фигурирует во всех книгах, и о котором постоянно говорят.
Как только ECMAScript был стандартизован, JavaScript стал одним из его диалектов, используемым компанией Netscape.
Другими популярными диалектами стали ActionScript и JScript (используемые в InternetExplorer).
Со временем в каждом диалекте ECMASсript стали появляться собственные пропиетарные теги и свойства (прим.: innerHTML в IE)

Основной точкой преткновения между диалектами стала разработка объектной модели документа (DOM).
Сила JavaScript как клиент-сайд кода была изрядно ограничена отсутсвием вменяемого API манипулирования элементами, поэтому и Microsoft и Netscape начали его разработку независимо, не дожидаясь стандартизации.
Level 0 DOM был реализован в JavaScript для Netscape 2 (даже современные браузеры поддерживают его, несмотря на сомнительную полезность). Microsoft же скопировала его для InternetExplorer.

W3C в 1998 анонсировал рекомендацию для DOM Level 1 и InternetExplorer 5.0 поставлялся с частичной её поддержкой. Это продолжалось до 2000ых, когда рекомендация DOM Level 2 была наконец опубликована и мы получили getElementById и событийную модель, однако было уже слишком поздно - Microsoft к этому времени уже использовал собственную событийную модель в InternetExplorer.
Проблема заключалась в том что начиная с 4ой версии InternetExplorer был интегрирован в Windows из за чего доля рынка Netscape начала страдать. В конце концов стало ясно что стратегия Microsoft была антиконкурентной, что привело к антимонопольному разбирательству в 1998 году. Но даже это не помогло Netscape - InternetExplorer 6 стал доминирующим браузером на рынке.

Развитие стандарта продолжалось витками, так в 1998 был выпущен стандарт ECMAScript 2, а в 1999 ECMAScript 3 (добавлены регулярные выражения, try/catch, улучшена работа со строками, возможность форматировать числа), который является основой современного JavaScript.

В 2001, Дуглас Крокфорд назвал и задокументировал формат JSON (JavaScript Object Notation), основной идее которого было использование синтаксиса JavaScript для хранения данных в текстовом формате. JSON использует JavaScript литералы объектов, массивов, строк, чисел, и логических переменных для представления структурированных данных.
Этот формат стал популярной легковесной альтернативой XML (разумеет этот формат очень легко употреблять при помощи JavaScript)
Например:

```
{
    "first": "John",
    "last": "Doe",
    "married": true,
    "born": 1890,
    "friends": [ "Tarzan", "Cheeta" ]
}
```


Следующее же крупное событие в истории JavaScript произошло в 2005 году. Джеймс Гаррет выпустил статью в которой он ввел термин AJAX и описал набор технологий (в котором, разумеется, JavaSсript была ключевой) для создания приложений desktop класса на базе браузера. Первым впечатляющим результатом применения AJAX стали Google карты, приложение позволяющее рассматривать карту мира, в то время как загружался лишь контент который видим на экране.

Следущее крупное событие в истории JavaScript произошло в 2005 году. В феврале были представлены Google карты, приложение позволяющее в браузере рассматривать карту всего мира, при этом браузер не грузил все данные сразу, а лишь по мере необходимости. Этот результат был достигнут при помощи использования стэка технологий под названием AJAX (Asynchronous JavaScript and XML). Два краугольных камня AJAX - это асинхронная загрузка данных в фоне (при помощи XMLHttoRequest) и динамическое обновление страницы с результатами (via dHTML). Этот подход значительно улучшил юзабилити веб приложений, тем самым приблизив их к приложениям desktop класса.
Это привело к периоду ренессанса в использовании JavaScript. Появилось множество библиотек с открытым исходным кодом: Prototype, jQuery, Dojo и Mootools, а так же многие другие, стал набирать популярность формат JSON.

В июле 2008 было принято решение переименовать ECMAScript 3.1 в ECMAScript 5 и вести язык вперед под псевдонимом Harmony.

Все это приводит нас к сегодняшнему дню в котором JavaScript выходит на совершенно новый виток эволюции, инновации и стандартизации с новыми разработками, такими как Nodejs, позволяющими использовать JavaScript на сервере, и HTML5 API позволяющие управлять пользовательскими медиа, открывать веб-сокеты для интерактивного общения, получать данные о геолокации и т.д.


### Теория
Итак, начнем с начала. В языке программирования группа слов, чисел и операторов, выполняющих специфичную задачу называется утверждением (**statement**)
В JavaScript утверждение может выглядеть например так:

```
a = b * 2;
```

Символы ``a`` и ``b`` здесь являются переменными, а ``2`` - литеральным значением
Символы ``=`` и ``*`` являются операторами - они совершают действия над значениями и переменными.
Большинство утверждений в JavaScript содержат ``;`` в конце (хотя наличие ``;`` в конце утверждения является опциональным, его использование все же помогает избежать ряда проблем).
Таким образом программа является просто набором утверждений, которые описывают шаг за шагом, что нужно сделать для достижения цели.
Утверждения состоят из одного и более выражений. Выражение (**expression**) - это ссылка на переменную или значение, а так же набор переменных и значений, совмещенный с операторами.
Например:

```
a = b * 2;
```

Это утверждение состоит из четырёх выражений:

* ``2`` - это выражение значения-литерала (значения напрямую включенные в код называются литералами (``'string'``, ``"another string"``, ``52``, ``true``, ``false``)
* ``b`` - это выражение переменной, которое говорит "получи текущее значение переменной"
* ``b * 2`` - это арифметическое выражение, которое говорит "выполни умножение"
* ``a = b * 2`` - это выражение присвоения, которое говорит "присвой результат выражения ``b*2`` переменной ``a``"

Отдельно стоящее выражение называют выражением-утверждением (**expression statement**).
Например оно может выглядеть так:

```
b * 2;
```

Само по себе утверждение "получи значение переменной b и умножь его на 2" бесполезно, потому что мы даже не сохраняем результат этих действий. Поэтому чаще всего мы можем увидеть выражения-утверждения в виде вызовов функции:

```
alert( a );
```

Настало время опробовать простенький снипет в деле. Запускаем браузер, открываем инструменты разработчика и
выполняем следующий код:

```
var a = 21;
var b = a * 2;
console.log( b );
```

#### Основные способы ввода/вывода данных

* Вывод: ``console.log``, ``alert``, элементы формы
* Ввод: ``promt``, элементы формы

#### Распространенные операторы:

* математические: ``+``, ``-``, ``*``, ``/``
* присвоение и комбинированное присвоение: ``=``, ``+=``, ``-+``, ``*=``, ``/=``
* инкремент, декремент: ``++``, ``--``
* сравнение: ``==``, ``===``, ``!=``, ``!==``, ``<``, ``>``, ``<=``, ``=>``
* логические и оператор ветвления: ``&&``, ``||``, ``if () {} else {}``
* цикла: ``while () {}``, ``do {} while ()``, ``for () {}``
* комментариев: ``//строчный``, ``/*блочный*/``

#### Определение переменных
Переменная состоит из имени и выделенной области памяти, которая ему соответствует.
Для объявления или, другими словами, создания переменной используется ключевое слово ``var``:

```
var foo; //объявляем переменную
foo = 42; //присваиваем значение переменной
```

Эти данные будут сохранены в соответствующей области памяти и в дальнейшем доступны при обращении по имени.
Для краткости можно совместить объявление переменной и запись данных:

```
var foo = 42;
```

Или объявить за раз сразу несколько переменных:

```
var foo = 42, bar = 'baz';
```

Имя (идентификатор) переменной должено начинаться с буквы, символа ``_`` или символа ``$``. Остальная часть может состоять из букв, цифр, симвов ``_`` или ``$``. (запрет на использования цифр в качестве первого символа идентификатора необходим для избежания путаницы с числовыми летаралами)
В EcmaScript 3 идентификаторы могут содержать буквы и цифры из полного набора символов Unicode, более старые же версии ограничены набором символов ASCII.

Ну и наконец идентификаторы не могут совпадать с ключевыми (зарезеревированными) словами языка (``for``, ``if``, и т.д.). Полный список ключевых слов можно посмотреть [тут](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Lexical_grammar#Keywords)

Во многих языках программирования, по мимо переменных, существуют так же константы.
В JavaScript, увы, изначально не было способа создания констант (он появился только в EcmaScript 6, подробнее [тут](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Statements/const)), поэтому, для того чтоб отличить их от перменных, константы обычно именуют заглавными буквами:

```
var IamVariable = 42;
var I_AM_CONSTANT = 42;
```


#### Запуск JavaScript вне браузера

На сегодняшний день одной из самых популярных сред, где исполняется JavaScript код, по мимо браузера, является NodeJS
Подробную инструкцию по установке, ровно как и документацию можно найти на [официальном сайте](https://nodejs.org/)

Итак, нода готова к запуску и пришло время написать первую программу.
Создадим файл ``index.js`` со следующим кодом внутри:

```
console.log('Hello world!');
```

И запустим его при помощи ноды из командной строки

```
cd <path_to_ur_index.js>
node index.js
```

#### Инструменты

* Текстовые редакторы:  [notepad++](https://notepad-plus-plus.org/), [atom](https://atom.io/) (*список открыт для предложений*)
* IDE: [WebStorm](https://www.jetbrains.com/webstorm/), [Brackeets](http://brackets.io/)
* *нужно ли добавлять тулзы для проверки качества кода?*

**Hint:** для WebStorm существует бесплатная студенческая лицензия, для её получаения необходимо:

1. завести [JetBrains Account](https://https://account.jetbrains.com/login)
2. подтвердить статус студента одним из следующий способов:
  * при помощи карточки [International Student Identity Card](https://www.isic.org/) (ISIC)
  * при электронной почты университета (в домене .edu)
  * при помощи скана студенческого билета

Подать заявку можно [тут](https://www.jetbrains.com/student/)

### Источники

* [http://www.infoworld.com/article/2653798/application-development/javascript-creator-ponders-past--future.html](http://www.infoworld.com/article/2653798/application-development/javascript-creator-ponders-past--future.html)
* [http://speakingjs.com/es5/pt02.html](http://speakingjs.com/es5/pt02.html)
* [http://dailyjs.com/2010/05/31/history-of-javascript-1/](http://dailyjs.com/2010/05/31/history-of-javascript-1/)
* [http://dailyjs.com/2010/05/31/history-of-javascript-2/](http://dailyjs.com/2010/05/31/history-of-javascript-2/)
* [http://dailyjs.com/2010/05/31/history-of-javascript-3/](http://dailyjs.com/2010/05/31/history-of-javascript-3/)
* [https://www.w3.org/community/webed/wiki/A_Short_History_of_JavaScript](https://www.w3.org/community/webed/wiki/A_Short_History_of_JavaScript)
* [YDKJS: Up & going](https://github.com/getify/You-Dont-Know-JS)
* JavaScript: The Definitive Guide, 6th Edition
