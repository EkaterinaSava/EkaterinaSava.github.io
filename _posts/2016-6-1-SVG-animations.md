---
layout: post
title: SVG-анимации
---

:pencil2: В один прекрасный рабочий день передо мной встала не самая тривиальная задача – анимировать svg.
Несмотря на то, что svg-спрайты – ежедневная практика, знаний о том, с какого угла подступиться к решению задачи, не было. Поэтому пришлось провести self-ликбез по векторной графике и разобраться с ее анимированием.

---

<h2 class="post__small-heading"> Шаг 1 – Знакомство с "внутренностями" svg </h2>

Для начала стоит разобраться с тем, из чего "сделаны" svg-шки. Немного теории и практики.

1. Читаем отличную [статью на Frontender.info](http://frontender.info/using-svg/http://frontender.info/using-svg/) и при желании изучаем все материалы по приведенным в статье дополнительным ссылкам
2. После прочтения стоит пройти небольшой практический курс от HTML Academy [«Знакомство с SVG»](https://htmlacademy.ru/courses/130) и попрактиковать создание простых фигур  

---

<h2 class="post__small-heading"> Шаг 2 – Исследование способов анимации </h2>

Следующим этапом стал поиск возможностей для анимирования векторной графики и первое, на что вы наткнетесь при аналогичном желании - море туториалов с использованием [SMIL](https://ru.wikipedia.org/wiki/SMIL). То, что нужно сделать, увидев это слово в любой открытом вами материале – сразу же его закрыть. 
Ибо запустив в браузере заботливо написанный по такому туториалу код, вы увидите в консоли вот такое сообщение: _SVG's SMIL animations (`<animate>`, `<set>`, etc.) are deprecated and will be removed. Please use CSS animations or Web animations instead_, что абсолютно нам не подходит, 
да и плюс [нулевая поддержка](http://caniuse.com/#feat=svg-smil) от IE должна окончательно остановить вас.

Двигаясь дальше в изучении вопроса анимаций svg, мы поймем, что имеем в распоряжении как немалое количество js-библиотек для решения подобных задач:

1. [Svg.js](http://svgjs.com/)
2. [Vivus](https://maxwellito.github.io/vivus/https://maxwellito.github.io/vivus/)
3. [GSAP](http://greensock.com/gsap)
4. [Snap.svg](http://snapsvg.io/)

Для решения своей задачи я остановила выбор на последней, ибо в наличии нашлось немало туториалов, кодпенов и примеров, что значительно упрощало старт.
  
---

<h2 class="post__small-heading"> Шаг 3 – Результаты </h2>

В процессе изучения выбранной мной библиотеки, я реализовала несколько примеров анимации, которые можно посмотреть на CodePen по ссылкам ниже:
  
* Анимация текстовой svg-маски

<p data-height="265" data-theme-id="light" data-slug-hash="EyaKVE" data-default-tab="result" data-user="EkaterinaSava" data-embed-version="2" class="codepen">See the Pen <a href="https://codepen.io/EkaterinaSava/pen/EyaKVE/">Svg Animated Text Mask</a> by Ekaterina Sava (<a href="http://codepen.io/EkaterinaSava">@EkaterinaSava</a>) on <a href="http://codepen.io">CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

* Анимация иконки по клику

<p data-height="265" data-theme-id="light" data-slug-hash="gMpgNG" data-default-tab="result" data-user="EkaterinaSava" data-embed-version="2" class="codepen">See the Pen <a href="http://codepen.io/EkaterinaSava/pen/gMpgNG/">Animate svg icon on click</a> by Ekaterina Sava (<a href="http://codepen.io/EkaterinaSava">@EkaterinaSava</a>) on <a href="http://codepen.io">CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

---  

Кроме того, в процессе я попробовала еще некоторые варианты __без использования скриптов__:

* Анимация внутри текстовой маски через изменение stroke-width

<p data-height="265" data-theme-id="light" data-slug-hash="ZOYPxw" data-default-tab="result" data-user="EkaterinaSava" data-embed-version="2" class="codepen">See the Pen <a href="https://codepen.io/EkaterinaSava/pen/ZOYPxw/">Text with animated pattern</a> by Ekaterina Sava (<a href="http://codepen.io/EkaterinaSava">@EkaterinaSava</a>) on <a href="http://codepen.io">CodePen</a>.</p>

---

  <h2 class="post__small-heading"> Почитать дополнительно </h2>

  * [CSS и SVG маски](http://css.yoksel.ru/css-and-svg-masks/)

--- 