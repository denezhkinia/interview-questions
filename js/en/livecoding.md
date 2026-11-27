# JavaScript — Livecoding (EN)

20 tasks from easy to hard. Vanilla JS, no libraries, no autocomplete, think out loud. Afterwards cover edge cases and tests.

| ID | Task | What it tests | Time, min | Rating | Companies |
|----|------|---------------|-----------|--------|-----------|
| js-081 | Implement `Array.prototype.map`, `filter`, and `reduce`. | `this`, sparse arrays, `thisArg`, reduce without an initial value | 10–15 | FAANG | A, Ap |
| js-082 | `classnames`: join class names from strings, arrays, and conditional objects. | Type checks, recursion | 15 | FAANG | M |
| js-083 | Flatten an arbitrarily nested array, with a `depth` parameter. | Recursion and an iterative stack-based version | 15 | FAANG | M, Ap |
| js-084 | Stack and Queue in JS; a queue with O(1) dequeue. | Data structures, why `shift()` is O(n) | 15 | FAANG | M |
| js-085 | `debounce` with `cancel` and `flush` methods. | Closures, `this`, arguments, timers | 15–20 | FAANG | M, MS |
| js-086 | `throttle` with leading and trailing options. | Timers, state | 20 | FAANG | M |
| js-087 | `curry` for a function with any number of arguments. | `fn.length`, closures | 15 | FAANG | M |
| js-088 | `memoize` with a custom resolver and a size limit (LRU). | Map key order, memory | 20 | FAANG | Baseline |
| js-089 | EventEmitter: `on`, `emit` with args, `once`, unsubscribe via a returned object. | OOP, unsubscribing during emit | 20 | FAANG | M, MS |
| js-090 | `promisify`: turn a callback-style function into a promise. | Node-style callbacks, `this` | 10 | FAANG | A |
| js-091 | Polyfill `Promise.all`, then `allSettled` and `any`. | Result order, empty input, non-promises | 20 | FAANG | Baseline |
| js-092 | Run promises sequentially, then a pool with a concurrency limit N. | Async coordination, queueing | 25 | FAANG | Ap |
| js-093 | `deepClone` handling cycles, Map, Set, Date; then `deepEqual`. | WeakMap, recursion, types | 25 | FAANG | Baseline |
| js-094 | Recursively filter a nested object / sanitize nested form data. | Recursion, data transformation, edge cases | 20 | FAANG | A |
| js-095 | Implement `JSON.stringify`. | Types, `undefined`, functions, `toJSON`, cycles | 30 | FAANG | A |
| js-096 | `getElementsByStyle(property, value)`: walk the DOM with `getComputedStyle`. | Tree traversal, computed styles | 20 | FAANG | A |
| js-097 | Two identical DOM trees A and B and a node in A: find the matching node in B. | Path to root, O(depth) memory | 20–25 | FAANG | M |
| js-098 | `clearAllTimeouts` and a `render` that builds DOM from a nested object. | Monkey-patching, DOM API | 25 | FAANG | M |
| js-099 | A class with an async operation (e.g. decryption) and a callback queue processed strictly in order. | State, queueing, races | 30 | FAANG | M |
| js-100 | API client: retry (exponential backoff + jitter), throttling, cancellation via `AbortController`, request deduplication. | API design, async, reliability | 40–45 | FAANG | MS |
