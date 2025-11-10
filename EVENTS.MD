# Bitrix24 REST API — События

Полный список событий, доступных для подписки через REST API Bitrix24.

---

## 🧩 Приложения

| Событие | Описание |
|----------|-----------|
| **ONAPPINSTALL** | Установка приложения на портал. |
| **ONAPPUNINSTALL** | Удаление приложения. |
| **ONAPPUPDATE** | Обновление версии приложения. |
| **ONAPPPAYMENT** | Успешная оплата подписки. |
| **ONSUBSCRIPTIONRENEW** | Продление подписки. |
| **ONAPPTEST** | Тестовая установка (sandbox). |
| **ONAPPMETHODCONFIRM** | Подтверждение доступности метода. |
| **ONOFFLINEEVENT** | Событие, произошедшее в оффлайн-режиме. |

---

## 📅 Бронирования (Booking)

| Событие | Описание |
|----------|-----------|
| **ONBOOKINGRESOURCETYPEADD / UPDATE / DELETE** | Управление типами ресурсов (например, переговорные). |
| **ONBOOKINGRESOURCEADD / UPDATE / DELETE** | Создание, изменение, удаление ресурса. |
| **ONBOOKINGADD / UPDATE / DELETE** | Добавление, изменение или удаление бронирования. |
| **ONBOOKINGWAITLISTITEMADD / UPDATE / DELETE** | Работа со списком ожидания. |

---

## 👥 HR / HCM Интеграции

| Событие | Описание |
|----------|-----------|
| **ONHUMANRESOURCESHCMLINKEMPLOYEELISTREQUESTED** | Запрошен список сотрудников. |
| **ONHUMANRESOURCESHCMLINKFIELDVALUEREQUESTED** | Запрошено значение поля. |
| **ONHUMANRESOURCESHCMLINKEMPLOYEELISTMAPPED** | Список сотрудников сопоставлен. |
| **ONSIGNHCMLINKB2EDOCUMENTSIGNED** | Документ B2E подписан. |

---

## 💬 Коммуникации (IM, Open Lines, Bots)

| Событие | Описание |
|----------|-----------|
| **ONIMCONNECTORMESSAGEADD / UPDATE / DELETE** | Сообщения от внешних коннекторов (Telegram, WhatsApp и др.). |
| **ONIMCONNECTORDIALOGSTART / FINISH** | Начало или завершение диалога. |
| **ONIMBOTMESSAGEADD / UPDATE / DELETE** | Сообщения чат-бота. |
| **ONIMBOTJOINCHAT / ONIMBOTDELETE / ONIMBOTCONTEXTGET** | Присоединение, удаление или запрос контекста бота. |
| **ONIMCOMMANDADD** | Добавление пользовательской команды. |
| **ONOPENLINEMESSAGEADD / UPDATE / DELETE** | Сообщения открытых линий. |
| **ONSESSIONSTART / FINISH** | Начало / завершение сессии чата. |

---

## 🛒 Каталог и Торговля (Catalog / Sale)

| Событие | Описание |
|----------|-----------|
| **CATALOG.PRICE.ON.ADD / UPDATE / DELETE** | Работа с ценами. |
| **CATALOG.PRODUCT.ON.ADD / UPDATE / DELETE** | Добавление или изменение товаров. |
| **CATALOG.MEASURE.ON.ADD / UPDATE / DELETE** | Управление единицами измерения. |
| **CATALOG.ROUNDING.ON.ADD / UPDATE / DELETE** | Настройка округления цен. |
| **CATALOG.PRICE.TYPE.ON.ADD / UPDATE / DELETE** | Типы цен. |
| **ONSALEORDERSAVED / ONSALEBEFOREORDERDELETE** | Сохранение или удаление заказа. |
| **ONPAYMENTENTITYSAVED / ONSHIPMENTENTITYSAVED** | Сохранение платежей и отгрузок. |
| **ONORDERENTITYSAVED / ONORDERDELETED** | Изменение или удаление сущности заказа. |

---

## 👤 Пользователи

| Событие | Описание |
|----------|-----------|
| **ONUSERADD** | Создание пользователя. |
| **MAIN.ON.USER.TYPE.ADD / UPDATE / DELETE** | Изменение типов пользователей. |

