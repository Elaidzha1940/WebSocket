⌨️ WebSocket.
=====

### EN
*WebSocket* is a computer communications protocol, providing a simultaneous two-way communication channel over a single Transmission Control Protocol (TCP) connection. The WebSocket protocol was standardized by the IETF as RFC 6455 in 2011.

-----

### RU
*WebSocket* - это протокол компьютерных коммуникаций, обеспечивающий одновременный двусторонний канал связи через одно соединение с использованием протокола управления передачей данных (TCP). Протокол WebSocket был стандартизирован IETF как RFC 6455 в 2011 году.

### Где применяется WebSocket?

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

- TLS — протокол безопасности, обеспечивающий шифрование данных при передаче по сети. Он защищает соединение от перехвата данных и атак типа «человек посередине» (Man-in-the-Middle).
- Где используется? WebSocket может использовать TLS для безопасного соединения, что превращает его в wss:// (WebSocket Secure), аналогично тому, как HTTP превращается в HTTPS.
- Пример использования: WebSocket-соединение может быть защищено через wss://example.com, чтобы передаваемые данные были зашифрованы и недоступны для злоумышленников.

-----
