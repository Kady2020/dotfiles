# Dotfiles

Файлы моих настроек, которые лежат в корне каждого проекта.

## [.editorconfig](http://editorconfig.org)

- Кодировка utf-8.
- Отступы пробелами.
- Ширина отступа равна 2 пробелам.
- [Перевод строки](https://ru.wikipedia.org/wiki/%D0%9F%D0%B5%D1%80%D0%B5%D0%B2%D0%BE%D0%B4_%D1%81%D1%82%D1%80%D0%BE%D0%BA%D0%B8) `LF`.
- В конце каждой строки убираются лишние пробелы.
- В конце файла добавляется пустая строка.

## .gitignore

- Логи (`logs`, `*.log`).
- Папки зависимостей (`node_modules`, `bower_components`).
- Генерируемые файлы (`dist`, `_site`).

## [.htmlhintrc](http://htmlhint.com)

- Атрибуты в нижнем регистре.
- Значения атрибутов в двойных кавычках.
- Экранирование специальных символов.
- Парные теги всегда должны закрываться.
- Уникальные `id`.
- `src` не должен быть пустым.
- Атрибуты не должны дублироваться.
- Обязательно должен быть заполнен тег `title`.
- Теги в нижнем регистре.
- У картинок обязательно должен быть атрибут `alt`.

## [.postcss-sorting.json](https://github.com/lysyi3m/atom-postcss-sorting)

- Неизвестные свойства вниз.
- Удалять все пустые строки.
- Вставлять пустую строку перед вложенными свойствами.
- Вставлять пустую строку перед вложенными @-свойствами.
- Сортировка свойств по моему принципу.

## [.stylelintrc](https://stylelint.io)

Скопированы и подправлены стандартные [stylelint-config-recommended](https://github.com/stylelint/stylelint-config-recommended) и [stylelint-config-standard](https://github.com/stylelint/stylelint-config-standard).

Подправлено:

- edit `"no-descending-specificity": true` to `null`
- edit `"no-duplicate-selectors": true` to `null`
- edit `"declaration-colon-newline-after": null,`
- edit `"value-list-comma-newline-after": null`
- add `"font-family-name-quotes": "always-where-required"`
- add `"string-quotes": "double"`
- add `"shorthand-property-no-redundant-values": true`

## package.json

Минимальные значения:

```json
{
  "name": "dotfiles",
  "version": "0.1.0"
}
```

- `browserslist` для автопрефиксера и других инструментов.

## [.prettierrc](https://prettier.io/)

- Ширина строки `80`.
- Ширина отступа равна 2 пробелам.
- Отступы пробелами.
- `;` в конце строк всегда.
- Одинарные кавычки в JS. Чтобы в CSS были двойные, нужно настроить в stylelint.
- Запятые по ES5.
- Пробелы в фигурных скобках `{ foo: bar }`.
- Скобку в JSX оставлять на той же строке.
- Без скобок стрелочные функции `x => x`.

## [.browserslistrc](https://github.com/browserslist/browserslist)

- `> 1%`
- `last 2 versions`
- `not ie <= 8`
