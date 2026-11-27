# JavaScript — Interview Questions (EN)

100 questions ordered from easy to hard: 80 theory questions (`js-001`–`js-080`) and 20 livecoding tasks (`js-081`–`js-100`, see [livecoding.md](livecoding.md)).

**Companies** — where candidate reports confirm the question: **M** = Meta, **A** = Amazon, **Ap** = Apple, **MS** = Microsoft. **Baseline** — a common question from general top lists, on topics all four companies list.

## Level 1 · Basics (001–020)

| ID | Question | Rating | Companies |
|----|----------|--------|-----------|
| js-001 | What data types exist in JS? How do primitives differ from objects? | FAANG | Baseline |
| js-002 | What is the difference between `var`, `let`, and `const`? | EPAM, FAANG | M, MS |
| js-003 | What is the difference between `==` and `===`? When do you need `Object.is`? | EPAM, FAANG | M, MS |
| js-004 | `null` vs `undefined`: what is the difference? Why is `typeof null === 'object'`? | FAANG | Baseline |
| js-005 | What is hoisting? How does it work for functions and variables? | EPAM, FAANG | Baseline |
| js-006 | What is the Temporal Dead Zone? | EPAM, FAANG | Baseline |
| js-007 | What is the difference between a function declaration and a function expression? | FAANG | Baseline |
| js-008 | How do arrow functions differ from regular functions? | FAANG | M |
| js-009 | What is the difference between an array and an object? | FAANG | M |
| js-010 | What are the differences between ES5 and ES6+? Give examples. | FAANG | Ap |
| js-011 | How does implicit type coercion work? What are `[] + {}` and `'5' - 2`? | FAANG | Baseline |
| js-012 | Truthy and falsy values. How does `??` differ from `\|\|`? How does `?.` work? | EPAM, FAANG | Baseline |
| js-013 | What is `NaN` and how do you check for it reliably? | FAANG | Baseline |
| js-014 | Spread vs rest: what is the difference? Destructuring with defaults. | FAANG | Baseline |
| js-015 | Pass by value vs by reference. Why doesn't `const` make an object immutable? | EPAM, FAANG | Baseline |
| js-016 | Shallow vs deep copy. What is wrong with `JSON.parse(JSON.stringify())`, and what does `structuredClone` give you? | EPAM, FAANG | Baseline |
| js-017 | What is the difference between `map`, `forEach`, `filter`, and `reduce`? | EPAM, FAANG | A, Ap |
| js-018 | What does `'use strict'` do? When is it better not to use it? | EPAM, FAANG | A |
| js-019 | What is the DOM? How does `NodeList` differ from `HTMLCollection`? | FAANG | M, MS |
| js-020 | `for (var i = 0; i < 3; i++) setTimeout(() => console.log(i))` — what is logged and how do you fix it? | FAANG | A |

## Level 2 · Intermediate (021–045)

| ID | Question | Rating | Companies |
|----|----------|--------|-----------|
| js-021 | What is a closure? Give a practical example. | EPAM, FAANG | M, A, MS |
| js-022 | Lexical environment and scope chain: how does the engine resolve a variable? | FAANG | Baseline |
| js-023 | How do you create private state with a closure? The Module pattern and IIFE. | FAANG | Baseline |
| js-024 | How is `this` determined? The four rules and their precedence. | EPAM, FAANG | M |
| js-025 | What is the difference between `call`, `apply`, and `bind`? | EPAM, FAANG | M |
| js-026 | Why does a method passed as a callback lose `this`? How do you fix it? | FAANG | Baseline |
| js-027 | What is a prototype and the prototype chain? | EPAM, FAANG | M, MS |
| js-028 | The difference between `__proto__`, `prototype`, and `Object.getPrototypeOf`. | FAANG | Baseline |
| js-029 | How does an ES6 `class` differ from a constructor function? What does `new` do step by step? | FAANG | M |
| js-030 | Private `#fields`, `static`, getters and setters in classes. | FAANG | Baseline |
| js-031 | Why is extending built-ins (`Array.prototype`) a bad idea? What is a polyfill? | FAANG | A, Ap |
| js-032 | How does the event loop work: call stack, task queue, microtask queue? | EPAM, FAANG | A |
| js-033 | Macrotasks vs microtasks. Why does a promise run before `setTimeout(0)`? | EPAM, FAANG | A |
| js-034 | Predict the output order: code with `setTimeout`, `Promise.then`, `queueMicrotask`, and `await`. | FAANG | M, A |
| js-035 | Explain promises to a 5-year-old. What states does a promise have? | EPAM, FAANG | M |
| js-036 | What is the difference between `Promise.all`, `allSettled`, `race`, and `any`? | FAANG | Baseline |
| js-037 | How do you handle errors in async/await? What happens to an unhandled rejection? | EPAM, FAANG | Baseline |
| js-038 | Callback hell: how do promises and async/await solve it? When is `.then` better than `await`? | EPAM, FAANG | Baseline |
| js-039 | Advantages of `Map` over a plain object. | FAANG | M |
| js-040 | Advantages of `Set` over an array. How does `Set` compare objects? | FAANG | M |
| js-041 | How does event propagation work: capturing, target, bubbling? | FAANG | M |
| js-042 | What is event delegation and why is it useful? | EPAM, FAANG | M |
| js-043 | The difference between `preventDefault`, `stopPropagation`, and `stopImmediatePropagation`. | FAANG | Baseline |
| js-044 | Debounce vs throttle: how often does a scroll listener fire and how do you relieve it? | EPAM, FAANG | M, MS |
| js-045 | Higher-order functions, currying, and partial application. | EPAM, FAANG | M |

