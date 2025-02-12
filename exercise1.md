## HTTP-сообщения

**HTTP (HyperText Transfer Protocol**, дословно — «протокол передачи гипертекста») представляет собой протокол прикладного уровня, используемый для доступа к ресурсам Всемирной Паутины. Под термином гипертекст следует понимать текст, в понятном для человека представлении, при этом содержащий ссылки на другие ресурсы.

Данный протокол описывается спецификацией RFC 2616. На сегодняшний день наиболее распространенной версией протокола является версия HTTP/2, однако нередко все еще можно встретить более раннюю версию HTTP/1.1.
***
Данные между клиентом и сервером в рамках работы протокола передаются с помощью HTTP-сообщений. Они бывают двух видов:

**Запросы (HTTP Requests)** — сообщения, которые отправляются клиентом на сервер, чтобы вызвать выполнение некоторых действий. Зачастую для получения доступа к определенному ресурсу. Основой запроса является HTTP-заголовок.  

**Ответы (HTTP Responses)** — сообщения, которые сервер отправляет в ответ на клиентский запрос.
Само по себе сообщение представляет собой информацию в текстовом виде, записанную в несколько строчек.
***
В целом, как запросы HTTP, так и ответы имеют следующую структуру:

**Стартовая строка (start line)** — используется для описания версии используемого протокола и другой информации — вроде запрашиваемого ресурса или кода ответа. Как можно понять из названия, ее содержимое занимает ровно одну строчку.  

**HTTP-заголовки (HTTP Headers)** — несколько строчек текста в определенном формате, которые либо уточняют запрос, либо описывают содержимое тела сообщения.  

**Пустая строка**, которая сообщает, что все метаданные для конкретного запроса или ответа были отправлены.  

**Опциональное тело сообщения**, которое содержит данные, связанные с запросом, либо документ (например HTML-страницу), передаваемый в  ответе.
Рассмотрим атрибуты HTTP-запроса подробнее.

***
### Стартовая строка

Стартовая строка, в зависимости от типа сообщения, называется **Request-Line или Status-Line**.

***
Стартовая строка HTTP-запроса (Request-Line )состоит из трех элементов:

1. Метод HTTP-запроса (method, реже используется термин verb).   
Обычно это короткое слово на английском, которое указывает, что конкретно нужно сделать с запрашиваемым ресурсом. Например, метод GET сообщает серверу, что пользователь хочет получить некоторые данные, а POST — что некоторые данные должны быть помещены на сервер.
2. Цель запроса.   
Представлена указателем ресурса URL, который состоит из протокола, доменного имени (или IP-адреса), пути к конкретному ресурсу на сервере. Дополнительно может содержать указание порта, несколько параметров HTTP-запроса и еще ряд опциональных элементов.
3. Версия используемого протокола (либо HTTP/1.1, либо HTTP/2),  
 которая определяет структуру следующих за стартовой строкой данных.

***

Стартовая строка HTTP-ответа называется строкой статуса (Status-Line). На ней располагаются следующие элементы:

1. Версия протокола (HTTP/2 или HTTP/1.1).
2. Код состояния, который указывает, насколько успешно завершилась обработка запроса.
3. Пояснение — короткое текстовое описание к коду состояния. Используется исключительно для того, чтобы упростить понимание и восприятие человека при просмотре ответа.

***
## HTTP методы

Методы позволяют указать конкретное действие, которое мы хотим, чтобы сервер выполнил, получив наш запрос.
1. GET  
Позволяет запросить некоторый конкретный ресурс. Дополнительные данные могут быть переданы через строку запроса (Query String) в составе URL (например ?param=value).
2. POST  
Позволяет отправить данные на сервер. Поддерживает отправку различных типов файлов, среди которых текст, PDF-документы и другие типы данных в двоичном виде. Обычно метод POST используется при отправке информации (например, заполненной формы логина) и загрузке данных на веб-сайт, таких как изображения и документы.
3. HEAD  
Здесь придется забежать немного вперед и сказать, что обычно сервер в ответ на запрос возвращает заголовок и тело, в котором содержится запрашиваемый ресурс. Данный метод при использовании его в запросе позволит получить только заголовки, которые сервер бы вернул при получении GET-запроса к тому же ресурсу. Запрос с использованием данного метода обычно производится для того, чтобы узнать размер запрашиваемого ресурса перед его загрузкой.
4. PUT  
Используется для создания (размещения) новых ресурсов на сервере. Если на сервере данный метод разрешен без надлежащего контроля, то это может привести к серьезным проблемам безопасности.
5. DELETE  
Позволяет удалить существующие ресурсы на сервере. Если использование данного метода настроено некорректно, то это может привести к атаке типа «Отказ в обслуживании» (Denial of Service, DoS) из-за удаления критически важных файлов сервера.
6. OPTIONS   
Позволяет запросить информацию о сервере, в том числе информацию о допускаемых к использованию на сервере HTTP-методов.
7. PATCH  
Позволяет внести частичные изменения в указанный ресурс по указанному расположению.









