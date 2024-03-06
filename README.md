Анализ применимости web-серверов на платформе github


Для анализа применимости веб-серверов, можно рассмотреть три наиболее популярных репозитория на платформе GitHub, которые представляют собой веб-серверы или инструменты для анализа веб-трафика и веб-аналитики. Эти репозитории включают в себя:
1.	Matomo (matomo-org/matomo): Это открытый источник альтернативы Google Analytics, который позволяет полностью контролировать собранные данные. Matomo собирает данные с веб-сайтов и приложений и визуализирует эти данные для извлечения инсайтов. Приватность встроена в основу этого инструмента, что делает его привлекательным для тех, кто заботится о защите личных данных пользователей [1].
2.	Plausible (plausible/analytics): Это легкий (менее 1 КБ) и приватный аналог Google Analytics, написанный на Elixir. Plausible фокусируется на простоте и приватности, предоставляя пользователям инструменты для отслеживания посещаемости сайта без использования куки или JavaScript [1].
3.	GoAccess (allinurl/goaccess): GoAccess - это инструмент для анализа веб-логов в реальном времени и интерактивного просмотра, который работает в терминале на системах *nix или через браузер. Этот инструмент позволяет анализировать логи веб-серверов и визуализировать данные о трафике, что может быть полезно для мониторинга производительности и безопасности веб-сайтов [1].
	Эти репозитории представляют собой различные подходы к анализу веб-трафика и веб-аналитике, от полноценных аналогов Google Analytics до инструментов для анализа веб-логов в реальном времени. Выбор между ними зависит от конкретных потребностей в приватности, производительности и удобстве использования.

Matomo может собирать различные данные, включая информацию, которая может быть личной, частной, чувствительной и/или конфиденциальной. Вот основные категории данных, которые
Matomo может отслеживать:

•	Анонимные IP-адреса: Matomo может собирать IP-адреса пользователей, но предлагает возможность анонимизации IP-адресов до определенного уровня, чтобы защитить личные данные пользователей [2].

•	Пользовательские идентификаторы: Matomo может отслеживать пользовательские идентификаторы, которые могут быть личными данными. Существует возможность активировать функцию приватности для замены каждого идентификатора пользователя псевдонимом [2].

•	Пользовательские измерения и переменные: Эти данные могут хранить личные данные, в зависимости от того, как они настроены и используются на сайте [2].

•	Поиск на сайте: Поиск на вашем сайте может содержать личные данные, например, когда пользователи ищут свое имя или почтовый индекс [2].

•	Heatmap и записи сессий: Эти данные могут содержать личные данные, например, профиль пользователя на социальной медиа-сайте, который будет записан в Heatmap и/или записи сессий. Если вы не хотите отслеживать эти данные, можно использовать атрибут data-matomo-mask для их исключения [2].

•	URL страниц и заголовки страниц: Эти данные могут содержать личные данные, в зависимости от того, как ваш сайт разработан [2].

•	URL-адреса ссылок: Могут содержать личные данные, например, когда ваши пользователи приходят с другого веб-сайта, который раскрывает личные данные ваших посетителей в URL-адресах страниц [2].

•	ID заказов электронной коммерции: Обычно считаются личными данными, поскольку ID заказа может быть связан с конкретным клиентом. Существует возможность активировать функцию приватности для замены каждого ID заказа псевдонимом [2].

•	Геолокация: Основывается на IP-адресе и может считаться личными данными [2].

  Matomo также собирает и обрабатывает следующую личную информацию по умолчанию:
  
•	IP-адрес: Используется для определения местоположения пользователя. Matomo автоматически анонимизирует IP-адрес, скрывая последнюю часть [3].

•	URL-адреса и заголовки страниц: Помогают понять, как люди используют ваш сайт, но могут содержать личные данные [3].

•	URL-адреса ссылок: Могут содержать личные данные, такие как идентификаторы ссылок Facebook/Google и даже URL-адреса профилей третьих сторон [3].

•	ID отслеживания cookies: Уникальные идентификаторы, которые могут помочь определить, является ли посещение новым или возвращающимся пользователем [3].

•	Данные геолокации: Полезны для понимания географических тенденций посетителей вашего сайта [3].

•	Поиск на сайте: Возможность, что пользователь может ввести личные данные, ища информацию на вашем сайте [3].

