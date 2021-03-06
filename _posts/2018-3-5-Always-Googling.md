---
layout: post
title: Постоянно это гуглю
---

:mag_right: Если что-то я погуглила минимум 2 раза и вот третий раз открываю гугл, чтобы это найти — самое время записать сюда после успешного поиска.

---

<h2 class="post__small-heading">Апдейт Node.js</h2>

via [stackoverflow](https://stackoverflow.com/questions/8191459/how-do-i-update-node-js)

<hr class="small">

1. Clear NPM's cache
2. Install a little helper called 'n'
3. Install latest stable Node.js version

<hr class="small">

  `sudo npm cache clean -f`

  `sudo npm install -g n`

  `sudo n stable`

---

<h2 class="post__small-heading">Проверка и апдейт пакетов npm</h2>

* Для начала нужно уставить глобально специальный пакет [npm-check](https://www.npmjs.com/package/npm-check)

  `npm install -g npm-check`

<hr class="small">

* Просто проверить глобально установленные пакеты

  `npm-check -g`

* Проверить и обновить нужные (покажет минорные/мажорные версии, главные фичи и т.п. — очень удобно!)

  `sudo npm-check -gu`

<hr class="small">

* Проверить пакеты в директории

  `cd <path>`

  `npm-check`

---

<h2 class="post__small-heading">Удаление пакетов npm</h2>

Чтобы что-то удалить, неплохо бы знать, что удалять :)

Начнем с глобально установленных пакетов.

<hr class="small">

* Посмотреть список всех глобально установленных пакетов (только на верхнем уровне, без погружения во внутренние зависимости — ибо обычно это несколько окон терминала)

  `npm list -g --depth=0`

<hr class="small">  

* Глобальное удаление пакетов (не требует установки чего-либо)

  `npm -g uninstall <package name>`

<hr class="small">

* Аналогично, но без флага `-g`, находясь в директории (ну или ручками, убрав пакет из `package.json`)

---
