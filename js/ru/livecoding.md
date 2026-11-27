# JavaScript — Livecoding (RU)

20 задач от простого к сложному. Vanilla JS без библиотек, редактор без автокомплита, решение вслух. После решения — edge cases и тесты.

| ID | Задача | Что проверяют | Время, мин | Рейтинг | Компании |
|----|--------|---------------|-----------|---------|----------|
| js-081 | Реализуйте `Array.prototype.map`, `filter` и `reduce`. | `this`, sparse arrays, `thisArg`, reduce без initial value | 10–15 | FAANG | A, Ap |
| js-082 | `classnames`: объединить классы из строк, массивов и объектов с условиями. | Проверка типов, рекурсия | 15 | FAANG | M |
| js-083 | Flatten массива произвольной вложенности, с параметром `depth`. | Рекурсия и итеративная версия со стеком | 15 | FAANG | M, Ap |
| js-084 | Stack и Queue на JS; queue с O(1) dequeue. | Структуры данных, почему `shift()` — O(n) | 15 | FAANG | M |
| js-085 | `debounce` с методами `cancel` и `flush`. | Замыкания, `this`, аргументы, таймеры | 15–20 | FAANG | M, MS |
| js-086 | `throttle` с опциями leading и trailing. | Таймеры, состояние | 20 | FAANG | M |
| js-087 | `curry` для функции с произвольным числом аргументов. | `fn.length`, замыкания | 15 | FAANG | M |
| js-088 | `memoize` с кастомным resolver и ограничением размера (LRU). | Map, порядок ключей, память | 20 | FAANG | База |
| js-089 | EventEmitter: `on`, `emit` с аргументами, `once`, отписка через возвращаемый объект. | ООП, отписка во время emit | 20 | FAANG | M, MS |
| js-090 | `promisify`: превратить callback-функцию в промис. | Node-style callbacks, `this` | 10 | FAANG | A |
| js-091 | Полифилл `Promise.all`, затем `allSettled` и `any`. | Порядок результатов, пустой вход, не-промисы | 20 | FAANG | База |
| js-092 | Запуск промисов последовательно, затем пул с лимитом параллельности N. | Async-координация, очередь | 25 | FAANG | Ap |
| js-093 | `deepClone` с циклами, Map, Set, Date; затем `deepEqual`. | WeakMap, рекурсия, типы | 25 | FAANG | База |
| js-094 | Рекурсивно отфильтровать вложенный объект / санитизировать данные вложенной формы. | Рекурсия, трансформация данных, edge cases | 20 | FAANG | A |
| js-095 | Реализуйте `JSON.stringify`. | Типы, `undefined`, функции, `toJSON`, циклы | 30 | FAANG | A |
| js-096 | `getElementsByStyle(property, value)`: обход DOM с `getComputedStyle`. | Обход дерева, вычисленные стили | 20 | FAANG | A |
| js-097 | Два одинаковых DOM-дерева A и B и узел из A: найти соответствующий узел в B. | Путь до корня, O(depth) памяти | 20–25 | FAANG | M |
| js-098 | `clearAllTimeouts` и `render`, строящий DOM из вложенного объекта. | Monkey-patching, DOM API | 25 | FAANG | M |
| js-099 | Класс с асинхронной операцией (например, расшифровкой) и очередью callback-ов строго по порядку. | Состояние, очередь, гонки | 30 | FAANG | M |
| js-100 | API-клиент: retry (exponential backoff + jitter), throttling, отмена через `AbortController`, дедупликация запросов. | Дизайн API, async, надёжность | 40–45 | FAANG | MS |
