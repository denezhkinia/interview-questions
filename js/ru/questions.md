# JavaScript — Вопросы для собеседования (RU)

100 вопросов от простого к сложному: 80 теоретических (`js-001`–`js-080`) и 20 задач на livecoding (`js-081`–`js-100`, см. [livecoding.md](livecoding.md)).

**Компании** — где вопрос подтверждён отчётами кандидатов: **M** = Meta, **A** = Amazon, **Ap** = Apple, **MS** = Microsoft. **База** — типовой вопрос из общих топ-списков на темы, которые указывают все четыре компании.

## Уровень 1 · Основы (001–020)

| ID | Вопрос | Рейтинг | Компании |
|----|--------|---------|----------|
| js-001 | Какие типы данных есть в JS? Чем примитивы отличаются от объектов? | FAANG | База |
| js-002 | Чем отличаются `var`, `let` и `const`? | EPAM, FAANG | M, MS |
| js-003 | Чем `==` отличается от `===`? Когда нужен `Object.is`? | EPAM, FAANG | M, MS |
| js-004 | `null` и `undefined`: в чём разница? Почему `typeof null === 'object'`? | FAANG | База |
| js-005 | Что такое hoisting? Как он работает для функций и переменных? | EPAM, FAANG | База |
| js-006 | Что такое Temporal Dead Zone? | EPAM, FAANG | База |
| js-007 | Чем function declaration отличается от function expression? | FAANG | База |
| js-008 | Чем стрелочные функции отличаются от обычных? | FAANG | M |
| js-009 | Чем массив отличается от объекта? | FAANG | M |
| js-010 | Какие отличия ES5 от ES6+? Приведите примеры. | FAANG | Ap |
| js-011 | Как работает неявное приведение типов? Чему равны `[] + {}` и `'5' - 2`? | FAANG | База |
| js-012 | Truthy и falsy значения. Чем `??` отличается от `\|\|`? Как работает `?.`? | EPAM, FAANG | База |
| js-013 | Что такое `NaN` и как его надёжно проверить? | FAANG | База |
| js-014 | Spread и rest: в чём разница? Деструктуризация с дефолтами. | FAANG | База |
| js-015 | Передача по значению и по ссылке. Почему `const` не делает объект неизменяемым? | EPAM, FAANG | База |
| js-016 | Поверхностное и глубокое копирование. Чем плох `JSON.parse(JSON.stringify())`, что даёт `structuredClone`? | EPAM, FAANG | База |
| js-017 | Чем отличаются `map`, `forEach`, `filter` и `reduce`? | EPAM, FAANG | A, Ap |
| js-018 | Что делает `'use strict'`? Когда его лучше не включать? | EPAM, FAANG | A |
| js-019 | Что такое DOM? Чем `NodeList` отличается от `HTMLCollection`? | FAANG | M, MS |
| js-020 | `for (var i = 0; i < 3; i++) setTimeout(() => console.log(i))` — что выведется и как исправить? | FAANG | A |

## Уровень 2 · Средний (021–045)

| ID | Вопрос | Рейтинг | Компании |
|----|--------|---------|----------|
| js-021 | Что такое замыкание? Приведите практический пример. | EPAM, FAANG | M, A, MS |
| js-022 | Лексическое окружение и scope chain: как движок ищет переменную? | FAANG | База |
| js-023 | Как сделать приватное состояние через замыкание? Паттерн Module и IIFE. | FAANG | База |
| js-024 | Как определяется `this`? Четыре правила и их приоритет. | EPAM, FAANG | M |
| js-025 | Чем отличаются `call`, `apply` и `bind`? | EPAM, FAANG | M |
| js-026 | Почему метод, переданный как callback, теряет `this`? Как исправить? | FAANG | База |
| js-027 | Что такое прототип и цепочка прототипов? | EPAM, FAANG | M, MS |
| js-028 | Разница между `__proto__`, `prototype` и `Object.getPrototypeOf`. | FAANG | База |
| js-029 | Чем `class` в ES6 отличается от функции-конструктора? Что делает `new` по шагам? | FAANG | M |
| js-030 | Приватные поля `#field`, `static`, геттеры и сеттеры в классах. | FAANG | База |
| js-031 | Почему плохо расширять встроенные объекты (`Array.prototype`)? Что такое полифил? | FAANG | A, Ap |
| js-032 | Как устроен event loop: call stack, task queue, microtask queue? | EPAM, FAANG | A |
| js-033 | Макрозадачи и микрозадачи. Почему промис выполняется раньше `setTimeout(0)`? | EPAM, FAANG | A |
| js-034 | Угадайте порядок вывода: код с `setTimeout`, `Promise.then`, `queueMicrotask` и `await`. | FAANG | M, A |
| js-035 | Объясните промисы пятилетнему ребёнку. Какие у них состояния? | EPAM, FAANG | M |
| js-036 | Чем отличаются `Promise.all`, `allSettled`, `race` и `any`? | FAANG | База |
| js-037 | Как обрабатывать ошибки в async/await? Что будет с необработанным rejection? | EPAM, FAANG | База |
| js-038 | Callback hell: как его решают промисы и async/await? Когда `.then` уместнее `await`? | EPAM, FAANG | База |
| js-039 | Преимущества `Map` перед обычным объектом. | FAANG | M |
| js-040 | Преимущества `Set` перед массивом. Как `Set` сравнивает объекты? | FAANG | M |
| js-041 | Как работает распространение событий: capturing, target, bubbling? | FAANG | M |
| js-042 | Что такое event delegation и зачем оно нужно? | EPAM, FAANG | M |
| js-043 | Разница между `preventDefault`, `stopPropagation` и `stopImmediatePropagation`. | FAANG | База |
| js-044 | Debounce и throttle: сколько раз срабатывает scroll listener и как его разгрузить? | EPAM, FAANG | M, MS |
| js-045 | Функции высшего порядка, каррирование и частичное применение. | EPAM, FAANG | M |

