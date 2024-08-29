---
icon: shield-halved
layout:
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Команды модерации

***

{% hint style="info" %}
**Подсказка**

**`<...>`** - обязательный аргумент.\
**`[...]`** - необязательный аргумент.

"/" в аргументе означает "или". \
Например, мьют участника: \
`unmute <@участник/ID участника>`\
`unmute @retrilzzy`\
`unmute` 613636431532785664

\
**`/команда`**- вызов через слэш(/).\
**`!команда`** - вызов через префикс (по умолчанию `!`, можно изменить при помощи [_`/manage-prefix`_](general.md#manage-prefix-ustanovite-svoi-prefiks-dlya-vashego-servera) или через [панель управления](https://dash.rzx-bot.top)).\
**`команда`** - вызов через слэш и префикс.
{% endhint %}

***

<details>

<summary><code>purge</code> - Очистка n количества сообщений в текущем канале</summary>

**Использование:**\
`purge <количество сообщений>`

**Пример:**\
**`!purge 5`**

</details>

<details>

<summary><code>purge_user</code> - Очистить все сообщения &#x3C;пользователя> в каждом канале за последние n минут</summary>

**Использование:** \
`purge_user <@участник/ID участника> [за последние сколько минут]`&#x20;

Пример:\
`!purge_user @retrilzzy 10`

</details>

<details>

<summary><code>purge_until</code> - Очистить сообщения в канале до заданного сообщения</summary>

**Использование:**\
`purge_until <ID сообщения>`

**Пример:**\
`!purge_until 1200619381080731648`

</details>

***

<details>

<summary><code>lock</code> - Блокирует отправку сообщений в канал</summary>

**Использование:**

`lock [#канал/ID канала]`

**Пример:**

`!lock #chat`

</details>

<details>

<summary><code>unlock</code> - Разблокирует канал</summary>

**Использование:**

`unlock [#канал/ID канала]`

**Примеры:**

`!unlock #чатик`

`!unlock 123456789`

</details>

<details>

<summary><code>mute</code> - Замьютить участника на сервере</summary>

**Использование:**

`mute <@участник/ID участника> <насколько минут> [причина]`

**Пример:**

`!mute @AKainly 10 проиграл все деньги в казике`

</details>

<details>

<summary><code>unmute</code> - Размьютить участника на сервере</summary>

**Использование:**

`unmute <@участник/ID участника>`

**Пример:**

`!unmute @Emika`

</details>

{% hint style="warning" %}
Для использования команд`lock unlock mute unmute`необходима роль с разрешением **"Управление сообщениями"** или вы должны быть **администратором**
{% endhint %}

<details>

<summary><code>kick</code>- Исключает участника с сервера</summary>

**Использование:**

`kick <@участник/ID участника> [причина]`

**Пример:**

`!kick @ds.mandar1n нубик`

</details>

{% hint style="warning" %}
Для использования команды `kick` необходима роль с разрешением **"Выгонять Участников"** или вы должны быть **администратором**
{% endhint %}

<details>

<summary><code>ban</code> - Забанить участника на сервере</summary>

**Использование:**

`ban <@участник/ID участника> [причина]`

**Пример:**

`!ban @ozai1155 24.3`

</details>

<details>

<summary><code>unban</code> - Разбанить участника на сервере</summary>

**Использование:**

`unban <ID пользователя>`

**Пример:**

`!unban 1089857134323306526`

</details>

{% hint style="warning" %}
Для использования команды `ban unban` необходима роль с разрешением **"Банить Участников"** или вы должны быть **администратором**
{% endhint %}

<details>

<summary><code>manage-roles</code> - Добавить или удалить роль у участника</summary>

**Использование:**

`manage-roles <добавить/убрать> <@участник/id> <@роль/id>`

**Пример:**

`!manage-roles добавить @ReZero2 Задрот`\
_Через слэш(/) удобнее_

</details>

{% hint style="warning" %}
Для использования команды `manage-roles` необходима роль с разрешением **"Управлять ролями"** или вы должны быть **администратором**
{% endhint %}
