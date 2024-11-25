⌨️ WebSocket.
=====

### EN
*WebSocket* is a computer communications protocol, providing a simultaneous two-way communication channel over a single Transmission Control Protocol (TCP) connection. The WebSocket protocol was standardized by the IETF as RFC 6455 in 2011.

-----

### RU
*WebSocket* - это протокол компьютерной коммуникации, который обеспечивает одновременный двусторонний обмен данными через одно соединение, используя TCP. 
Проще говоря, он позволяет устанавливать интерактивные соединения между клиентом и сервером для обмена сообщениями в режиме реального времени, что делает его идеальным выбором для динамичных приложений, таких как чаты, онлайн-игры и системы уведомлений.

#### HTTP и WebSocket: ?
- HTTP - Клиент (например, браузер) отправляет запрос серверу и ждет ответа. Сервер сам не может отправить сообщение клиенту - только если клиент снова сделает запрос. Это похоже на то, как если бы вы спрашивали друга, готов ли он, и ждали его ответа каждый раз.

- WebSocket - Здесь между клиентом и сервером устанавливается постоянное соединение. Они могут отправлять сообщения друг другу в любой момент. Это как если бы вы с другом держали открытый телефонный разговор и могли говорить, когда захотите, без необходимости перезванивать.

### HTTP - запрос и ответ.
### WebSocket - общение в реальном времени.
-----

### Протокол WebSocket был стандартизирован IETF как RFC 6455 в 2011 году.

- IETF (Internet Engineering Task Force) - это организация, которая разрабатывает и поддерживает технические стандарты для Интернета, такие как протоколы и архитектуры. Ее работа помогает обеспечивать совместимость и надежность сетевых технологий.

- RFC 6455 - это документ (Request for Comments), опубликованный IETF в 2011 году, в котором описан стандарт для протокола WebSocket. Он детально объясняет, как устанавливать, поддерживать и завершать двунаправленное соединение между клиентом и сервером.

- RFC-документы служат официальными техническими руководствами для разработчиков и инженеров, работающих с интернет-протоколами.
-----

#### WebSocket часто используется в следующих случаях:

1. Чаты и мессенджеры - для обеспечения мгновенной передачи сообщений между пользователями.
2. Реалтайм-обновления в приложениях - например, обновление курсов акций или отображение результатов спортивных событий в реальном времени.
3. Такси и геолокационные приложения: для обновления местоположения водителя и клиента в режиме реального времени.
4. Игры: для передачи данных о состоянии игры между сервером и игроками.
5. Уведомления в реальном времени: приложения, которым необходимо отправлять пользователям мгновенные уведомления.
-----

1. TCP (Transmission Control Protocol)

- TCP - это один из основных протоколов Интернета, который обеспечивает надежную передачу данных. Он гарантирует, что данные передаются в правильном порядке и без потерь.
- Где используется? Используется для сетевых соединений, требующих надежной доставки данных, например, для работы с WebSocket. WebSocket открывает соединение поверх TCP, чтобы поддерживать постоянное соединение между клиентом и сервером.

2. TLS (Transport Layer Security)

- TLS - протокол безопасности, обеспечивающий шифрование данных при передаче по сети. Он защищает соединение от перехвата данных и атак типа «человек посередине» (Man-in-the-Middle).
- Где используется? WebSocket может использовать TLS для безопасного соединения, что превращает его в wss:// (WebSocket Secure), аналогично тому, как HTTP превращается в HTTPS.
- Пример использования: WebSocket-соединение может быть защищено через wss://example.com, чтобы передаваемые данные были зашифрованы и недоступны для злоумышленников.

3. SSE (Server-Sent Events)
- SSE - это технология, позволяющая серверу отправлять данные клиенту в режиме реального времени по одностороннему соединению. В отличие от WebSocket, соединение устанавливается только от сервера к клиенту.
- Где используется? SSE подходит для простых реализаций, где нужно передавать данные только от сервера клиенту, например, для обновления новостей или уведомлений. SSE проще, чем WebSocket, но не поддерживает двустороннюю связь.
- Когда использовать? SSE подходит для случаев, когда приложение требует только поток данных от сервера (например, ленты новостей), а WebSocket лучше использовать, когда требуется двусторонняя связь (например, чаты).

-----

