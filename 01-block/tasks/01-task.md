# Подготовка окружения
1. Установка [node.js](https://nodejs.org/en) и [npm](https://www.npmjs.com/)
    1. Переходим на [node.js](https://nodejs.org/en)
    2. Устанавливаем "Recommended For Most Users" версию
    3. Откроем консоль и выполним команды:
    ```
        node -v
    ```
    ```
        npm -v
    ```
   Если команды отработали правильно, то вы увидите версии node.js и npm соответственно

## Создание и настройка react приложения

1. Чтобы создать react приложение будем пользоваться [Create React App](https://create-react-app.dev/) но с использованием кастомного темплейта [cra-template-typescript-styled](https://www.npmjs.com/package/cra-template-typescript-styled)
    1. Для этого установим темплейт
   ```
   npm i cra-template-typescript-styled
   ```
    2. И используем его
   ```
   npx create-react-app todo-list --template typescript-styled
   ```
2. Темплейт содержит зависимости на [Styled Components](https://styled-components.com/) и [Prettier](https://prettier.io/). Не забудьте поставить дополнительные плагины в вашей среде разработки, чтобы комфортно с ними работать.
3. Добавьте зависимости на [MUI](https://mui.com/) самостоятельно

## Создание компоненты Timer
1. Создайте компоненту таймер и добавьте: 
   - Заголовок с названием
   - Поле где будет отображаться текущее значение таймера
   - две кнопки
2. Напишите логику, которая будет выполняться по кликам на кнопку.

## Требования
1. Компонента таймер должна быть [мемоизирована](https://ru.reactjs.org/docs/react-api.html#reactmemo)
2. Обработчики событий (колбеки) должен быть [мемоизирован](https://ru.reactjs.org/docs/hooks-reference.html#usecallback)
3. Обязательное использование useSate
4. Используем Styled Components
5. Подключенный prettier, eslint и публикация на github pages.
