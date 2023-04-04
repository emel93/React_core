# Раздел 3: React section
[Документация на русском](https://ru.reactjs.org/docs/getting-started.html)


## Блок 1: Таймер / Обратный отсчёт

Поработаем с таймерами и временем, освоим библиотеку компонентом [MUI](https://mui.com/)

### Что предстоит освоить
- Создание приложения с [create-react-app](https://create-react-app.dev/)
- Проверка через [eslint](https://eslint.org/).
- Автоформатирование [prettier](https://prettier.io/) (через плагин к [eslint](https://eslint.org/))
- Познакомится с библиотекой компонентов [MUI](https://mui.com/)

### Что предстоит сделать 
- Таймер
- Компоненту с обратным отсчётом

[Подробное описание задачи](./01-block/01-block.md)

### Темы для ревью

1. Окружение и зависимости
   - node.js
   - npm
   - create react app
   - prettier
   - eslint
   - MUI
   - styled components
   - React Developers Tools
2. React
   - JSX, условный рендеринг, работа с коллекциями
   - props, children
   - state
   - особенности работы с событиями
   - работа с формами
   - функциональные компоненты и namespaces
   - Vitrual DOM
   - Функции Lifecycle, использование интервалов
   - Ref
   - React.Fragment

### Дополнительные материалы
- [React документация](https://ru.reactjs.org/docs/getting-started.html)
- [Видеокурс](https://www.youtube.com/watch?v=GNrdg3PzpJQ)

#### npm vs yarn
Yarn - альтернативный пакетный менеджер для js. У него есть преимущества, но их немного - поэтому используем npm, как более распространенный.

#### Eslint + Prettier + Husky
[Стиль кода. Eslint. Husky.](https://www.youtube.com/playlist?list=PLlwtdxQXoJAvMeHYm-bMyTECOjKAXLFN0)  
Eslint - инструмент для статического анализа кода js. Позволяет выявить возможные ошибки на ранней стадии, унифицировать код и упростить решение merge-конфликтов.  
Конфиги для линтера и преттира: [.eslintrc.json](https://gist.github.com/jm-program/76c3faaf3cbf434c636d4620011d324d), [.prettierrc](https://gist.github.com/jm-program/8d91648662b9edd58897478062212b6c).  
Установку зависимостей смотрим [тут](https://github.com/airbnb/javascript/tree/master/packages/eslint-config-airbnb), дополнительно потребуются пакеты `babel-eslint`, `prettier`.  Файл `src/serviceWorker.js` добавляем в `.eslintignore`.  
Внимание: Могут быть конфликты между реакт-форматированием и prettier. Если линтеру не нравится что-то по переносам / отступам и это никак не исправить - правьте конфликтующее свойство в своем конфиге линтера и пишете ментору о проблеме.  
Prettier - автоформатирование кода с минимумом настроек. Решает споры "какой стиль кода лучше" (об это много копий сломано, малополезное занятие).  
[Husky](https://github.com/typicode/husky) - с помощью него настраиваем запуск линтера перед коммитом (pre-commit) - если проверка не проходит, коммитить не дает.

#### Деплой
На github pages, как деплоить - смотрим в документации Create React App.  
