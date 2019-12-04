---
layout: post
title: React Course
---

 :mortar_board: С 14 ноября по 23 декабря 2019 года я буду обучаться на [курсе по React](https://learn.javascript.ru/courses/react) от портала [learn.javascript.ru](https://learn.javascript.ru). Здесь буду вести дневник основных этапов обучения и выполнения домашних заданий, а также записывать важные теоретические материалы. 

* Занятия 2 раза в неделю по пн и чт по полтора часа

* Преподаватель — [Максим Крамаренко](https://learn.javascript.ru/profile/maksym-kramarenko)

_Этот пост существует тут исключительно для личной мотивации, самоконтроля и структурирования материала в голове._

---

<h2 class="post__small-heading">:large_blue_circle: Занятие #0 / Организационное</h2>

**_14/11/2019_**

Первое занятие шло 40 минут и было посвященно общим и организационным вопросам.
К занятию #1 (первому полноценному) в понедельник преподаватель порекомендовал изучить слудующие материалы:

* [Скринкаст по React.js](https://learn.javascript.ru/screencast/react) — как сказал Маским, это единственная обязательная домашка за весь курс (все остальные, по большому счету, по желанию)

* Порекомендовал освежить в памяти 4 крупные темы из [учебника по Javascript](https://learn.javascript.ru/):

    + [Деструктуризация](https://learn.javascript.ru/destructuring-assignment)

    + [Классы](https://learn.javascript.ru/class)

    + [Промисы](https://learn.javascript.ru/async)

    + [Модули](https://learn.javascript.ru/modules)

* При отсутствии знаний и наличии времени — посмотреть скринкасты:

    + по [гиту](https://learn.javascript.ru/screencast/git)

    + и [вебпаку](https://learn.javascript.ru/screencast/webpack)

<hr class="small">

### :small_blue_diamond: Домашка #0

<h5 class="post__underlined-heading">Скринкаст</h5>

<div class="post__block post__block--left-space">
    <p>Посмотрела 2 раза и написала код.</p>
    <p>Мой код живет <a href="https://github.com/EkaterinaSava/react__screencast">тут</a></p>
    <p>А оригинальный код автора курса — <a href="https://github.com/javascriptru/react-screencast-code">здесь</a></p>
</div>

<!-- <h5 class="post__underlined-heading">Теория по JS-y</h5>

<div class="post__block post__block--left-space">
    <p><b>Деструктуризация</b></p>
    <p>Более точное название <b><i>деструктурирующее присваивание</i></b></p>
    <p><b>Классы</b></p>
    <p><b>Промисы</b></p>
    <p><b>Модули</b></p>
</div> -->

---

<h2 class="post__small-heading">:large_blue_circle: Занятие #1</h2>

**_18/11/2019_**

__Продолжительность:__ 1 час 55 минут

__Краткое содержание:__

+ Заинитили новый проект через create-react-app

+ Создали ряд компонентов: app, restaurants, dishes и dish

+ Написали эти компоненты в разных стилях: через классы и через функции

+ Рассмотрели хуки, написали кастоный хук

+ Подключили к проекту сторонний фреймворк Ant для стилизации проекта

__Ссылки от преподавателя__ по темам первого занятия:

+ [Create React App](https://github.com/facebook/create-react-app)

+ [Husky для прекоммит-хуков](https://www.npmjs.com/package/husky)

+ [Dev-сервер Вебпака](https://webpack.js.org/configuration/dev-server/)

+ [Жизненные циклы Реакта](http://projects.wojtekmaj.pl/react-lifecycle-methods-diagram/)

+ [Теория о Javascript-модулях](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules)

+ [Введение в react-хуки](https://reactjs.org/docs/hooks-intro.html)

+ [Документация фреймворка Ant Design](https://ant.design/)


Плюс ссылка на [репозиторий нашего учебного проекта](https://github.com/Ta4i/react-2019-11-14), в нем же — описание первого домашнего задания, а также алгоритма по которому нужно его делать.

<hr class="small">

### :small_blue_diamond: Домашка #1

__Задание:__
1. Реализовать компоненту Restautant (class/func);
2. Вывести средний рейтинг ресторана с помощью компоненты [Rate](https://ant.design/components/rate/);
3. Вывести список отзывов;
4. *Сделать наше приложение красивее с помощью компонент [https://ant.design/](https://ant.design/);

Мой форкнутый репозиторий — [https://github.com/EkaterinaSava/react-2019-11-14](https://github.com/EkaterinaSava/react-2019-11-14)

Моя ветка с первым д/з — [home-work-1](https://github.com/EkaterinaSava/react-2019-11-14/tree/home-work-1)

Кроме этого залила первую домашку через Firebase на хостинг [https://react-course-hw-1-by-sava.firebaseapp.com](https://react-course-hw-1-by-sava.firebaseapp.com)

Ссылка на пулл-реквест — [https://github.com/Ta4i/react-2019-11-14/pull/9](https://github.com/Ta4i/react-2019-11-14/pull/9)

---

<h2 class="post__small-heading">:large_blue_circle: Занятие #2</h2>

**_21/11/2019_**

__Продолжительность:__ 1 час 50 минут

__Краткое содержание:__

+ Прошлись по основным моментам домашнего задания, обсудили ошибки и возможные улучшения

+ Рассмотрели, что такое `defaultProps` и добавили пример к компоненту

+ Подключили пакет `prop-types` и добавили `propTypes` для компонента рейтинга

+ Рассмотрели "хук" `componentDidCatch` и пример с его использованием

+ Подключили к проекту пакет `enzyme` и адаптер для него

+ Написали тест с помощью `Jest` и `Enzyme` для компонента ресторана

+ Рассмотрели асинхронные тесты

<hr class="small">

### :small_blue_diamond: Домашка #2

__Задание:__
1. Покрыть тестами блюда;
2. Написать PropTypes для компонент (сколько хватит сил).

Моя ветка со вторым д/з — [home-work-2](https://github.com/EkaterinaSava/react-2019-11-14/tree/home-work-2)

Ссылка на пулл-реквест — [https://github.com/Ta4i/react-2019-11-14/pull/21](https://github.com/Ta4i/react-2019-11-14/pull/21)

---

<h2 class="post__small-heading">:large_blue_circle: Занятие #3</h2>

**_25/11/2019_**

__Продолжительность:__ 1 час 50 минут

__Краткое содержание:__

+ Прошлись по основным моментам домашнего задания, обсудили тесты и `propTypes`

+ Добавили компонент корзины `cart-badge` в хэдэр

+ Добавили в проект `redux`

+ Использовали в `App`-компоненте `Provider` и `store`

+ Создали компонент `Counter` и несколько редьюсеров

+ Переделали получение данных о ресторанах, теперь они берутся из `store`

+ Добавили корзине возможность читать данные из `store` о количестве блюд

<hr class="small">

### :small_blue_diamond: Домашка #3

__Задание:__
1. Реализовать удаление блюда с корзины;
2. Создать компоненту Order, в которой выводить все блюда с корзины с названием и стоимостью, и выводить общую стоимость.

Моя ветка с третьим д/з — [home-work-3](https://github.com/EkaterinaSava/react-2019-11-14/tree/home-work-3)

Ссылка на пулл-реквест — [https://github.com/Ta4i/react-2019-11-14/pull/32](https://github.com/Ta4i/react-2019-11-14/pull/32)*

_*К сожалению, я сделала только первую часть д/з, мне не хватило времени к обозначенному для д/з сроку разобраться как делать второе задание, оно показалось мне порядочно сложное. Не поняла как правильно как брать данные о выбранных блюдах из стора._

---

<h2 class="post__small-heading">:large_blue_circle: Занятие #4</h2>

**_28/11/2019_**

__Продолжительность:__ 1 час 45 минут

__Краткое содержание:__

+ Изменили стуктуру наших (замоканых) данных, теперь они "нормализованы"

+ Добавили так называемые `selectors` и специальный npm-пакет `reselect` в проект

+ Переделали компонент `Dishes` в связи с новой структурой данных

+ Рассмотрели такую сущность как `middleware`

+ Добавили в компонент `Review` форму для отзывов

+ Добавили в проект пакет `redux-devtools-extension` и рассмотрели как он работает


<hr class="small">

### :small_blue_diamond: Домашка #4

__Задание:__
1. Починить Reviews и AverageRating;
2. Добавлять отзыв к ресторану;
3. Надо генерировать id комментария и нового пользователя в middlewares.

Моя ветка с третьим д/з — [home-work-4](https://github.com/EkaterinaSava/react-2019-11-14/tree/home-work-4)

Ссылки на пулл-реквест в этот раз нет: я перестала окончательно понимать, что происходит, попыталась скомпиллировать д/з из работ других учеников, но окончательно запуталась и решила, что так не годится делать домашку — надо пересматривать лекции и как-то разбираться.

---

<h2 class="post__small-heading">:large_blue_circle: Занятие #5</h2>

**_05/12/2019_**

__Продолжительность:__ 1 час хх минут

__Краткое содержание:__

---

<!-- 14/11/2019 -->
