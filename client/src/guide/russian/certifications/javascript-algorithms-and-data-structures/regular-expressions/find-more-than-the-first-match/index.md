---
title: Find More Than the First Match
localeTitle: Найдите больше, чем первый матч
---
## Найдите больше, чем первый матч

Если у вас несколько строк вашего регулярного выражения внутри строки, вы можете получить функцию `match()` чтобы обнаружить все из них. Просто пометите флаг `g` в конце вашего регулярного выражения! Это то, что вы делаете в этой задаче.

## Подсказка 1:

Измените регулярное выражение так, чтобы оно обнаруживало слово «мерцание».

## Подсказка 2:

Вы можете добавить несколько тегов в регулярное выражение! Например, регулярное выражение, которое обнаруживает множественные вхождения и обнаруживает независимо от случая, может быть структурировано как `gi` или `ig` .

## Оповещение о спойлере - решение впереди!

## Решение

```javascript
let twinkleStar = "Twinkle, twinkle, little star"; 
 let starRegex = /twinkle/gi; 
 let result = twinkleStar.match(starRegex); 

```