Matomo предлагает гибкие настройки для управления сбором личных данных, позволяя активировать функцию приватности для замены личных данных на псевдонимы и предлагая возможности анонимизации IP-адресов.

Преимущества Plausible:

•	Простота и легкость использования: Plausible предлагает простой и интуитивно понятный интерфейс, без необходимости обучения или предварительного опыта. Это делает его доступным для широкого круга пользователей, включая новичков в области веб-аналитики [4].

•	Приватность и защита данных: Plausible разработан с учетом приватности пользователей и не требует от них согласия на использование куки и других механизмов отслеживания. Это особенно важно для соблюдения регулятивных требований, таких как GDPR и CCPA [4].

•	Низкое влияние на производительность сайта: Вес скрипта Plausible составляет менее 1 КБ, что значительно меньше, чем у Google Analytics. Это помогает уменьшить время загрузки страниц и улучшить общую производительность сайта [4].

•	Открытый исходный код и самостоятельный хостинг: Plausible доступен как открытый исходный код, что позволяет разработчикам и организациям самостоятельно хостить его. Это также позволяет полностью контролировать собранные данные [4].

Недостатки Plausible:

•	Ограниченный функционал по сравнению с Google Analytics: Google Analytics предлагает более широкий спектр функций и глубокие аналитические возможности, которые могут быть необходимы для более сложных веб-сайтов и бизнес-аналитики. Plausible может не предлагать все необходимые инструменты для некоторых задач [5].

•	Меньшая популярность и доступность поддержки: Поскольку Google Analytics является более устоявшейся и широко используемой системой, есть больше доступных ресурсов и сообществ для поддержки. Plausible, будучи новым и менее распространенным инструментом, может иметь меньше ресурсов для обучения и поддержки [5].

•	Недостаток некоторых функций: В то время как Plausible фокусируется на приватности и простоте, некоторые пользователи могут искать более продвинутые функции, доступные в Google Analytics, такие как детальный анализ пользовательского поведения, интеграция с другими сервисами и возможности для создания пользовательских отчетов [5].
	В целом, выбор между Plausible и Google Analytics зависит от конкретных потребностей в аналитике, приоритетов в приватности данных пользователей и доступности ресурсов для обучения и поддержки.

GoAccess предоставляет возможность визуализации различных типов данных, полученных из веб-серверов, таких как Nginx и Apache. Основные типы данных, которые можно визуализировать с помощью GoAccess, включают:

•	Статистика по страницам: Позволяет анализировать, какие страницы сайта наиболее посещаемы. Это может помочь в определении наиболее популярного контента и страниц с высоким трафиком.

•	Статистика по источникам трафика: GoAccess может отслеживать, откуда приходит трафик на сайт. Это может включать информацию о поисковых системах, ссылках на другие сайты, социальных сетях и т.д.

•	Статистика по браузерам и операционным системам: Анализ данных о том, какие браузеры и операционные системы используют посетители сайта. Это может быть полезно для определения совместимости и оптимизации контента.

•	Статистика по географическому расположению: GoAccess может предоставить информацию о географическом расположении посетителей, что может быть полезно для определения аудитории сайта и оптимизации контента для определенных регионов.

•	Статистика по HTTP-методам: Анализ данных о том, какие HTTP-методы (GET, POST и т.д.) используются для доступа к сайту.

•	Статистика по статусам ответов HTTP: Мониторинг статусов ответов HTTP (200 OK, 404 Not Found и т.д.) помогает определить эффективность работы сервера и наличие потенциальных проблем.

•	Статистика по протоколам: Мониторинг использования протоколов HTTP и HTTPS, что может быть полезно для определения безопасности и эффективности веб-сервера.
	
 GoAccess предлагает интерактивный интерфейс, который позволяет пользователям навигировать по данным в реальном времени и визуализировать различные типы данных для более глубокого анализа и понимания трафика веб-сайта. Это делает GoAccess мощным инструментом для анализа веб-трафика и мониторинга производительности веб-серверов.





Использованные источники:
1.	https://github.com/topics/web-analytics
2.	https://matomo.org/faq/general/faq_18254/
3.	https://matomo.org/faq/new-to-piwik/personal-data-matomo-analytics-collects-and-why/
4.	https://plausible.io/vs-google-analytics
5.	https://independentwp.com/blog/plausible-vs-google-analytics/


# Nastasya-1.2
