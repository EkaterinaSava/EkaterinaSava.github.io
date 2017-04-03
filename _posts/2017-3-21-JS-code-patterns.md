---
layout: post
title: JavaScript Code Patterns
---

:pencil: Полезные шаблоны

---

  <h2 class="post__small-heading">«Модули»</h2>

  По мотивам «You dont know JS: Scope & Closures» – Глава 5: Замыкание области видимости ([:link:подглава «Модули»](https://github.com/azat-io/you-dont-know-js-ru/blob/master/scope%20%26%20closures/ch5.md#Модули))

  Замыкания являются весьма мощным инструментом, дающим доступ к шаблонам, таким как модули в их различных формах.

  Модули требуют две ключевых характеристики:

  1) внешнюю функцию-обертку, которую будут вызывать, чтобы создать закрытую область видимости

  2) возвращаемое значение функции-обертки должно включать в себя ссылку на не менее чем одну внутреннюю функцию, у которой потом будет замыкание на внутреннюю область видимости обертки.

  <script async src="//jsfiddle.net/ekaterinasava/k46rantv/embed/js/"></script>

---

  <h2 class="post__small-heading">Пример AJAX на vanilla JavaScript</h2>

  По статье [An Example of AJAX with Vanilla Javascript](https://webdesign.tutsplus.com/tutorials/an-example-of-ajax-with-vanilla-javascript--cms-25763) by George Martsoukos (4 Feb 2016).

  Пример, использующий XMLHttpRequest API для инициализации AJAX запроса (все шаги описаны в комментариях кода):

  <script async src="//jsfiddle.net/ekaterinasava/ksq056cs/embed/"></script>
