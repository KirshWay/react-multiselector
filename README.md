# React MultiSelector

Проект для изучения взаимодействия React + TypeScript и других особенностей React

- test view demo : https://kirshfein.github.io/react-multiselector/

Проект развернут на [Create React App](https://github.com/facebook/create-react-app).

## Скрипты

Устанавливаем пакеты: `npm ci`

**С полным соотвествием package-lock.json**

Запуск разработки: `npm run dev`

Запуск тестов: `npm run test`

Сборка релиза: `npm run build`

Проверка линтерами:

- `npm run lint`
- `npm run lint:unix` - для unix и linux систем

Проверка типизации TypeScript: `npm run type-check`

# Описание структуры проекта

Все более подробные описания содержатся в соответствующих директориях.

### Внутри директории `src`

`components` - React компоненты приложения
`components/ui` - многократно переиспользуемые базовые компоненты

`api` - содержит описание всех функций для запросов к api

`assets` - используемые файлы

`scripts` - переиспользуемые скрипты

`styles` - стили и scss переменные
`styles/mixins` - переиспользуемые компоненты стилей и миксины
`styles/modules` - переиспользуемые файлы стилей

`hooks` - содержит все кастомные хуки

`pages` - все компоненты шаблонов страниц

`store` - Redux хранилище (actions, reducers, types)

`types` - переиспользуемая типизация в приложении

`hooks` - переиспользуемые хуки в приложении

### Вне директории `src`

`.nginx` - настроки nginx

`.storybook` - настройки Storybook

### Дополнительно

- В проекте настроен докер контейнер с проксированием через nginx и открытием на 3030 порту.

- Добавлен шаблон `.gitlab-ci.yml` файла, которые необходимо переопределить для конкретного проекта.