## Level 3 · Advanced (046–065)

| ID | Question | Rating | Companies |
|----|----------|--------|-----------|
| js-046 | How do you cancel a fetch? How does `AbortController` work? | EPAM, FAANG | MS |
| js-047 | Race condition in autocomplete: how do you avoid showing a stale response? | FAANG | MS, Ap |
| js-048 | How do you run an array of promises sequentially instead of in parallel? | FAANG | Ap |
| js-049 | Retry strategies: exponential backoff, jitter, idempotency. | FAANG | MS |
| js-050 | Generators and iterators. How does `Symbol.iterator` work? | EPAM, FAANG | Baseline |
| js-051 | Async generators and `for await...of`: where are they useful (streaming, pagination)? | FAANG | Baseline |
| js-052 | `Map` vs `WeakMap`, `Set` vs `WeakSet`. Why a store keyed by DOM nodes? | EPAM, FAANG | M |
| js-053 | How does garbage collection work (mark-and-sweep)? | EPAM, FAANG | Baseline |
| js-054 | Common frontend memory leaks and how to find them in DevTools. | EPAM, FAANG | Baseline |
| js-055 | ES Modules vs CommonJS: static analysis, tree shaking, live bindings, circular dependencies. | EPAM, FAANG | Baseline |
| js-056 | How do you build and publish an npm package? `exports`, dual ESM/CJS, `peerDependencies`. | FAANG | Ap |
| js-057 | Dynamic `import()` and code splitting. | FAANG | Baseline |
| js-058 | `Proxy` and `Reflect`: how is reactivity built on them (Vue 3, MobX)? | EPAM, FAANG | Baseline |
| js-059 | Property descriptors, `Object.freeze`, `seal`, `preventExtensions`. | FAANG | Baseline |
| js-060 | `Symbol`: why does it exist and what are well-known symbols? | FAANG | Baseline |
| js-061 | `0.1 + 0.2`: how do you avoid floating-point issues? When do you need `BigInt`? | EPAM, FAANG | Baseline |
| js-062 | What happens when you type a URL into the browser and the site loads? | FAANG | A |
| js-063 | `<script>`: how do `async`, `defer`, and `type="module"` differ? | FAANG | Baseline |
| js-064 | Browser storage: cookies, `localStorage`, `sessionStorage`, IndexedDB. | FAANG | Ap |
| js-065 | `requestAnimationFrame` vs `requestIdleCallback` vs `setTimeout`. | EPAM, FAANG | Baseline |

## Level 4 · Expert (066–080)

| ID | Question | Rating | Companies |
|----|----------|--------|-----------|
| js-066 | How does the browser prioritize promises, `setTimeout`, and rendering? Impact on UI performance. | FAANG | A |
| js-067 | Can microtasks freeze a page? Recursive `Promise.then` vs recursive `setTimeout`. | FAANG | Baseline |
| js-068 | Critical rendering path: DOM, CSSOM, layout, paint, composite. | FAANG | Ap |
| js-069 | Reflow and layout thrashing. How do you batch DOM reads and writes? | FAANG | Baseline |
| js-070 | How does V8 optimize code: hidden classes, inline caches, JIT, deoptimization? | FAANG | Baseline |
| js-071 | V8 generational GC: young/old generation, scavenge, pauses. | FAANG | Baseline |
| js-072 | `WeakRef` and `FinalizationRegistry`: when to use them and when not? | FAANG | Baseline |
| js-073 | XSS and CSRF: client-side defenses (CSP, sanitization, SameSite). | FAANG | Ap, A |
| js-074 | CORS: preflight, credentials; why it protects the browser, not the server. | FAANG | Ap |
| js-075 | Web Workers, SharedArrayBuffer, `Atomics`: moving work off the main thread. | FAANG | Baseline |
| js-076 | Service Worker: lifecycle and caching strategies. | FAANG | Baseline |
| js-077 | Streams API and streaming LLM responses: `ReadableStream`, SSE, backpressure. | FAANG | Baseline (AI role) |
| js-078 | How does the choice of data structure affect UI performance (Map, Set, Tree, state normalization)? | FAANG | A |
| js-079 | How do you design a JS SDK for external consumers: contracts, errors, rate limiting, versioning? | FAANG | MS |
| js-080 | How do you measure and improve Core Web Vitals (LCP, INP, CLS) with JS? | FAANG | Baseline |
