<a name="settings"></a>

Настройки
=========

Все настройки, описанные ниже, могут быть заданы несколькими способами.
Настройки задаются послойно, т.е. каждый следующий слой перезаписывает предыдущие настройки.

Способы задания настроек, упорядоченные по их приоритету:

-   Настройки в конфигурационных файлах сервера.

    Задаются через профили пользователей.

-   Для сессии.

    Из консольного клиента ClickHouse в интерактивном режиме отправьте запрос `SET setting=value`.
    Аналогично можно использовать ClickHouse-сессии в HTTP-протоколе, для этого необходимо указывать HTTP-праметр `session_id`.

-   Для запроса.
    -   При запуске консольного клиента ClickHouse в неинтерактивном режиме установите параметр запуска `--setting=value`.
    -   При использовании HTTP API передавайте cgi-параметры (`URL?setting_1=value&setting_2=value...`).

Настройки, которые можно задать только в конфигурационном файле сервера, в разделе не рассматриваются.

```eval_rst
.. toctree::
    :glob:

    *
```