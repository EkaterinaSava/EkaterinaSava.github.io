---
layout: post
title: Разработка в блокчейне Ethereum
---

Так как для меня знакомство с программированием блокчейна в новинку, буду записывать всякие базовые вещи, вроде полезных ссылок, где и что скачать, консольные команды и подобное.

---

__Настройка окружения__

1. Установка Geth (Go Ethereum — Official Go implementation of the Ethereum protocol)

  — инструкция по [установке Geth](https://github.com/ethereum/go-ethereum/wiki/Installation-Instructions-for-Mac) на MacOS
  — если кратко, то

  1. первая команда переключает в ветку brew, где есть ethereum

  2. вторая - устанавливает его

  {% highlight %}
  brew tap ethereum/ethereum
  brew install ethereum
  {% endhighlight %}

  —  после установки для запуска Geth со всеми необходимыми флагами прописываем в консоли:

  ```
  geth --dev --rpc --rpcaddr "0.0.0.0" --rpccorsdomain "*" --rpcapi "admin,debug,miner,shh,txpool,personal,eth,net,web3" --datadir "~/NewChain/firstTest" --networkid 1337 console
  ```

  (остановить его можно, напечатав в консоли `exit`)

  — затем необходимо создать новый аккаунт (не выходя из запущенного Geth)

  ```
  personal.newAccount('123')
  ```

  создаем 2 аккаунта, прописав эту команду 2 раза (рекомендация: использовать один и тот же пароль для всех аккаунтов)

  важно! потеря пароля от аккаунта лишает доступа к аккаунту, возможности восстановить его нет

2. Установка Mist

---
