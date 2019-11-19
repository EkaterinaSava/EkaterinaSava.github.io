---
layout: post
title: Памятка / Firebase
---

:fire: Мини-туториал по добавлению проектов в Firebase с возможностью захостить демки на их домене.

---

<h2 class="post__small-heading">Создание проекта</h2>

* Идем на сайт [https://firebase.google.com/](https://firebase.google.com/)

* В верхнем правом углу по ссылке переходим [в консоль](https://console.firebase.google.com/u/0/?pli=1)

* Жмем кнопку «Добавить проект», выбираем имя проекта и регион, создаем его

---

<h2 class="post__small-heading">Хостинг проекта</h2>

* Для начала единожды должно быть установлено `Firebase CLI`

```
npm install -g firebase-tools
```

* После этого нужно залогиниться (опять же глобально и единожды) через команду

```
firebase login
```

После этого откроется браузер и нужно будет залогиниться в гугло-аккаунт, после успешного логина в консоле будет надпись об успешном логине `✔  Success! Logged in as ekaterinasava@gmail.com`

* Находясь в папке проекта, который мы собираемся хостить, необходимо выподнить команду:

```
firebase init
```

* CLI сообщит, что мы собираемся инициализировать Firebase в этом каталоге и спросит, готовы ли мы продолжить, на что ему, конечно, надо написать `y`

* Далее он предложит список того, что можно сделать, нас интересует опция Hosting, которую мы и выбираем пробелом

* После уточняющих вопросов, на которые можно ответить, например, вот так (зависит от проекта):

```
? What do you want to use as your public directory? public
? Configure as a single-page app (rewrite all urls to /index.html)? Yes
? File public/index.html already exists. Overwrite? No
```

будет сообщение `Firebase initialization complete!`

* И после этого мы можем деплоить наше приложение через команду

```
firebase deploy
```

---