---

## ✅ Задачи (Tasks)

| Событие | Описание |
|----------|-----------|
| **ONTASKADD / UPDATE / DELETE** | Создание, изменение, удаление задачи. |
| **ONTASKCOMMENTADD / UPDATE / DELETE** | Работа с комментариями задачи. |

---

## 💼 CRM

| Сущность | Примеры событий | Описание |
|-----------|----------------|-----------|
| **Лиды** | `ONCRMLEADADD`, `ONCRMLEADUPDATE`, `ONCRMLEADDELETE` | Изменения лидов. |
| **Сделки** | `ONCRMDEALADD`, `ONCRMDEALUPDATE`, `ONCRMDEALDELETE`, `ONCRMDEALMOVETOCATEGORY` | Работа со сделками. |
| **Компании** | `ONCRMCOMPANYADD`, `ONCRMCOMPANYUPDATE`, `ONCRMCOMPANYDELETE` | CRUD операций по компаниям. |
| **Контакты** | `ONCRMCONTACTADD`, `ONCRMCONTACTUPDATE`, `ONCRMCONTACTDELETE` | CRUD операций по контактам. |
| **Котировки (Quotes)** | `ONCRMQUOTEADD`, `ONCRMQUOTEUPDATE`, `ONCRMQUOTEDELETE` | Работа с коммерческими предложениями. |
| **Пользовательские поля** | `...USERFIELDADD / UPDATE / DELETE / SETENUMVALUES` | Изменения пользовательских полей. |
| **Валюты / Товары / Свойства / Разделы** | `ONCRMCURRENCY*`, `ONCRMPRODUCT*`, `ONCRMPRODUCTPROPERTY*`, `ONCRMPRODUCTSECTION*` | Изменения справочников. |
| **Активности** | `ONCRMACTIVITYADD / UPDATE / DELETE` | Добавление, изменение, удаление дел. |
| **Реквизиты / Банковские данные / Адреса** | `ONCRMREQUISITE*`, `ONCRMBANKDETAIL*`, `ONCRMADDRESS*` | Работа с реквизитами. |
| **Повторяющиеся сущности** | `ONCRMDEALRECURRING*`, `ONCRMINVOICERECURRING*` | Повторяющиеся сделки и счета. |
| **Таймлайн** | `ONCRMTIMELINECOMMENT*`, `ONCRMTIMELINEITEMACTION` | Комментарии и действия в истории. |
| **Динамические сущности (Smart Process)** | `ONCRMDYNAMICITEMADD_*`, `UPDATE_*`, `DELETE_*` | Smart Process элементы (кастомные типы). |
| **Типы сущностей** | `ONCRMTYPEADD / UPDATE / DELETE` | Управление типами CRM-сущностей. |
| **Документы** | `ONCRMDOCUMENTGENERATORDOCUMENT*` | События генерации документов. |
| **Счета (Invoices)** | `ONCRMINVOICEADD / UPDATE / DELETE / SETSTATUS` | Изменения в счетах. |

---

## ☎️ Телефония (Voximplant / External)

| Событие | Описание |
|----------|-----------|
| **ONVOXIMPLANTCALLINIT / START / END** | Инициация, начало, завершение звонка. |
| **ONEXTERNALCALLSTART / ONEXTERNALCALLBACKSTART** | Входящий или обратный вызов через внешнюю телефонию. |

---

## 📆 Календарь

| Событие | Описание |
|----------|-----------|
| **ONCALENDARENTRYADD / UPDATE / DELETE** | События календаря. |
| **ONCALENDARSECTIONADD / UPDATE / DELETE** | Разделы календаря. |
| **ONCALENDARROOMCREATE / UPDATE / DELETE** | Управление комнатами календаря. |

---

## 📰 Живая лента и Соцсеть

| Событие | Описание |
|----------|-----------|
| **ONLIVEFEEDPOSTADD / UPDATE / DELETE** | Публикации в живой ленте. |
| **ONSONETGROUPADD / UPDATE / DELETE** | Работа с группами. |
| **ONSONETGROUPSUBJECTADD / UPDATE / DELETE** | Темы (категории) групп. |