## Уровень 3 · Продвинутый (046–065)

| ID | Вопрос | Рейтинг | Компании |
|----|--------|---------|----------|
| js-046 | Как отменить fetch? Как работает `AbortController`? | EPAM, FAANG | MS |
| js-047 | Race condition в автокомплите: как не показать устаревший ответ? | FAANG | MS, Ap |
| js-048 | Как выполнить массив промисов последовательно, а не параллельно? | FAANG | Ap |
| js-049 | Стратегии retry: exponential backoff, jitter, идемпотентность. | FAANG | MS |
| js-050 | Генераторы и итераторы. Как работает `Symbol.iterator`? | EPAM, FAANG | База |
| js-051 | Async-генераторы и `for await...of`: где они нужны (стриминг, пагинация)? | FAANG | База |
| js-052 | `Map` vs `WeakMap`, `Set` vs `WeakSet`. Зачем store с DOM-узлом в качестве ключа? | EPAM, FAANG | M |
| js-053 | Как работает сборщик мусора (mark-and-sweep)? | EPAM, FAANG | База |
| js-054 | Типичные утечки памяти во фронтенде и как найти их в DevTools. | EPAM, FAANG | База |
| js-055 | ES Modules vs CommonJS: статический анализ, tree shaking, live bindings, циклические зависимости. | EPAM, FAANG | База |
| js-056 | Как собрать и опубликовать npm-пакет? `exports`, dual ESM/CJS, `peerDependencies`. | FAANG | Ap |
| js-057 | Динамический `import()` и code splitting. | FAANG | База |
| js-058 | `Proxy` и `Reflect`: как на них строится реактивность (Vue 3, MobX)? | EPAM, FAANG | База |
| js-059 | Дескрипторы свойств, `Object.freeze`, `seal`, `preventExtensions`. | FAANG | База |
| js-060 | `Symbol`: зачем нужен и какие есть well-known symbols? | FAANG | База |
| js-061 | `0.1 + 0.2`: как избежать проблем с дробными числами? Когда нужен `BigInt`? | EPAM, FAANG | База |
| js-062 | Что происходит, когда вводишь URL в браузере и сайт загружается? | FAANG | A |
| js-063 | `<script>`: чем отличаются `async`, `defer` и `type="module"`? | FAANG | База |
| js-064 | Хранилища браузера: cookies, `localStorage`, `sessionStorage`, IndexedDB. | FAANG | Ap |
| js-065 | `requestAnimationFrame` vs `requestIdleCallback` vs `setTimeout`. | EPAM, FAANG | База |

## Уровень 4 · Эксперт (066–080)

| ID | Вопрос | Рейтинг | Компании |
|----|--------|---------|----------|
| js-066 | Как браузер приоритизирует промисы, `setTimeout` и рендеринг? Влияние на производительность UI. | FAANG | A |
| js-067 | Можно ли повесить страницу микрозадачами? Рекурсивный `Promise.then` vs рекурсивный `setTimeout`. | FAANG | База |
| js-068 | Critical rendering path: DOM, CSSOM, layout, paint, composite. | FAANG | Ap |
| js-069 | Reflow и layout thrashing. Как батчить чтения и записи DOM? | FAANG | База |
| js-070 | Как V8 оптимизирует код: hidden classes, inline caches, JIT, deoptimization? | FAANG | База |
| js-071 | Поколения GC в V8: young/old generation, scavenge, паузы. | FAANG | База |
| js-072 | `WeakRef` и `FinalizationRegistry`: когда применять, а когда нет? | FAANG | База |
| js-073 | XSS и CSRF: защита на стороне JS (CSP, sanitization, SameSite). | FAANG | Ap, A |
| js-074 | CORS: preflight, credentials; почему это защита браузера, а не сервера. | FAANG | Ap |
| js-075 | Web Workers, SharedArrayBuffer, `Atomics`: вынос вычислений из main thread. | FAANG | База |
| js-076 | Service Worker: жизненный цикл и стратегии кэширования. | FAANG | База |
| js-077 | Streams API и стриминг ответа LLM: `ReadableStream`, SSE, backpressure. | FAANG | База (для AI-роли) |
| js-078 | Как выбор структуры данных влияет на производительность UI (Map, Set, Tree, нормализация состояния)? | FAANG | A |
| js-079 | Как спроектировать JS SDK для внешних потребителей: контракты, ошибки, rate limiting, версионирование? | FAANG | MS |
| js-080 | Как измерить и улучшить Core Web Vitals (LCP, INP, CLS) средствами JS? | FAANG | База |
