---
layout: post
title: Разработка блокчейна с нуля на JavaScript
---

Пытаюсь разобраться и не умереть `.__.`

С нуля по шагам.

---

<h2 class="post__small-heading">Network Stack</h2>

В этом ключе нас интересуют `gossip-протоколы`

  * нет единой точки централизации, благодаря чему система

      — устойчива

      — и масштабируема

      — такая сеть может передавать сообщения пушем / пулом / гибридно

Каждый член blockchain-сети является нодой    

  * full-node (полная нода) – это член сети имеющий у себя весь блокчейн и способный валидировать блоки

  * рут / корень сети отвечает на вопрос, где остальные ноды

      — он может быть полной нодой (что является дорогостоящим)

      — или листом возможных членов сети, отвечающим на вопрос куда коннектиться за информацией

И здесь нас начинают интересовать `TCP/UDP-протоколы`

---

__Цель (задание) на данном этапе:__

* пишем gossip-ноду

* например, мы получили от нашего рута 4 порта (на самом деле, в реальной жизни, он скорее отдаст нам алреса других рутов и по идее каждый член сети доожен вести себя как рут – уметь отдваать список нод) и нам надо выбрать к чему коннектиться

* для этого нам необходимо придумать алгоритм выбора пиров – к примеру, каждая нода будет передавать сообщение 3 ближайщим другим пирам (а нашем случае, будет в качестве идентификаторов использовать порты) в большую сторону:

    — так к примеру 100 порт должен приконнектиться к 101, 102, 103;

    — 101 – к 100, 102, 103; ... ;

    — 103 — к 102, 104,105 и т.д.

* так мы получаем сеть, в которой понятным образом выбирается пир, что позволяет достаточно равномерно распределить нагрузку по сети

* дальше мы решаем как будем распространять сообщения: мы договариваемся, что это будет gossip-протокол с пушем, то етсь когда придет сообщения, мы будем сразу же делать пуш в сеть

* в первую очередь нам нужно имплементировать коннект к руту и забор оттуда списка портов, а дальше - коннект по ближайщим 3 портам (как мы решили это в алгоритме)

* далее основная суть gossip-a – посылка сообщений: то есть нужно сделать метод, который посылает сообщение всем своим пирам, после того как установлен connection

* если вы являетесь пиром и принимаете сообщение, то

    — не отправляете его обратно

    — распространяете это сообщение только тем пирам, которые его еще не получили (опираясь на изначальный алгоритм выбора пиров)

* нужно сделать console.log() что сообщение пришло  


---
