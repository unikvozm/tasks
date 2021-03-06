# RSS Игра в пятнашки

### Deadline:

## Задание
Вам нужно реализовать классическую игру [пятнашки](https://ru.wikipedia.org/wiki/Игра_в_15)

### Правила игры
`Игра представляет собой набор одинаковых квадратных костяшек с нанесёнными числами, заключённых в квадратную коробку. Длина стороны коробки в четыре раза больше длины стороны костяшек для набора из 15 элементов, соответственно в коробке остаётся незаполненным одно квадратное поле. Цель игры — перемещая костяшки по коробке, добиться упорядочивания их по номерам, желательно сделав как можно меньше перемещений`

### Приблизительный внешний вид
![](https://i.imgur.com/AFOXNmG.png)

### Основные функциональные требования
  `Базовые(обязательные):`
  - дизайн на свое усмортрение, но должен быть адаптивный (декстоп, планшет, мобильный), при переходе между версиями все должно отображаться корректно, должен присутствовать весь функционал, ничего не должно пропадать, уезжать за пределы экрана. Допустимо изменить внешний вид для мобильной версии (например спрятать кнопки в бургер-меню)
  - изначально файл index.html должен быть пустой (все необходимые элементы генерируются с использованием JS)
  - размер поля по умолчанию 4х4
  - cостояние игрового поля генерируется случайным образом забивается числами при запуске новой игры цифры перемешиваются 
  - при клике по фишке, стоящей рядом с пустой клеткой, фишка перемещается на место пустой клетки
  - реализовать возможности начать игру заново без перезагрузки страницы
  - реализовать отображение продолжительности игры в минутах и секундах "##:##" и колличество ходов
 - использование [eslint (eslint-config-airbnb-base)](https://eslint.org/), [webpack](https://webpack.js.org/)
  - реализовать возможности сохранения игры (например с помощью localStorage), что бы при перезагрузке страницы иметь возможность продолжить с тогоже места где остановился

  `дополнительные(для получения дополнительных баллов):`
  - реализовать возможность выбора размера поля: от 3х3 до 8х8
  - реализовать анимация перемещение пятнашек на поле
  - при решении игры надо выводить сообщение «Ура! Вы решили головоломку за #:## и N ходов»
  - лучших 10 результатов сохраняется в таблицу рекордов и их можно каким либо образом посмотреть (например по нажатию кнопки)
  - использование [TypeScript](https://www.typescriptlang.org/)

### Тенические требования
- должно работать в Chrome последней версии
- задание должно использовать Canvas
- покрытие кода unit-tests ( [Jest](https://jestjs.io/), [Mocha](https://mochajs.org/), [Chai](https://www.chaijs.com/) )

### Требования к коммитам, PR, репозиторию

- [Общие требования из этапа 2](https://github.com/rolling-scopes-school/docs/blob/master/stage2-tasks-requirements.md)
- рабочее приложение должно быть размещено на GitHub Pages (https://pages.github.com/), это произойдет автоматически при создании `gh-pages` бранча. После чего страница будет доступна по адресу вида - https://your-github-account.github.io/name-repository

## Критерий оценки:
**Максимальный бал за задание: 145**

`минимальный набор:`
- pеализована генерация DOM-элементов и index.html пустой изначально: `+10`
- cостояние игрового поля генерируется случайным образом: `+10`
- реализован выбор размера поля: `+10`
- реализовано отображение времени игры и колличества ходов: `+5`

`стандартный набор:`
- реализовано сохранение игры и 10 лучших результатов с иcпользованием LocalStorage: `+5`
- использовались в коде фишеки ES6 и более (promises, classes, деструктуризацию и тд): `+15`

`повышенный набор:`
- реализована анимация перемещения пятнашек на поле: `+15`
- unit-tests setup + протестировано 5 функций: `+15`
- реализовано сохранения игры и 10 лучших результатов с иcпользованием [node.js](https://nodejs.org/en/)/[express](http://expressjs.com/)/[mongodb](https://www.mongodb.com/): `+15`

`технические требования:`
- использован eslint, webpack: `+10`
- использован [TypeScript](https://www.typescriptlang.org/): `+15`
- выполены требования к репозиторию, коммитам и PR: `+10`

`штрафы:`
- ошибки или предупреждения eslint-config-airbnb-base: `-15`
- до `-50` баллов за нарушение [stage2-tasks-requirements](https://github.com/rolling-scopes-school/docs/blob/master/stage2-tasks-requirements.md)

## Кто выполянет проверку задания?
Ваш ментор.

## Полезные ссылки

- [eslint](https://eslint.org/)
- [TypeScript](https://www.typescriptlang.org/)
- [Canvas](https://developer.mozilla.org/en/docs/Web/API/Canvas_API/Tutorial)
- [Game Canvas](https://www.w3schools.com/graphics/game_canvas.asp)
- [node.js](https://nodejs.org/en/), [express](http://expressjs.com/), [mongodb](https://www.mongodb.com/)
- [Jest](https://jestjs.io/), [Mocha](https://mochajs.org/), [Chai](https://www.chaijs.com/)
- [Стрим YouTube Bootstrap( пример подключения webpack, eslint, написания unit-tests)](https://www.youtube.com/watch?v=1Nk09Z4ca4A&list=PLe--kalBDwjj81fKdWlvpLsizajSAK-lh&index=32)
- [Стрим RSS live coding: game boostrap](https://www.youtube.com/watch?v=pz9SihVxjo8&list=PLe--kalBDwjiBYlF6OivjURvvJg58tYY2&index=8)