# Javascript ծրագրավորման լեզվի հարցազրույցի հարցեր և պատասխաններ

> Սեղմեք :star: եթե ձեզ դուր է գալիս. 
> Եթե ունեք ձեր հարցերը, կխնդրենք բացել Pull Request այդ հարցերը ծրագրում ավելացնելու համար.

## Բովանդակություն

| No. | Հարցեր                                                                                           |
|-----|--------------------------------------------------------------------------------------------------|
| 1   | [Որոնք են JavaScript լեզվում Primitive տիպերը?](#որոնք-են-javascript-լեզվում-primitive-տիպերը)     |
| 2   | [Ինչ է undefined և undeclared?](#ինչ-է-undefined-և-undeclared)                                   |
| 3   | [Ինչի համար է typeof օպերատորը?](#ինչի-համար-է-typeof-օպերատորը)                                  |
| 4   | [Ինչ է NAN և ինչպես կարող ենք հասկանալ, որ արժեքը NAN է?](#ինչ-է-nan-և-ինչպես-կարող-ենք-հասկանալ-որ-արժեքը-nan-է) |
| 5   | [Ինչ է toString և ինչպես կարող ենք այն օգտագործել?](#ինչ-է-tostring-և-ինչպես-կարող-ենք-այն-օգտագործել) |
| 6   | [Ինչ է toNumber և ինչպես կարող ենք այն օգտագործել?](#ինչ-է-tonumber-և-ինչպես-կարող-ենք-այն-օգտագործել) |
| 7   | [Ինչ է toBoolean և ինչպես կարող ենք այն օգտագործել?](#ինչ-է-toboolean-և-ինչպես-կարող-ենք-այն-օգտագործել) |
| 8   | [Ինչ է Coercion և ինչպես կարող ենք այն օգտագործել?](#ինչ-է-coercion-և-ինչպես-կարող-ենք-այն-օգտագործել) |
| 9   | [Ինչ է boxing-ը?](#ինչ-է-boxing-ը)                                                               |
| 10  | [Ինչ են double equal (==) և triple equal (===) օպերատորները?](#ինչ-են-double-equal--և-triple-equal--օպերատորները) |
| 11  | [Ինչ է hoisting-ը JavaScript-ում?](#ինչ-է-hoisting-ը-javascript-ում)                              |
| 12  | [Ինչ տարբերություն կա let, const և var միջև?](#ինչ-տարբերություն-կա-let-const-և-var-միջև)           |
| 13  | [Ինչ է closure-ը JavaScript-ում?](#ինչ-է-closure-ը-javascript-ում)                                |
| 14  | [Ինչպես է աշխատում "this" բանալի բառը JavaScript-ում?](#ինչպես-է-աշխատում-this-բանալի-բառը-javascript-ում) |
| 15  | [Ինչ է Event Loop-ը JavaScript-ում?](#ինչ-է-event-loop-ը-javascript-ում)                          |
| 16  | [Ինչ է debounce-ը և throttle-ը JavaScript-ում?](#ինչ-է-debounce-ը-և-throttle-ը-javascript-ում)    |
| 17  | [Ինչ է `Promise`-ը և ինչպես է այն աշխատում?](#ինչ-է-promise-ը-և-ինչպես-է-այն-աշխատում)            |
| 18  | [Ինչպես է աշխատում async/await-ը JavaScript-ում?](#ինչպես-է-աշխատում-asyncawait-ը-javascript-ում) |
| 19  | [Ինչ է DOM-ը և ինչ տարբերություն կա HTML-ի և DOM-ի միջև?](#ինչ-է-dom-ը-և-ինչ-տարբերություն-կա-html-ի-և-dom-ի-միջև) |
| 20  | [Ինչ է ES6 մոդուլը և ինչպես է այն աշխատում?](#ինչ-է-es6-մոդուլը-և-ինչպես-է-այն-աշխատում)           |
| 21  | [Ինչ է JavaScript-ում call, apply, bind մեթոդները?](#ինչ-է-javascript-ում-call-apply-bind-մեթոդները) |
| 22  | [Ինչ է `map`, `filter` և `reduce` մեթոդները JavaScript-ում?](#ինչ-է-map-filter-և-reduce-մեթոդները-javascript-ում) |
| 23  | [Ինչ է տարբերություն shallow copy-ի և deep copy-ի միջև?](#ինչ-է-տարբերություն-shallow-copy-ի-և-deep-copy-ի-միջև) |
| 24  | [Ինչ է `prototype`-ը JavaScript-ում?](#ինչ-է-prototype-ը-javascript-ում)                         |
| 25  | [Ինչ է JavaScript-ում event bubbling-ը և event capturing-ը?](#ինչ-է-javascript-ում-event-bubbling-ը-և-event-capturing-ը) |
| 26  | [Ինչ է IIFE (Immediately Invoked Function Expression)?](#ինչ-է-iife-immediately-invoked-function-expression) |
| 27  | [Ինչ է JavaScript-ում WeakMap-ը և WeakSet-ը?](#ինչ-է-javascript-ում-weakmap-ը-և-weakset-ը)         |
| 28  | [Ինչ է Execution Context-ը JavaScript-ում?](#ինչ-է-execution-context-ը-javascript-ում)           |
| 29  | [Ինչ է Scope-ը և Scope Chain-ը JavaScript-ում?](#ինչ-է-scope-ը-և-scope-chain-ը-javascript-ում)   |
| 30  | [Ինչ է JavaScript-ի strict mode-ը?](#ինչ-է-javascript-ի-strict-mode-ը)                           |
| 31  | [Ինչ է CORS-ը և ինչու է այն կարևոր?](#ինչ-է-cors-ը-և-ինչու-է-այն-կարևոր)                         |
| 32  | [Ինչ է Module Pattern-ը JavaScript-ում?](#ինչ-է-module-pattern-ը-javascript-ում)                 |
| 33  | [Ինչ տարբերություն կա mutable և immutable օբյեկտների միջև?](#ինչ-տարբերություն-կա-mutable-և-immutable-օբյեկտների-միջև) |
| 34  | [Ինչպես են աշխատում setters և getters JavaScript-ում?](#ինչպես-են-աշխատում-setters-և-getters-javascript-ում) |
| 35  | [Ինչ է տարբերություն function declaration-ի և function expression-ի միջև?](#ինչ-է-տարբերություն-function-declaration-ի-և-function-expression-ի-միջև) |
| 36  | [Ինչ է Higher Order Function-ը JavaScript-ում?](#ինչ-է-higher-order-function-ը-javascript-ում)   |
| 37  | [Ինչ է Currying-ը JavaScript-ում?](#ինչ-է-currying-ը-javascript-ում)                             |
| 38  | [Ինչ է JavaScript-ի Task Queue-ը?](#ինչ-է-javascript-ի-task-queue-ը)                             |
| 39  | [Ինչ է JavaScript-ում տարբեր սխալների տեսակները (SyntaxError, ReferenceError, TypeError)?](#ինչ-է-javascript-ում-տարբեր-սխալների-տեսակները-syntaxerror-referenceerror-typeerror) |
| 40  | [Ինչ է JavaScript-ի Garbage Collection-ը?](#ինչ-է-javascript-ի-garbage-collection-ը)            |
| 41  | [Ինչ է Promise Chaining-ը JavaScript-ում?](#ինչ-է-promise-chaining-ը-javascript-ում)             |
| 42  | [Ինչ է Microtasks-ը JavaScript-ում?](#ինչ-է-microtasks-ը-javascript-ում)                         |
| 43  | [Ինչ է Callback Hell-ը և ինչպես կարող ենք այն խուսափել?](#ինչ-է-callback-hell-ը-և-ինչպես-կարող-ենք-այն-խուսափել) |
| 44  | [Ինչ տարբերություն կա `setTimeout`, `setInterval` և `requestAnimationFrame` միջև?](#ինչ-տարբերություն-կա-settimeout-setinterval-և-requestanimationframe-միջև) |
| 45  | [Ինչ է Service Worker-ը JavaScript-ում?](#ինչ-է-service-worker-ը-javascript-ում)                 |
| 46  | [Ինչ է տարբեր եղանակներ զանգվածի միջոցով անցնելու համար JavaScript-ում?](#ինչ-է-տարբեր-եղանակներ-զանգվածի-միջոցով-անցնելու-համար-javascript-ում) |
| 47  | [Ինչ է Web Storage-ը (localStorage և sessionStorage)?](#ինչ-է-web-storage-ը-localstorage-և-sessionstorage) |
| 48  | [Ինչ է Proxy-ը և Reflect-ը JavaScript-ում?](#ինչ-է-proxy-ը-և-reflect-ը-javascript-ում)           |
| 49  | [Ինչ է JavaScript-ում generators-ը?](#ինչ-է-javascript-ում-generators-ը)                         |
| 50  | [Ինչ է Iterables և Iterators-ը JavaScript-ում?](#ինչ-է-iterables-և-iterators-ը-javascript-ում)   |
| 51  | [Ինչ է Destructuring-ը JavaScript-ում?](#ինչ-է-destructuring-ը-javascript-ում)                   |
| 52  | [Ինչ է Template Literals-ը և ինչպես կարող ենք այն օգտագործել?](#ինչ-է-template-literals-ը-և-ինչպես-կարող-ենք-այն-օգտագործել) |
| 53  | [Ինչ է Tagged Templates-ը JavaScript-ում?](#ինչ-է-tagged-templates-ը-javascript-ում)             |
| 54  | [Ինչ է Set-ը և Map-ը JavaScript-ում?](#ինչ-է-set-ը-և-map-ը-javascript-ում)                       |
| 55  | [Ինչ է JavaScript-ի Event Delegation-ը?](#ինչ-է-javascript-ի-event-delegation-ը)                 |
| 56  | [Ինչ է Factory Function-ը JavaScript-ում?](#ինչ-է-factory-function-ը-javascript-ում)             |
| 57  | [Ինչ է Class-ը JavaScript-ում?](#ինչ-է-class-ը-javascript-ում)                                   |
| 58  | [Ինչ է object cloning-ի տարբեր եղանակներ JavaScript-ում?](#ինչ-է-object-cloning-ի-տարբեր-եղանակներ-javascript-ում) |
| 59  | [Ինչ է JSON-ը և ինչու է այն կարևոր JavaScript-ում?](#ինչ-է-json-ը-և-ինչու-է-այն-կարևոր-javascript-ում) |
| 60  | [Ինչ է AJAX-ը JavaScript-ում?](#ինչ-է-ajax-ը-javascript-ում)                                     |
| 61  | [Ինչ է Fetch API-ը և ինչպես է այն աշխատում?](#ինչ-է-fetch-api-ը-և-ինչպես-է-այն-աշխատում)         |
| 62  | [Ինչ է Axios-ը և ինչ է տարբերությունը Fetch API-ի հետ?](#ինչ-է-axios-ը-և-ինչ-է-տարբերությունը-fetch-api-ի-հետ) |
| 63  | [Ինչ է JavaScript-ում Modules-ը?](#ինչ-է-javascript-ում-modules-ը)                               |
| 64  | [Ինչ է WebSockets-ը JavaScript-ում?](#ինչ-է-websockets-ը-javascript-ում)                         |
| 65  | [Ինչ է DOM Traversing-ը JavaScript-ում?](#ինչ-է-dom-traversing-ը-javascript-ում)                 |
| 66  | [Ինչ է Custom Events-ը JavaScript-ում?](#ինչ-է-custom-events-ը-javascript-ում)                   |
| 67  | [Ինչ է Shadow DOM-ը JavaScript-ում?](#ինչ-է-shadow-dom-ը-javascript-ում)                         |
| 68  | [Ինչ է JavaScript-ում polyfill-ը?](#ինչ-է-javascript-ում-polyfill-ը)                             |
| 69  | [Ինչ է Event Loop-ի և Call Stack-ի միջև կապը JavaScript-ում?](#ինչ-է-event-loop-ի-և-call-stack-ի-միջև-կապը-javascript-ում) |
| 70  | [Ինչ է Nullish Coalescing Operator-ը JavaScript-ում?](#ինչ-է-nullish-coalescing-operator-ը-javascript-ում) |
| 71  | [Ինչ է Optional Chaining-ը JavaScript-ում?](#ինչ-է-optional-chaining-ը-javascript-ում)           |
| 72  | [Ինչ է ES5 և ES6 տարբերությունները JavaScript-ում?](#ինչ-է-es5-և-es6-տարբերությունները-javascript-ում) |
| 73  | [Ինչ է JavaScript Engine-ը և ինչ տարբերություն կա V8-ի և SpiderMonkey-ի միջև?](#ինչ-է-javascript-engine-ը-և-ինչ-տարբերություն-կա-v8-ի-և-spidermonkey-ի-միջև) |
| 74  | [Ինչ է Node.js-ը և ինչու է այն կարևոր JavaScript-ի համար?](#ինչ-է-nodejs-ը-և-ինչու-է-այն-կարևոր-javascript-ի-համար) |
| 75  | [Ինչ է JavaScript-ում streams-ը?](#ինչ-է-javascript-ում-streams-ը)                               |
| 76  | [Ինչ է JavaScript-ի տարբեր տվյալների կառուցվածքները (Data Structures)?](#ինչ-է-javascript-ի-տարբեր-տվյալների-կառուցվածքները-data-structures) |
| 77  | [Ինչ է JavaScript-ում WeakRef-ը?](#ինչ-է-javascript-ում-weakref-ը)                               |
| 78  | [Ինչ է Web APIs-ը JavaScript-ում?](#ինչ-է-web-apis-ը-javascript-ում)                             |
| 79  | [Ինչ է JavaScript-ի Performance Optimization-ը?](#ինչ-է-javascript-ի-performance-optimization-ը) |
| 80  | [Ինչ է JavaScript-ում Event Listeners-ը?](#ինչ-է-javascript-ում-event-listeners-ը)               |
| 81  | [Ինչ է JavaScript-ում debounce-ի timeout-ի կիրառությունը?](#ինչ-է-javascript-ում-debounce-ի-timeout-ի-կիրառությունը) |
| 82  | [Ինչ է JavaScript-ում singleton pattern-ը?](#ինչ-է-javascript-ում-singleton-pattern-ը)           |
| 83  | [Ինչ է JavaScript-ում memory leak-ը և ինչպես կարող ենք խուսափել?](#ինչ-է-javascript-ում-memory-leak-ը-և-ինչպես-կարող-ենք-խուսափել) |
| 84  | [Ինչ է JavaScript-ում Data Binding-ը?](#ինչ-է-javascript-ում-data-binding-ը)                     |
| 85  | [Ինչ է JavaScript-ում async generator-ը?](#ինչ-է-javascript-ում-async-generator-ը)               |
| 86  | [Ինչ է Intersection Observer API-ը JavaScript-ում?](#ինչ-է-intersection-observer-api-ը-javascript-ում) |
| 87  | [Ինչ է JavaScript-ում DOM Events-ը?](#ինչ-է-javascript-ում-dom-events-ը)                         |
| 88  | [Ինչ է JavaScript-ում class inheritance-ը?](#ինչ-է-javascript-ում-class-inheritance-ը)           |
| 89  | [Ինչ է JavaScript-ում different states of a Promise-ը?](#ինչ-է-javascript-ում-different-states-of-a-promise-ը) |
| 90  | [Ինչ է JavaScript-ում Event Target-ը?](#ինչ-է-javascript-ում-event-target-ը)                     |
| 91  | [Ինչ է JavaScript-ում Module Federation-ը?](#ինչ-է-javascript-ում-module-federation-ը)           |
| 92  | [Ինչ է JavaScript-ում array-ի մանիպուլյացիայի տարբեր եղանակներ?](#ինչ-է-javascript-ում-array-ի-մանիպուլյացիայի-տարբեր-եղանակներ) |
| 93  | [Ինչ է JavaScript-ում dynamic imports-ը?](#ինչ-է-javascript-ում-dynamic-imports-ը)               |
| 94  | [Ինչ է JavaScript-ում Proxy Pattern-ը?](#ինչ-է-javascript-ում-proxy-pattern-ը)                   |
| 95  | [Ինչ է JavaScript-ում Function Overloading-ը?](#ինչ-է-javascript-ում-function-overloading-ը)     |
| 96  | [Ինչ է JavaScript-ում Symbol()-ի տարբեր կիրառությունները?](#ինչ-է-javascript-ում-symbol-ի-տարբեր-կիրառությունները) |
| 97  | [Ինչ է JavaScript-ում Virtual DOM-ը?](#ինչ-է-javascript-ում-virtual-dom-ը)                       |
| 98  | [Ինչ է JavaScript-ում `Object.freeze()`-ը?](#ինչ-է-javascript-ում-objectfreeze-ը)                |
| 99  | [Ինչ է JavaScript-ում `Object.seal()`-ը?](#ինչ-է-javascript-ում-objectseal-ը)                    |
| 100 | [Ինչ է JavaScript-ում Function Composition-ը?](#ինչ-է-javascript-ում-function-composition-ը)    |


---

1. ### Որոնք են JavaScript լեզվում Primitive տիպերը?

    JavaScript-ը ունի 7 primitive տիպեր՝

    1. [string](https://tc39.es/ecma262/multipage/ecmascript-data-types-and-values.html#sec-ecmascript-language-types-string-type)
    2. [number](https://tc39.es/ecma262/multipage/ecmascript-data-types-and-values.html#sec-numeric-types)
    3. [boolean](https://tc39.es/ecma262/multipage/ecmascript-data-types-and-values.html#sec-ecmascript-language-types-boolean-type)
    4. [null](https://tc39.es/ecma262/multipage/ecmascript-data-types-and-values.html#sec-ecmascript-language-types-null-type)
    5. [undefined](https://tc39.es/ecma262/multipage/ecmascript-data-types-and-values.html#sec-ecmascript-language-types-undefined-type)
    6. [symbol](https://tc39.es/ecma262/multipage/ecmascript-data-types-and-values.html#sec-ecmascript-language-types-symbol-type) (ECMAScript 6-ից)
    7. [bigint](https://tc39.es/ecma262/multipage/ecmascript-data-types-and-values.html#sec-ecmascript-language-types-bigint-type) (ECMAScript 11-ից)

    ```javascript
    typeof 1; // number
    typeof 'hello'; // string
    typeof true; // boolean
    typeof null; // object
    typeof undefined; // undefined
    typeof Symbol(); // symbol
    typeof 1n; // bigint
    ```
2. ###  Ինչ է undefined և undeclared?
   
    "undefined" նշանակում է, որ փոփոխականը հայտարարված է, բայց այն չունի արժեք:

    ```javascript
    var a;
    typeof a; // undefined
    ```

    "undeclared" նշանակում է, որ փոփոխականը երբեք չի հայտարարվել:

    ```javascript
    console.log(c); // ReferenceError: c is not defined
    ```

3. ### Ինչի համար է typeof օպերատորը

   `typeof` օպերատորը օգտագործվում է փոփոխականի տվյալների տիպը պարզելու համար:

   ```javascript
   console.log(typeof 123); // "number"
   console.log(typeof 'Hello'); // "string"
   console.log(typeof true); // "boolean"
   ```
---

**[⬆ Back to Top](#բովանդակություն)**

---


4. ### Ինչ է NAN և ինչպես կարող ենք հասկանալ, որ արժեքը NAN է
   `NaN` նշանակում է **"անվավեր թիվ"** (invalid number) JavaScript-ում։ Այն առաջանում է այն դեպքում, երբ թվաբանական գործողությունը կամ արժեքի փոխակերպումը չի տալիս վավեր թիվ։
   
   ```javascript
   Number('abc');    // NaN
   Math.sqrt(-1);    // NaN
   0 / 0;           // NaN
   ```
   Ութային համակարգով թվեր, ինչպիսիք են 0o46, վավեր են JavaScript-ում և չեն վերադարձնում NaN։ Օրինակ՝
   
    ```javascript
    Number('0o46'); // 38
    Number('0b111'); // 7
    Number('0x16'); // 22
    ```
   
   #### Ինչպես ստուգել, որ արժեքը NaN է
   Քանի որ NaN === NaN միշտ վերադարձնում է false, դուք չեք կարող ուղղակի համեմատել NaN-ի հետ։ Դրա փոխարեն օգտագործեք isNaN() կամ Number.isNaN() ֆունկցիաները:
   
   **`isNaN()`**
   Ստուգում է, արդյոք արժեքը "Not-a-Number" է, սակայն նախ փոխակերպում է այն թվի։
   Այս պատճառով այն երբեմն կարող է սխալ արդյունք տալ:

   ```javascript
   isNaN('abc');      // true (փոխակերպումից հետո)
   isNaN(NaN);        // true
   isNaN(0o46);       // false (վավեր թիվ է)
   isNaN('123abc');   // true (փոխակերպման սխալ)
   ```
   **`Number.isNaN()`**
   Ավելի խիստ տարբերակ է, որը ստուգում է միայն այն դեպքում, երբ արժեքը իսկապես NaN է և չի փորձում որևէ փոխակերպում։

    ```javascript
    Number.isNaN('abc');    // false (ոչ թիվ է)
    Number.isNaN(NaN);      // true
    Number.isNaN(0o46);     // false (վավեր թիվ է)
    Number.isNaN('123abc'); // false (ոչ մի փոխակերպում չկա)
    ```
---

**[⬆ Back to Top](#բովանդակություն)**

---


5. ### Ինչ է toString և ինչպես կարող ենք այն օգտագործել
   `toString`-ը JavaScript-ում օբյեկտների և primitive արժեքների մեթոդ է, որը վերադարձնում է տվյալ արժեքի տողի (string) ներկայացումը։ Այն հիմնականում մաս է կազմում `Object.prototype`-ին և հասանելի է գրեթե բոլոր օբյեկտների և արժեքների համար։
   
   #### Ինչպես է աշխատում `toString` մեթոդը
   **Primitive արժեքներ**  
   Primitive արժեքները (օրինակ՝ թիվ, boolean, string) ունեն իրենց սեփական `toString` մեթոդը, որը վերադարձնում է դրանց տողային ներկայացումը։

   ```javascript
   let num = 123;
   console.log(num.toString());  // "123"

   let bool = true;
   console.log(bool.toString()); // "true"
   ```
   **Զանգվածներ (Array.prototype.toString)**
   Զանգվածի տարրերը վերածվում են տողերի և բաժանվում ստորակետներով։

    ```javascript
   let arr = [1, 2, 3];
   console.log(arr.toString()); // "1,2,3"
    ```
   **Օբյեկտներ (Object.prototype.toString)**
   Եթե օբյեկտը չունի իր սեփական toString մեթոդը, JavaScript-ը ժառանգում է այն Object.prototype.toString-ից, որը վերադարձնում է [object <Type>] ձևաչափի արժեք։

    ```javascript
    let obj = {};
    console.log(obj.toString()); // "[object Object]"
    ```
   
   **Պատվերով toString մեթոդ**
   Օբյեկտները կարող են վերաձևավորել իրենց սեփական toString մեթոդը՝ տրամադրելով ավելի օգտակար ներկայացում։

    ```javascript
      let product = {
      name: "Laptop",
      price: 1000,
      toString: function () {
      return `Product: ${this.name}, Price: $${this.price}`;
      }
     }
     console.log(product.toString()); // "Product: Laptop, Price: $1000"
    ```
   **Թվային հիմքերի աջակցություն**
 
   toString մեթոդը թույլ է տալիս թիվը փոխակերպել տարբեր թվային հիմքերով՝ տրամադրելով հիմքի արժեքը արգումենտով։
       
   ```javascript
      let num = 255;
      console.log(num.toString(2));  // "11111111" (երկուական)
      console.log(num.toString(16)); // "ff" (տասնվեցական)
    ```
   #### Ինչ մեթոդներ են օգտագործվում
   
   #### `Object.prototype.toString`
   Այս մեթոդը ըստ լռելյայն վերադարձնում է `[object <Type>]` ձևաչափի արժեք՝ կախված օբյեկտի տիպից։
   
   ```javascript
   let obj = {};
   console.log(Object.prototype.toString.call(obj)); // "[object Object]"
   ```
   
   #### Տիպերին հատուկ `toString` մեթոդներ
   Primitive արժեքները (թվեր, boolean, տողեր) կամ զանգվածները հաճախ ունեն իրենց սեփական `toString` մեթոդները։
   
   ---
   
   #### Տիպի փոխակերպում (Type Coercion)
   Երբ JavaScript-ին անհրաժեշտ է արժեքը տողի ձևով, այն ավտոմատ կերպով կիրառում է `toString` կամ `String()`։
   
   ```javascript
   let value = 42;
   console.log(String(value)); // "42"
   ```
   
   ---
   
   #### Կարևոր Նշումներ
   
   - **Primitive տիպերի դեպքում**՝ `toString` մեթոդը հաճախ ուղղակի վերադարձնում է արժեքի տողային ներկայացումը։
   - **Օբյեկտների դեպքում**՝ դուք կարող եք վերաձևավորել `toString`, որպեսզի ներկայացումը լինի ավելի օգտակար։
   - **Սխալ գործածություն**՝ `null` կամ `undefined` արժեքների վրա կիրառելիս մեթոդը կվերադարձնի սխալ։
   
   ```javascript
   console.log(null.toString());       // TypeError: Cannot read property 'toString' of null
   console.log(undefined.toString()); // TypeError: Cannot read property 'toString' of undefined
   ```
   
   Այս խնդիրը կարելի է լուծել `String()` ֆունկցիայի միջոցով։
   
   ```javascript
   console.log(String(null));       // "null"
   console.log(String(undefined));  // "undefined"
   ```
---

**[⬆ Back to Top](#բովանդակություն)**

---

6. ### Ինչ է toNumber և ինչպես կարող ենք այն օգտագործել
   
   `toNumber` հասկացությունը JavaScript-ում վերաբերում է այն պրոցեսին, որով արժեքը փոխարկվում է թվի։ Չնայած JavaScript-ում չկա հատուկ ներկառուցված `toNumber` մեթոդ, այս գործընթացը իրականացվում է **Number()** ֆունկցիայի կամ JavaScript-ի ավտոմատ տիպի փոխակերպման միջոցով։
   
   ---
   
   #### Ինչպես է աշխատում `toNumber`
   
   1. **`Number()` ֆունկցիա**
      `Number()` ֆունկցիան օգտագործվում է տողերը, boolean-ները և այլ արժեքներ թվի փոխակերպելու համար։
   
      ```javascript
      let str = "123";
      console.log(Number(str)); // 123 (թիվ)
   
      let bool = true;
      console.log(Number(bool)); // 1
   
      let nullValue = null;
      console.log(Number(nullValue)); // 0
      ```
   
   2. **Տիպի ավտոմատ փոխակերպում (Type Coercion)**
      Երբ JavaScript-ը ակնկալում է թիվ, բայց ստանում է այլ տիպի արժեք, այն ավտոմատ կերպով փորձում է փոխակերպել այդ արժեքը թվի։
   
      ```javascript
      let result = "5" * 2;
      console.log(result); // 10 (տողը փոխակերպվեց թվի)
      ```
   
   3. **Տողերի վրա կիրառումը**
      Եթե տողը պարունակում է միայն թվեր, այն կարող է հաջողությամբ փոխարկվել։ Հակառակ դեպքում արդյունքը կլինի `NaN`։
   
      ```javascript
      let validStr = "456";
      console.log(Number(validStr)); // 456
   
      let invalidStr = "123abc";
      console.log(Number(invalidStr)); // NaN
      ```
   
   ---
   
   #### Կարևոր Նշումներ
   
   - **Boolean-ների փոխարկում**:
      - `true` → 1
      - `false` → 0
   
   - **Null-ի և Undefined-ի փոխարկում**:
      - `null` → 0
      - `undefined` → `NaN`
   
   - **Տողի փոխակերպման սխալներ**:
     Եթե տողը պարունակում է ոչ թվային սիմվոլներ, արդյունքը կլինի `NaN`։
   
     ```javascript
     console.log(Number("abc")); // NaN
     console.log(Number("123abc")); // NaN
     ```
   
   - **Օբյեկտների փոխարկում**:
     Օբյեկտները նախ փորձում են փոխարկվել primitive արժեքի (օգտագործելով `valueOf()` կամ `toString()`), ապա արդյունքը փոխարկվում է թվի։
   
     ```javascript
     let obj = {
       valueOf() {
         return 42;
       }
     };
     console.log(Number(obj)); // 42
     ```
   
   ---
   
   #### Օրինակներ
   
   #### Թվային փոխակերպումներ տարբեր տիպերի վրա
   
   ```javascript
   console.log(Number("42"));     // 42
   console.log(Number(true));      // 1
   console.log(Number(false));     // 0
   console.log(Number(null));      // 0
   console.log(Number(undefined)); // NaN
   ```
   
   #### Տիպի ավտոմատ փոխակերպում
   
   ```javascript
   console.log("6" * 2); // 12 (տողը փոխարկվեց թվի)
   console.log("6" + 2); // "62" (կատարվեց տողի միացում)
   ```
   
   #### Օբյեկտի փոխակերպում թվի
   
   ```javascript
   let customObj = {
     toString() {
       return "100";
     }
   };
   console.log(Number(customObj)); // 100
   ```
   
   ---
   
   #### Ինչպես խուսափել սխալներից
   
   1. **Ստուգեք `NaN` արդյունքները**
      Կարող եք օգտագործել `isNaN()` կամ `Number.isNaN()`՝ պարզելու համար, արդյոք փոխակերպումը հաջող է։
   
      ```javascript
      let result = Number("abc");
      console.log(Number.isNaN(result)); // true
      ```
   
   2. **Փոխակերպում `parseInt()` կամ `parseFloat()` միջոցով**
      Եթե ցանկանում եք ստանալ միայն թվային մասը, օգտագործեք `parseInt()` կամ `parseFloat()`։
   
      ```javascript
      console.log(parseInt("123abc"));   // 123
      console.log(parseFloat("123.45px")); // 123.45


---

**[⬆ Back to Top](#բովանդակություն)**

---

7. ### Ինչ է toBoolean և ինչպես կարող ենք այն օգտագործել
   
   `toBoolean` հասկացությունը JavaScript-ում վերաբերում է արժեքների փոխակերպմանը Boolean (ճշմարիտ կամ կեղծ) տիպի։ Չնայած չկա հատուկ ներկառուցված `toBoolean` մեթոդ, այս պրոցեսը իրականացվում է JavaScript-ի ավտոմատ տիպի փոխակերպման կամ **Boolean()** ֆունկցիայի միջոցով։
   
   ---
   
   #### Ինչպես է աշխատում `toBoolean`
   
   1. **`Boolean()` ֆունկցիա**
      `Boolean()` ֆունկցիան օգտագործվում է ցանկացած արժեք Boolean տիպի փոխարկելու համար։
   
      ```javascript
      console.log(Boolean(1));        // true
      console.log(Boolean(0));        // false
      console.log(Boolean("hello")); // true
      console.log(Boolean(""));      // false
      console.log(Boolean(null));     // false
      console.log(Boolean(undefined));// false
      ```
   
   2. **Ավտոմատ փոխակերպում (Type Coercion)**
      JavaScript-ը հաճախ ավտոմատ կերպով փոխակերպում է արժեքը Boolean-ի՝ կախված կոնտեքստից (օրինակ՝ պայմաններում, if արտահայտություններում):
   
      ```javascript
      if ("hello") {
        console.log("This is true");
      }
      // Output: This is true
   
      if (0) {
        console.log("This will not run");
      }
      // Output: ոչինչ չի տպվի
      ```
   
   ---
   
   #### Կարևոր Նշումներ
   
   #### Ճշմարիտ (Truthy) արժեքներ
   
   Հետևյալ արժեքները փոխարկվում են **true**:
   - Ցանկացած ոչ դատարկ տող (`"hello"`, `"0"`)
     - Ցանկացած ոչ զրոյական թիվ (`1`, `-1`, `3.14`)
     - Ցանկացած օբյեկտ կամ զանգված (`{}`, `[]`)
     - Infinity (`Infinity`, `-Infinity`)
   
   #### Կեղծ (Falsy) արժեքներ
   
   Հետևյալ արժեքները փոխարկվում են **false**:
   - `false`
     - `0`
     - `""` (դատարկ տող)
     - `null`
     - `undefined`
     - `NaN`
   
   ```javascript
   console.log(Boolean(false));     // false
   console.log(Boolean(0));         // false
   console.log(Boolean(""));       // false
   console.log(Boolean(null));      // false
   console.log(Boolean(undefined)); // false
   console.log(Boolean(NaN));       // false
   ```
   
   ---
   
   #### Օրինակներ
   
   #### Պայմաններում ավտոմատ փոխակերպում
   
   ```javascript
   let value = "hello";
   if (value) {
     console.log("Truthy value");
   } else {
     console.log("Falsy value");
   }
   // Output: Truthy value
   ```
   
   #### Ճշմարիտ և կեղծ արժեքների ցուցակ
   
   ```javascript
   let truthyValues = [1, "0", {}, [], "hello", Infinity];
   let falsyValues = [0, "", null, undefined, NaN, false];
   
   truthyValues.forEach(value => console.log(Boolean(value))); // true
   falsyValues.forEach(value => console.log(Boolean(value))); // false
   ```
   
   ---
   
   #### Ինչպես խուսափել սխալներից
   
   1. **Միշտ օգտագործեք հստակ փոխակերպում**
      Օգտագործեք `Boolean()` ֆունկցիան, եթե պետք է հստակ պարզեք, որ արժեքը Boolean է։
   
      ```javascript
      console.log(Boolean("")); // false
      console.log(Boolean("false")); // true
      ```
   
   2. **Պայմաններում հաշվարկների ժամանակ ուշադրություն դարձնել կոնտեքստին**
      Գիտակցեք, որ որոշ արժեքներ, օրինակ՝ "0" (տող), կարող են համարվել truthy, մինչդեռ թվային 0-ը falsy է։
   
      ```javascript
      if ("0") {
        console.log("Truthy");
      }
      // Output: Truthy
   
      if (0) {
        console.log("Falsy");
      }
      // Output: ոչինչ չի տպվի
      ```
  
---

   **[⬆ Back to Top](#բովանդակություն)**

   ---

8. ### Ինչ է Coercion և ինչպես կարող ենք այն օգտագործել
   
   `Coercion`-ը JavaScript-ում վերաբերում է մեկ տիպի արժեքի ավտոմատ կամ ձեռքով փոխակերպմանը մյուս տիպի։ Սա սովորաբար կատարվում է, երբ JavaScript-ը պետք է աշխատի տարբեր տիպի արժեքների հետ՝ դրանք համապատասխանեցնելով։ Տարբերում են երկու հիմնական տեսակի `Coercion`՝ **Ավտոմատ (Implicit)** և **Ձեռքով (Explicit)**։
   
   ---
   
   #### Ինչպես է աշխատում Coercion
   
   #### 1. Ավտոմատ (Implicit Coercion)
   Ավտոմատ փոխակերպումը տեղի է ունենում, երբ JavaScript-ը ինքն է որոշում, որ անհրաժեշտ է փոխակերպել արժեքը՝ որոշակի գործողություն կատարելու համար։
   
   ```javascript
   console.log(1 + "2");    // "12" (թիվը փոխակերպվեց տողի)
   console.log("5" * 2);    // 10 (տողը փոխակերպվեց թվի)
   console.log(false == 0);  // true (Boolean-ը փոխակերպվեց թվի)
   ```
   
   #### 2. Ձեռքով (Explicit Coercion)
   Ձեռքով փոխակերպումը տեղի է ունենում, երբ ծրագրավորողը օգտագործում է հատուկ ֆունկցիաներ կամ օպերատորներ՝ արժեքը փոխակերպելու համար։
   
   ```javascript
   console.log(Number("123"));   // 123 (տողը փոխակերպվեց թվի)
   console.log(String(123));      // "123" (թիվը փոխակերպվեց տողի)
   console.log(Boolean(0));       // false (թիվը փոխակերպվեց Boolean-ի)
   ```
   
   ---
   
   #### Օրինակներ
   
   #### Թվերի և տողերի փոխակերպում
   
   - **Ավտոմատ փոխակերպում**:
     ```javascript
     console.log("6" - 1); // 5 (տողը փոխակերպվեց թվի)
     console.log("6" + 1); // "61" (թիվը փոխակերպվեց տողի)
     ```
   
   - **Ձեռքով փոխակերպում**:
     ```javascript
     console.log(Number("6"));   // 6
     console.log(String(6));      // "6"
     ```
   
   #### Boolean-ի փոխակերպում
   
   - **Ավտոմատ փոխակերպում**:
     ```javascript
     if ("hello") {
       console.log("Truthy");
     }
     // Output: Truthy
   
     if ("") {
       console.log("Falsy");
     } else {
       console.log("Falsy value");
     }
     // Output: Falsy value
     ```
   
   - **Ձեռքով փոխակերպում**:
     ```javascript
     console.log(Boolean("hello")); // true
     console.log(Boolean(0));        // false
     ```
   
   #### Օբյեկտների փոխակերպում
   
   JavaScript-ը փորձելու է օբյեկտը primitive արժեքի փոխակերպել՝ օգտագործելով նրա `toString()` կամ `valueOf()` մեթոդները։
   
   ```javascript
   let obj = {
     valueOf() {
       return 42;
     }
   };
   console.log(obj + 1); // 43 (օբյեկտը փոխակերպվեց թվի)
   ```
   
   ---
   
   #### Կարևոր Նշումներ
   
   1. **Falsy և Truthy արժեքներ**
      JavaScript-ում որոշ արժեքներ, ինչպիսիք են `0`, `""`, `null`, `undefined`, և `NaN`, համարվում են **Falsy**։ Մնացած բոլոր արժեքները համարվում են **Truthy**։
   
   2. **Օպերատորների ազդեցությունը**
      Տարբեր օպերատորներ, օրինակ՝ `+`, `-`, և `==`, կարող են տարբեր կերպ ազդել փոխակերպումների վրա։
   
      ```javascript
      console.log(1 + "1");  // "11" (տողային միացում)
      console.log(1 - "1");  // 0 (թվային հանում)
      console.log(1 == "1"); // true (ավտոմատ փոխակերպում)
      ```
   
   3. **Խուսափեք անսպասելի ավտոմատ փոխակերպումներից**
      Ավելի հստակություն ստանալու համար օգտագործեք === օպերատորը՝ տիպը և արժեքը համեմատելու համար։
   
      ```javascript
      console.log(1 === "1"); // false (ոչ մի փոխակերպում չի կատարվում)
      ```
   
   ---
   
   #### Ինչպես խուսափել սխալներից
   
   1. **Հստակորեն փոխակերպեք արժեքները**
      Օգտագործեք `String()`, `Number()` կամ `Boolean()` ֆունկցիաները՝ ձեռքով փոխակերպումներ կատարելու համար։
   
      ```javascript
      console.log(Number("123")); // 123
      console.log(Boolean(""));  // false
      ```
   
   2. **Գիտակցեք Truthy և Falsy արժեքները**
      Գիտակցեք, թե որ արժեքները ավտոմատ կերպով կդառնան `true` կամ `false`:
   
      ```javascript
      let values = [0, 1, "", "hello", null, undefined, [], {}];
      values.forEach(value => console.log(Boolean(value)));
      // Output: false, true, false, true, false, false, true, true
      ```

---

**[⬆ Back to Top](#բովանդակություն)**

---

9. ### Ինչ է boxing-ը

   `Boxing`-ը JavaScript-ում այն գործընթացն է, որի միջոցով primitive (պարզագույն) արժեքը, ինչպիսիք են թվերը, տողերը կամ Boolean-ները, **փոխակերպվում են համապատասխան օբյեկտի տիպի**։ Սա թույլ է տալիս կիրառել օբյեկտներին բնորոշ մեթոդներ և հատկություններ primitive արժեքների վրա։
   
   JavaScript-ը իրականացնում է այս գործընթացը ավտոմատ կերպով, երբ primitive արժեքի վրա կիրառում եք մեթոդ կամ հատկություն, որը բնորոշ է օբյեկտներին։
   
   ---
   
   #### Ինչպես է աշխատում Boxing-ը
   
   1. **Primitive արժեքի ավտոմատ փաթեթավորում**:
      Երբ primitive արժեքի վրա կանչում եք մեթոդ կամ հատկություն, JavaScript-ը ստեղծում է համապատասխան օբյեկտի ժամանակավոր պատճեն (wrapper object):
   
      ```javascript
      let str = "hello";
      console.log(str.toUpperCase()); // "HELLO"
      ```
      Այստեղ `"hello"` տողը ավտոմատ կերպով «փաթեթավորվում» է `String` օբյեկտի մեջ, որպեսզի հնարավոր լինի կանչել `toUpperCase()` մեթոդը։
   
   2. **Ավարտից հետո օբյեկտի ոչնչացում**:
      Երբ գործողությունը ավարտվում է, ժամանակավոր օբյեկտը ոչնչացվում է, և primitive արժեքը մնում է անփոփոխ։
   
      ```javascript
      let num = 42;
      console.log(num.toFixed(2)); // "42.00"
      console.log(typeof num);    // "number"
      ```
   
   ---
   
   #### Օրինակներ
   
   #### Տողի (String) Boxing
   
   ```javascript
   let text = "JavaScript";
   console.log(text.length);     // 10 (տողը փաթեթավորվում է String օբյեկտի մեջ)
   console.log(text.charAt(4));  // "S"
   ```
   
   #### Թվերի (Number) Boxing
   
   ```javascript
   let number = 123.456;
   console.log(number.toFixed(2)); // "123.46"
   console.log(number.toExponential()); // "1.23456e+2"
   ```
   
   #### Boolean Boxing
   
   ```javascript
   let isTrue = true;
   console.log(isTrue.toString()); // "true"
   ```
   
   ---
   
   #### Unboxing
   
   **Unboxing**-ը հակառակ գործընթացն է, երբ օբյեկտը նորից վերածվում է primitive արժեքի։
   
   ```javascript
   let numObj = new Number(42); // Number օբյեկտ
   let primitiveNum = numObj.valueOf(); // Primitive թիվ
   console.log(primitiveNum); // 42
   console.log(typeof primitiveNum); // "number"
   ```
   
   ---
   
   #### Կարևոր Նշումներ
   
   1. **Ավտոմատ Boxing-ը կարճատև է**
      Primitive արժեքները փաթեթավորվում են միայն մեթոդի կանչի ընթացքում և անմիջապես ոչնչացվում են։ Primitive արժեքը միշտ մնում է անփոփոխ։
   
   2. **Մի օգտագործեք `new` օպերատորը primitive արժեքների համար**
      Ցանկացած ժամանակ փորձեք աշխատել primitive արժեքների հետ առանց դրանք «հստակ փաթեթավորելու»:
   
      ```javascript
      let str1 = "hello";          // Primitive տող
      let str2 = new String("hello"); // String օբյեկտ
   
      console.log(typeof str1); // "string"
      console.log(typeof str2); // "object"
      ```
   
   3. **Primitive արժեքների և օբյեկտների համեմատում**
      Primitive արժեքներն ու դրանց օբյեկտները կարող են տարբեր արդյունք տալ համեմատության դեպքում:
   
      ```javascript
      let str1 = "hello";
      let str2 = new String("hello");
   
      console.log(str1 == str2);  // true (տիպը փոխակերպվում է)
      console.log(str1 === str2); // false (տիպերը տարբեր են)
      ```
  
---

**[⬆ Back to Top](#բովանդակություն)**

   ---


10. ### Ինչ են double equal (==) և triple equal (===) օպերատորները
  
 JavaScript-ում `==` (Double Equal) և `===` (Triple Equal) օպերատորները օգտագործվում են արժեքները համեմատելու համար։ Չնայած դրանք կարծես նման են, նրանք աշխատում են տարբեր կերպ։

   
   #### Տարբերությունը Double Equal (==) և Triple Equal (===) միջև
   
   #### 1. **Double Equal (`==`)**
   Double Equal օպերատորը համեմատում է երկու արժեքները **միայն նրանց արժեքների** հիման վրա, անտեսելով տիպը։ Եթե արժեքների տիպերը տարբեր են, JavaScript-ը ավտոմատ կերպով փորձում է դրանք փոխակերպել նույն տիպի (type coercion)։
   
   Եթե երկու արժեքներն էլ նույն տիպի են, `==`-ը իրականացնում է նույն գործողությունը, ինչ `===`-ը՝ համեմատելով նրանց արժեքները առանց որևէ փոխակերպման։
   
   #### Օրինակներ
   ```javascript
   console.log(5 == "5");       // true ("5" տողը փոխակերպվում է թվի)
   console.log(true == 1);       // true (true-ը փոխակերպվում է 1-ի)
   console.log(null == undefined); // true (միայն այս դեպքերում դրանք հավասար են)
   ```
   
   #### Կախվածությունը տիպի փոխակերպումից
   Type coercion-ը կարող է բերել անսպասելի արդյունքների:
   ```javascript
   console.log("" == 0);  // true (դատարկ տողը փոխակերպվում է թվի)
   console.log("\t\n" == 0); // true (սպիտակատողային սիմվոլները փոխակերպվում են թվի)
   ```
   
   #### 2. **Triple Equal (`===`)**
   Triple Equal օպերատորը համեմատում է երկու արժեքները **և նրանց արժեքների**, և նրանց տիպերի հիման վրա։ Եթե արժեքները տարբեր տիպերի են, դրանք համարվում են ոչ հավասար։
   
   #### Օրինակներ
   ```javascript
   console.log(5 === "5"); // false (տիպերը տարբեր են)
   console.log(true === 1); // false (տիպերը տարբեր են)
   console.log(null === undefined); // false (տիպերը տարբեր են)
   ```
   
   #### Առանց տիպի փոխակերպման
   Triple Equal-ը համեմատում է միայն այն, ինչ կա առանց որևէ փոխակերպման:
   ```javascript
   console.log("" === 0);  // false
   console.log("5" === 5); // false
   ```
   
   ---
   
   #### Երբ օգտագործել `==` և երբ `===`
   
   1. **Օգտագործեք `===`**
      - Երբ ցանկանում եք խուսափել անսպասելի տիպի փոխակերպումներից։
      - Երբ համեմատությունը պետք է լինի ավելի հստակ և կանխատեսելի։
   
   2. **Օգտագործեք `==` միայն այն դեպքում, եթե գիտեք, թե ինչպես է տիպի փոխակերպումը աշխատում**:
      ```javascript
      console.log(null == undefined); // true (սպեցիֆիկ դեպք)
      ```
   
   ---
   
   #### ECMA-262 Սպեցիֆիկացիա
   
   Համեմատության օպերատորների աշխատանքը մանրամասն նկարագրված է [ECMAScript Language Specification, Equality Operators](https://tc39.es/ecma262/#sec-abstract-equality-comparison):
   
   - **Abstract Equality Comparison (`==`)**՝ նկարագրում է, թե ինչպես է տիպի փոխակերպումը կատարվում։
   - **Strict Equality Comparison (`===`)**՝ նկարագրում է, թե ինչպես են համեմատվում արժեքներն առանց փոխակերպման։
   
   #### ECMAScript Specification:
   - [Abstract Equality Comparison](https://tc39.es/ecma262/#sec-abstract-equality-comparison)
   - [Strict Equality Comparison](https://tc39.es/ecma262/#sec-strict-equality-comparison)

   ---

   **[⬆ Back to Top](#բովանդակություն)**

   ---

11. ### Ինչ է hoisting-ը JavaScript-ում?
   **Hoisting**-ը JavaScript-ում այն մեխանիզմն է, որի միջոցով փոփոխականները, ֆունկցիաները և դասերը "բարձրացվում" են իրենց սահմանման տիրույթի վերև՝ դրանց հայտարարված լինելու մասին նախապես տեղեկացնելու նպատակով։ Սակայն միայն հայտարարված լինելը "բարձրացվում" է, ոչ թե նրանց արժեքի նշանակումը։
   
   Hoisting-ը կիրառվում է ինչպես գլոբալ, այնպես էլ ֆունկցիաների և բլոկների ներսում, ինչը նշանակում է, որ այն հիմնականում աշխատում է ցանկացած տիրույթում՝ համատեքստից կախված։
   
   ---
   
   #### Ինչպես է աշխատում Hoisting-ը
   
   #### 1. Փոփոխականների Hoisting
   
   - **`var`-ի դեպքում**:
     `var` փոփոխականները "բարձրացվում" են իրենց տիրույթի վերև, սակայն նրանց արժեքը մնում է անորոշ (`undefined`) մինչև ծրագրի ընթացքի ժամանակային պահը։ Այս հատկությունը կարող է առաջացնել սխալներ, քանի որ կարող եք փորձել մուտք գործել փոփոխականը նախքան նրա փաստացի արժեքի վերագրումը։
   
     ```javascript
     console.log(x); // undefined
     var x = 5;
     console.log(x); // 5
     ```
   
   - **`let` և `const`-ի դեպքում**:
     Թեև դրանք նույնպես "բարձրացվում" են, բայց մնում են "Temporal Dead Zone"-ում (ժամանակավոր մեռյալ գոտի) մինչև նրանց փաստացի հայտարարված պահը։ Օգտագործելը նախքան հայտարարելը կհանգեցնի սխալի։
   
     ```javascript
     console.log(y); // ReferenceError: Cannot access 'y' before initialization
     let y = 10;
     console.log(y); // 10
     ```
   
     Այս մեխանիզմը օգնում է կանխել ոչ կանխատեսելի վարքագիծ՝ ստիպելով հայտարարված փոփոխականներն օգտագործել միայն նրանց տեսանելիության սահմաններում։
   
   #### 2. Ֆունկցիաների Hoisting
   
   - **Function Declaration**:
     Ֆունկցիաների հայտարարումները ամբողջությամբ "բարձրացվում" են։ Սա նշանակում է, որ դուք կարող եք կանչել ֆունկցիան մինչև նրա սահմանումը։
   
     ```javascript
     greet(); // Output: "Hello!"
     function greet() {
       console.log("Hello!");
     }
     ```
   
   Սա հնարավոր է, քանի որ ֆունկցիայի ամբողջ սահմանումը, ներառյալ մարմինը, "բարձրացվում" է։
   
   - **Function Expressions**:
     Ֆունկցիաները, որոնք հայտարարված են որպես փոփոխականի արժեք, "բարձրացվում" են միայն որպես փոփոխական (`undefined`)։ Այսինքն՝ ֆունկցիայի փաստացի սահմանումը հասանելի չէ նախքան հայտարարված պահը։
   
     ```javascript
     sayHi(); // TypeError: sayHi is not a function
     var sayHi = function() {
       console.log("Hi!");
     };
     ```
   
   #### 3. Դասերի Hoisting
   
   Դասերը նույնպես "բարձրացվում" են, բայց մնում են "Temporal Dead Zone"-ում մինչև նրանց փաստացի հայտարարումը։ Սա նշանակում է, որ դրանք հասանելի չեն նախքան իրական հայտարարված պահը։
   
   ```javascript
   let obj = new MyClass(); // ReferenceError: Cannot access 'MyClass' before initialization
   class MyClass {
     constructor() {
       console.log("Instance created");
     }
   }
   ```
   
   Ի տարբերություն ֆունկցիաների, դասերը չեն կարող օգտագործվել իրենց սահմանումից առաջ, քանի որ դրանց բարձրացումը գործում է միայն որպես սինթաքսային ստուգում։
   
   ---
   
   #### Կարևոր Նշումներ
   
   1. **`var`-ը խորհուրդ չի տրվում օգտագործել:**
      - `var`-ի Hoisting-ը և արժեքի `undefined` դառնալու հատկությունը կարող են հանգեցնել բարդ սխալների։
      - Փոխարենը օգտագործեք `let` կամ `const`։
   
   2. **Function Expressions-ն ավելի կանխատեսելի է:**
      - Ֆունկցիաները, որոնք հայտարարված են որպես փոփոխականի արժեք, ավելի հստակ վերահսկում են իրենց հասանելիությունը։
   
   3. **Temporal Dead Zone (TDZ):**
      - `let`, `const`, և դասերը "բարձրացվում" են, բայց մնում են TDZ-ում մինչև իրական հայտարարումը։ TDZ-ն սկսվում է տիրույթի սկզբից և ավարտվում է փոփոխականի փաստացի հայտարարությամբ։
   
   4. **Հիմնված ECMAScript Սպեցիֆիկացիայի վրա:**
      - Hoisting-ի մեխանիզմի մանրամասները նկարագրված են [ECMAScript Language Specification](https://tc39.es/ecma262/#sec-variable-statement):
   
   ECMAScript Specification:
   - [Variable Statement](https://tc39.es/ecma262/#sec-variable-statement)
   - [Function Declaration Instantiation](https://tc39.es/ecma262/#sec-function-definitions-runtime-semantics-instantiatefunctionobject)
   - [Class Definitions](https://tc39.es/ecma262/#sec-class-definitions-runtime-semantics-classdefinitionevaluation)


   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

12. ### Ինչ տարբերություն կա let, const և var միջև?
   JavaScript-ում փոփոխականները կարելի է հայտարարել երեք հիմնական բանալի բառերով՝ `var`, `let` և `const`։ Թեև դրանք կարող են թվալ նման, դրանք ունեն տարբեր վարքագծեր և սահմանափակումներ, որոնք ազդում են դրանց օգտագործման վրա։

   
   #### Տարբերություններ
   
   #### 1. `var`
   
   - **Տիրույթ (Scope):**
     `var`-ով հայտարարված փոփոխականները ունեն ֆունկցիոնալ կամ գլոբալ տիրույթ, ինչը նշանակում է, որ դրանք տեսանելի են ամբողջ ֆունկցիայի կամ սկրիպտի ընթացքում, նույնիսկ եթե հայտարարված են բլոկի ներսում։
   
     ```javascript
     if (true) {
       var x = 10;
     }
     console.log(x); // 10
     ```
   
   - **Hoisting:**
     `var`-ով հայտարարված փոփոխականները "բարձրացվում" են իրենց տիրույթի վերև և ստանում են արժեք `undefined` մինչև դրանց փաստացի հայտարարված լինելը։
   
     ```javascript
     console.log(a); // undefined
     var a = 5;
     ```
   
   - **Կրկնակի հայտարարում:**
     Նույն տիրույթում հնարավոր է կրկնակի հայտարարել փոփոխական `var`-ով՝ առանց սխալի։
   
     ```javascript
     var b = 10;
     var b = 20;
     console.log(b); // 20
     ```
   
   #### 2. `let`
   
   - **Տիրույթ (Scope):**
     `let`-ով հայտարարված փոփոխականները ունեն բլոկային տիրույթ (block scope), ինչը նշանակում է, որ դրանք տեսանելի են միայն իրենց բլոկի ներսում։
   
     ```javascript
     if (true) {
       let y = 10;
     }
     console.log(y); // ReferenceError: y is not defined
     ```
   
   - **Hoisting:**
     Թեև `let`-ով փոփոխականները նույնպես "բարձրացվում" են, դրանք մնում են Temporal Dead Zone (TDZ)-ում մինչև իրական հայտարարված պահը։ Օգտագործելը նախքան հայտարարումը կհանգեցնի ReferenceError-ի։
   
     ```javascript
     console.log(z); // ReferenceError: Cannot access 'z' before initialization
     let z = 15;
     ```
   
   - **Կրկնակի հայտարարում:**
     Նույն տիրույթում `let`-ով փոփոխականները կրկնակի հայտարարել հնարավոր չէ։
   
     ```javascript
     let c = 5;
     let c = 10; // SyntaxError: Identifier 'c' has already been declared
     ```
   
   #### 3. `const`
   
   - **Տիրույթ (Scope):**
     `const`-ով հայտարարված փոփոխականները նույնպես ունեն բլոկային տիրույթ (block scope)։
   
     ```javascript
     if (true) {
       const d = 30;
     }
     console.log(d); // ReferenceError: d is not defined
     ```
   
   - **Hoisting:**
     `const`-ը նույնպես բարձրացվում է, բայց մնում է Temporal Dead Zone (TDZ)-ում մինչև դրա փաստացի հայտարարումը։ Օգտագործումը մինչև հայտարարումը կհանգեցնի ReferenceError-ի։
   
     ```javascript
     console.log(e); // ReferenceError: Cannot access 'e' before initialization
     const e = 25;
     ```
   
   - **Կրկնակի հայտարարում:**
     Նույն տիրույթում `const`-ով փոփոխականները կրկնակի հայտարարել հնարավոր չէ։
   
     ```javascript
     const f = 50;
     const f = 60; // SyntaxError: Identifier 'f' has already been declared
     ```
   
   - **Փոփոխություն:**
     `const`-ով փոփոխականները չեն կարող վերագրվել նոր արժեք։ Սակայն, եթե դրանք օբյեկտ կամ զանգված են, դրանց պարունակությունը կարելի է փոխել։
   
     ```javascript
     const g = 100;
     g = 200; // TypeError: Assignment to constant variable.
   
     const obj = { name: "John" };
     obj.name = "Jane"; // Նորմալ է
     console.log(obj.name); // "Jane"
     ```
   
   ---
   
   ## Ընդհանուր Համեմատություն
   
   | Բանալի Բառ | Տիրույթ | Hoisting | Կրկնակի Հայտարարում | Վերագրման Հնարավորություն |
   |------------|---------|----------|---------------------|---------------------------|
   | `var`      | Ֆունկցիոնալ կամ գլոբալ | Այո, `undefined` արժեքով | Թույլատրվում է          | Թույլատրվում է           |
   | `let`      | Բլոկային              | Այո, բայց TDZ-ում է       | Արգելվում է             | Թույլատրվում է           |
   | `const`    | Բլոկային              | Այո, բայց TDZ-ում է       | Արգելվում է             | Արգելվում է (բացառությամբ օբյեկտների և զանգվածների պարունակության) |
   
   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

13. ### Ինչ է closure-ը JavaScript-ում?
   
   **Closure**-ը JavaScript-ի առանձնահատկություն է, որի միջոցով ֆունկցիան "հիշում" է այն տիրույթը (scope), որտեղ այն ստեղծվել է։ Closure-ը թույլ է տալիս ֆունկցիային մուտք գործել և պահպանել իր արտաքին ֆունկցիայի փոփոխականները, նույնիսկ եթե արտաքին ֆունկցիան ավարտել է իր աշխատանքը։
   
   Closure-ները կարևոր դեր ունեն JavaScript-ում և լայնորեն կիրառվում են օրինակ գաղտնի տվյալներ պահպանելու, կարգաբերման (encapsulation) և callback-ների համար։
   
   ---
   
   #### Ինչպես է աշխատում Closure-ը
   
   Closure ստեղծվում է այն ժամանակ, երբ ներքին ֆունկցիան մուտք է գործում արտաքին ֆունկցիայի փոփոխականներին։
   
   #### Օրինակ 1. Հիմնական Closure
   
   ```javascript
   function outerFunction(outerVariable) {
     return function innerFunction(innerVariable) {
       console.log(`Outer Variable: ${outerVariable}`);
       console.log(`Inner Variable: ${innerVariable}`);
     };
   }
   
   const newFunction = outerFunction("outside");
   newFunction("inside");
   // Output:
   // Outer Variable: outside
   // Inner Variable: inside
   ```
   
   Այս օրինակում `innerFunction`-ը մուտք ունի `outerFunction`-ի փոփոխական `outerVariable`-ին, նույնիսկ եթե `outerFunction`-ն ավարտել է իր աշխատանքը։
   
   ---
   
   #### Օրինակ 2. Գաղտնի տվյալների պահպանում
   
   Closure-ները կարող են օգտագործվել անձնական (private) տվյալներ ստեղծելու համար։
   
   ```javascript
   function secretKeeper(secret) {
     return {
       getSecret: function() {
         return secret;
       },
       setSecret: function(newSecret) {
         secret = newSecret;
       }
     };
   }
   
   const mySecret = secretKeeper("Initial Secret");
   console.log(mySecret.getSecret()); // "Initial Secret"
   mySecret.setSecret("New Secret");
   console.log(mySecret.getSecret()); // "New Secret"
   ```
   
   Այստեղ `secret` փոփոխականը "պաշտպանված" է և հասանելի է միայն `getSecret` և `setSecret` մեթոդների միջոցով։
   
   ---
   
   #### Օրինակ 3. Ցիկլերի և Closure-ների խնդիր
   
   Closure-ները կարող են առաջացնել չնախատեսված վարքագիծ ցիկլերում։
   
   ```javascript
   for (var i = 0; i < 3; i++) {
     setTimeout(function() {
       console.log(i);
     }, 1000);
   }
   // Output:
   // 3
   // 3
   // 3
   ```
   
   Այս խնդիրն առաջանում է, քանի որ `var`-ը չի ստեղծում բլոկային տիրույթ, և բոլոր ֆունկցիաները "հիշում" են նույն փոփոխականը։ Այս խնդիրն ուղղելու համար կարելի է օգտագործել `let` կամ IIFE։
   
   #### `let` լուծում
   ```javascript
   for (let i = 0; i < 3; i++) {
     setTimeout(function() {
       console.log(i);
     }, 1000);
   }
   // Output:
   // 0
   // 1
   // 2
   ```
   
   #### IIFE լուծում
   ```javascript
   for (var i = 0; i < 3; i++) {
     (function(i) {
       setTimeout(function() {
         console.log(i);
       }, 1000);
     })(i);
   }
   // Output:
   // 0
   // 1
   // 2
   ```
   
   ---
   
   #### Closure-ների կարևորությունը
   
   1. **Տվյալների գաղտնիություն և անվտանգություն:**
      Closure-ները թույլ են տալիս պաշտպանել փոփոխականները արտաքին միջավայրից, ստեղծելով վերահսկված հասանելիություն։
   
   2. **Կարգաբերում (Encapsulation):**
      Օգտագործելով closure, դուք կարող եք կառուցել ֆունկցիաներ, որոնք մուտք ունեն միայն անհրաժեշտ տվյալներին՝ ավելորդ մուտքերը կանխելու համար։
   
   3. **Callback-ներ և ասինխրոն ծրագրավորում:**
      Closure-ները կարևոր են callback-ներում և async գործողություններում, քանի որ դրանք թույլ են տալիս պահպանել կոնտեքստը։
   
   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

14. ### Ինչպես է աշխատում "this" բառը JavaScript-ում?
   
   `this` բառը JavaScript-ում ներկայացնում է ֆունկցիայի կատարման համատեքստը (execution context): Այն մատնանշում է այն օբյեկտը, որին ֆունկցիան կապված է։ `this`-ի արժեքը կարող է փոփոխվել՝ կախված այն բանից, թե ինչպես է ֆունկցիան կանչվում։
   
   ---
   
   #### Ինչպես է որոշվում `this`-ի արժեքը
   
   #### 1. Գլոբալ տիրույթում (`global context`)
   
   Գլոբալ տիրույթում `this`-ը մատնանշում է գլոբալ օբյեկտը։
   
   - **Բրաուզերում** `this`-ը մատնանշում է `window` օբյեկտը։
   - **Node.js-ում** `this`-ը մատնանշում է `global` օբյեկտը։
   
   ```javascript
   console.log(this); // Բրաուզերում -> window, Node.js-ում -> global
   ```
   
   #### 2. Օբյեկտի մեթոդում
   
   Մեթոդի ներսում `this`-ը մատնանշում է այն օբյեկտը, որի մաս է մեթոդը։
   
   ```javascript
   const obj = {
     name: "John",
     greet() {
       console.log(this.name);
     }
   };
   obj.greet(); // "John"
   ```
   
   #### 3. Ֆունկցիայի ներսում
   
   Սովորական ֆունկցիայի ներսում (ոչ strict mode-ով)`this`-ը մատնանշում է գլոբալ օբյեկտը։
   
   ```javascript
   function showThis() {
     console.log(this);
   }
   showThis(); // Բրաուզերում -> window, Node.js-ում -> global
   ```
   
   **Strict Mode**-ում `this`-ը կլինի `undefined`։
   
   ```javascript
   'use strict';
   function showThis() {
     console.log(this);
   }
   showThis(); // undefined
   ```
   
   #### 4. Arrow Function-ի ներսում
   
   Arrow ֆունկցիաները **չունեն իրենց սեփական `this` արժեքը**։ Դրանք "ժառանգում" են `this`-ը իրենց արտաքին տիրույթից։
   
   ```javascript
   const obj = {
     name: "Alice",
     greet() {
       const arrowFunc = () => {
         console.log(this.name);
       };
       arrowFunc();
     }
   };
   obj.greet(); // "Alice"
   ```
   
   #### 5. Կառուցիչ Ֆունկցիայում (Constructor Function)
   
   Կառուցիչ ֆունկցիայի ներսում `this`-ը մատնանշում է նոր ստեղծված օբյեկտը։
   
   ```javascript
   function Person(name) {
     this.name = name;
   }
   const person = new Person("Jane");
   console.log(person.name); // "Jane"
   ```
   
   #### 6. Event Listener-ներում
   
   Event Listener-ի ներսում `this`-ը մատնանշում է այն HTML տարրը, որը ակտիվացրել է իրադարձությունը։
   
   ```javascript
   document.querySelector("button").addEventListener("click", function() {
     console.log(this); // Մատնանշում է սեղմված կոճակը
   });
   ```
   
   Arrow ֆունկցիաների դեպքում `this`-ը կլինի արտաքին տիրույթից։
   
   ```javascript
   document.querySelector("button").addEventListener("click", () => {
     console.log(this); // Մատնանշում է արտաքին տիրույթը (օրինակ՝ window)
   });
   ```
   
   ---
   
   #### `this`-ի վերահսկում (Binding)
   
   #### 1. `call()` և `apply()` մեթոդներ
   
   Դուք կարող եք ձեռքով սահմանել `this`-ի արժեքը `call()` կամ `apply()` մեթոդների միջոցով։
   
   ```javascript
   function greet(greeting) {
     console.log(`${greeting}, ${this.name}`);
   }
   const user = { name: "John" };
   
   greet.call(user, "Hello"); // "Hello, John"
   greet.apply(user, ["Hi"]); // "Hi, John"
   ```
   
   #### 2. `bind()` մեթոդ
   
   `bind()` մեթոդը ստեղծում է նոր ֆունկցիա՝ կապված ձեր սահմանած `this`-ի արժեքին։
   
   ```javascript
   const user = { name: "Jane" };
   function greet() {
     console.log(this.name);
   }
   
   const boundGreet = greet.bind(user);
   boundGreet(); // "Jane"
   ```

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

15. ### Ինչ է Event Loop-ը JavaScript-ում?
   **Event Loop**-ը JavaScript-ի կարևոր մեխանիզմներից է, որը կառավարում է, թե ինչպես է լեզուն կատարում բազմաբնույթ գործողություններ (tasks), վերլուծում ասինխրոն կոդը և ապահովում ֆունկցիաների ճիշտ հերթական կատարումը։ Այն հանդիսանում է JavaScript-ի **Single-Threaded, Non-Blocking** բնույթի հիմքը։
   
   Event Loop-ը թույլ է տալիս JavaScript-ին աշխատել ասինխրոն կերպով՝ չընդհատելով հիմնական թելի (main thread) աշխատանքը։
   
   ---
   
   #### Ինչպես է աշխատում Event Loop-ը
   
   #### 1. Call Stack (Call Stack)
   
   Call Stack-ը JavaScript-ի կառուցվածք է, որը հետևում է այն ֆունկցիաներին, որոնք սպասում են իրենց կատարումը։ Երբ ֆունկցիա կանչվում է, այն ավելացվում է stack-ի վերևում, իսկ երբ ավարտվում է, հանվում է stack-ից։
   
   ```javascript
   function first() {
     console.log("First");
   }
   function second() {
     first();
     console.log("Second");
   }
   second();
   // Output:
   // First
   // Second
   ```
   
   #### 2. Web API-ներ և Task Queue
   
   Բրաուզերը կամ Node.js-ն ապահովում են **Web API**-ներ (օրինակ՝ `setTimeout`, `fetch`), որոնք աշխատում են Call Stack-ից դուրս։ Web API-ներն են՝
   
   - `setTimeout` և `setInterval` - նախատեսված են ժամանակի վրա հիմնված գործառույթների համար։
   - `XMLHttpRequest` և `fetch` - աշխատում են HTTP հարցումների հետ։
   - DOM իրադարձությունները (օրինակ՝ click, input)։
   
   Երբ Web API-ները ակտիվանում են (օրինակ՝ timer-ը ավարտվում է կամ հարցման պատասխանը ստացվում է), դրանք ավարտված առաջադրանքը տեղափոխում են Task Queue (կամ Microtask Queue՝ կախված տիպից)։
   
   ```javascript
   console.log("Start");
   setTimeout(() => {
     console.log("Timeout");
   }, 1000);
   console.log("End");
   // Output:
   // Start
   // End
   // Timeout
   ```
   
   #### 3. Event Loop-ի դերը
   
   Event Loop-ը հետևում է Call Stack-ին և Task Queue-ին։ Երբ Call Stack-ը դատարկ է, Event Loop-ը վերցնում է Task Queue-ի առաջին առաջադրանքը և ավելացնում է այն Call Stack-ի մեջ՝ կատարելու համար։
   
   ---
   
   #### Միկրոտասկեր և Մակրոտասկեր
   
   JavaScript-ի ասինխրոն առաջադրանքները բաժանվում են երկու կատեգորիայի՝ **Microtasks** և **Macrotasks**։
   
   #### 1. Մակրոտասկեր (Macrotasks)
   
   Մակրոտասկերը ներառում են մեծածավալ աշխատանքներ, որոնք բրաուզերն ավելացնում է Task Queue-ի մեջ։ Դրանք ներառում են՝
   - `setTimeout`
   - `setInterval`
   - `setImmediate` (հասանելի է Node.js-ում)
   - DOM իրադարձությունները (օրինակ՝ click, input)
   
   Macrotask-ը տեղափոխվում է Task Queue և սպասում է, մինչ Call Stack-ը դատարկ կլինի։
   
   #### 2. Միկրոտասկեր (Microtasks)
   
   Միկրոտասկերը փոքր առաջադրանքներ են, որոնք կատարում են ավելի բարձր առաջնահերթությամբ՝ նախքան Macrotask-երը։ Դրանք ներառում են՝
   - `Promises` (կամ `Promise.then`)
   - `MutationObserver`
   - `queueMicrotask` (օգտագործվում է ուղղակի միկրոտասկ ստեղծելու համար)
   
   Միկրոտասկերն ավելացվում են Microtask Queue-ում և կատարվում են հենց որ Call Stack-ը դատարկ է՝ նախքան հաջորդ Macrotask-ի մեկնարկը։
   
   ```javascript
   console.log("Start");
   setTimeout(() => console.log("Macrotask"), 0);
   Promise.resolve().then(() => console.log("Microtask"));
   console.log("End");
   // Output:
   // Start
   // End
   // Microtask
   // Macrotask
   ```
   
   ---
   
   #### Web API-ների աշխատանքի մանրամասները
   
   1. **Timer (setTimeout, setInterval):**
      - Timer-ը սկսում է աշխատել Web API-ում։ Երբ ժամանակը լրանում է, callback-ը տեղափոխվում է Macrotask Queue։
   
   2. **Promises:**
      - Promise-ի արդյունքը (`.then`, `.catch`, `.finally`) ուղարկվում է Microtask Queue։
   
   3. **DOM իրադարձություններ:**
      - Սկսած click-ից մինչև input իրադարձություններ, դրանք տեղադրվում են Macrotask Queue-ում։
   
   4. **Network Requests (fetch, XMLHttpRequest):**
      - Երբ հարցման պատասխանը ստացվում է, callback-ը տեղափոխվում է Macrotask Queue։
   
   ---
   
   #### Հոսքի գործընթաց
   
   1. Call Stack-ում սինխրոն կոդի կատարում։
   2. Ասինխրոն գործողությունները (օրինակ՝ `setTimeout`, `fetch`) տեղափոխվում են Web API-ներ։
   3. Արդյունքները վերադարձվում են Task Queue կամ Microtask Queue։
   4. Event Loop-ը ստուգում է Microtask Queue-ը։ Եթե այն դատարկ չէ, կատարում է Microtask-երը։
   5. Եթե Microtask Queue-ը դատարկ է, Event Loop-ը անցնում է Task Queue-ին։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

16. ### Ինչ է debounce-ը և throttle-ը JavaScript-ում?
   `debounce` և `throttle` տեխնիկաները օգտագործվում են JavaScript-ում բարձր հաճախականությամբ իրադարձությունների (high-frequency events) օպտիմալացման համար։ Դրանք կարևոր են այն դեպքերում, երբ իրադարձությունները կարող են կանչվել շատ հաճախ և հանգեցնել կատարողականության անկման։
   
   - **Debounce**: Կատարման հաճախականությունը սահմանափակելու մեթոդ, որը թույլ է տալիս ֆունկցիան կանչվել միայն այն ժամանակ, երբ որոշակի ժամանակահատվածում այլ կանչ չի եղել։
   - **Throttle**: Կատարման հաճախականությունը սահմանափակելու մեթոդ, որը թույլ է տալիս ֆունկցիան կանչվել ֆիքսված միջակայքով՝ անկախ իրադարձությունների հաճախականությունից։
   
   ---
   
   #### Debounce-ի աշխատանքը
   
   **Debounce**-ը երաշխավորում է, որ ֆունկցիան կկատարվի միայն այն դեպքում, եթե իրադարձությունը որոշակի ժամանակահատվածում կրկին չկատարվի։
   
   #### Օրինակ:
   Երբեմն անհրաժեշտ է ֆունկցիան կանչել միայն այն ժամանակ, երբ օգտատերը դադարում է մուտքագրումը:
   
   ```javascript
   function debounce(func, delay) {
     let timer;
     return function(...args) {
       clearTimeout(timer);
       timer = setTimeout(() => func.apply(this, args), delay);
     };
   }
   
   const logMessage = debounce(() => {
     console.log("Input stopped");
   }, 300);
   
   document.getElementById("input").addEventListener("keyup", logMessage);
   ```
   
   - **Ինչպես է աշխատում:**
   - Ամեն անգամ, երբ իրադարձությունը կանչվում է, նախորդ `setTimeout`-ը մաքրվում է (clearTimeout):
   - Եթե ժամանակային միջակայքում այլ կանչ չի լինում, ֆունկցիան կատարվում է։
   
   #### Օգտագործման դեպքեր:
   - Input դաշտում մուտքագրման հետ կապված իրադարձություններ։
   - Window-ի չափսի փոփոխման (resize) իրադարձություններ։
   
   ---
   
   #### Throttle-ի աշխատանքը
   
   **Throttle**-ը երաշխավորում է, որ ֆունկցիան կկատարվի ֆիքսված ժամանակահատվածում մեկ անգամ՝ անկախ իրադարձության հաճախականությունից։
   
   #### Օրինակ:
   Անհրաժեշտ է վերահսկել window-ի scroll իրադարձությունը՝ առանց ֆունկցիան հաճախ կանչելու:
   
   ```javascript
   function throttle(func, interval) {
     let lastCall = 0;
     return function(...args) {
       const now = Date.now();
       if (now - lastCall >= interval) {
         lastCall = now;
         func.apply(this, args);
       }
     };
   }
   
   const logScroll = throttle(() => {
     console.log("Scrolled");
   }, 1000);
   
   window.addEventListener("scroll", logScroll);
   ```
   
   - **Ինչպես է աշխատում:**
   - Ֆունկցիան կատարում է միայն այն դեպքում, երբ ֆիքսված ժամանակահատվածն անցել է նախորդ կանչից։
   
   #### Օգտագործման դեպքեր:
   - Scroll իրադարձություններ։
   - Button-ի հաճախակի սեղմումների վերահսկում։
   
   ---
   
   #### Տարբերությունը `debounce`-ի և `throttle`-ի միջև
   
   | **Նկարագրություն**            | **Debounce**                                   | **Throttle**                       |
   |--------------------------------|-----------------------------------------------|-------------------------------------|
   | **Նպատակ**                    | Կատարել ֆունկցիան միայն իրադարձության դադարից հետո։| Կատարել ֆունկցիան ֆիքսված միջակայքով։ |
   | **Կիրառման դեպքեր**            | Input դաշտի իրադարձություններ։                | Scroll կամ resize իրադարձություններ։ |
   | **Կատարում հաճախականությամբ**  | Փոքր հաճախականությամբ։                         | Ֆիքսված ժամանակային միջակայքով։      |

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

17. ### Ինչ է Promise-ը և ինչպես է այն աշխատում?
   
   **Promise**-ը JavaScript-ում օբյեկտ է, որը ներկայացնում է ապագայում կատարվող կամ չկատարվող գործողություն։ Այն կարևոր գործիք է ասինխրոն ծրագրավորման համար և թույլ է տալիս մշակել գործողությունների հաջորդականությունը՝ առանց callback-ների խառնաշփոթի (callback hell):
   
   Promise-ը կարող է ունենալ երեք վիճակ՝
   1. **Pending (սպասող):** Սկզբնական վիճակ, երբ գործողությունը դեռ չի ավարտվել։
   2. **Fulfilled (կատարված):** Գործողությունը հաջողությամբ ավարտվել է, և արդյունքն հասանելի է։
   3. **Rejected (մերժված):** Գործողությունը ձախողվել է, և սխալի պատճառը հասանելի է։
   
   ---
   
   #### Ինչպես է աշխատում Promise-ը
   
   #### 1. Ստեղծում և կառուցվածք
   
   Promise-ը ստեղծվում է `Promise` կոնստրուկտորի միջոցով, որը որպես արգումենտ ընդունում է **executor** ֆունկցիա։ Այս ֆունկցիան ունի երկու պարամետր՝ `resolve` և `reject`, որոնք օգտագործվում են արդյունքը վերադարձնելու կամ սխալը նշելու համար։
   
   ```javascript
   const myPromise = new Promise((resolve, reject) => {
     let success = true;
   
     if (success) {
       resolve("Task completed successfully");
     } else {
       reject("Task failed");
     }
   });
   ```
   
   #### 2. `then`, `catch` և `finally` մեթոդներ
   
   Promise-ը ունի հետևյալ մեթոդները՝
   
   - **`then`:** Կատարվում է, երբ Promise-ը `fulfilled` վիճակում է։
   - **`catch`:** Կատարվում է, երբ Promise-ը `rejected` վիճակում է։
   - **`finally`:** Կատարվում է անկախ արդյունքից։
   
   ```javascript
   myPromise
     .then(result => {
       console.log(result); // "Task completed successfully"
     })
     .catch(error => {
       console.log(error); // "Task failed"
     })
     .finally(() => {
       console.log("Promise settled");
     });
   ```
   
   #### 3. Ասինխրոն գործողություններ
   
   Promise-ը հաճախ օգտագործվում է ասինխրոն գործողությունների համար, օրինակ՝ API հարցումներ:
   
   ```javascript
   const fetchData = new Promise((resolve, reject) => {
     setTimeout(() => {
       const data = { id: 1, name: "John" };
       resolve(data);
     }, 2000);
   });
   
   fetchData
     .then(response => {
       console.log(response); // { id: 1, name: "John" }
     })
     .catch(error => {
       console.log(error);
     });
   ```
   
   ---
   
   #### Promise-ի շղթայականություն (Chaining)
   
   Promise-ների շղթայականությունը թույլ է տալիս կատարել հաջորդական գործողություններ՝ օգտագործելով `then` մեթոդը:
   
   ```javascript
   fetchData
     .then(response => {
       console.log(response.name); // "John"
       return response.id;
     })
     .then(id => {
       console.log(`ID is ${id}`); // "ID is 1"
     })
     .catch(error => {
       console.log(error);
     });
   ```
   
   ---
   
   #### Promise.all, Promise.race և Promise.allSettled
   
   #### 1. **`Promise.all`**
   
   `Promise.all` մեթոդը կատարում է մի քանի Promise-ներ զուգահեռ և վերադարձնում է արդյունքները, երբ բոլորն ավարտվել են։ Եթե որևէ մեկը ձախողվի, ամբողջը մերժվում է։
   
   ```javascript
   const p1 = Promise.resolve(1);
   const p2 = Promise.resolve(2);
   const p3 = Promise.resolve(3);
   
   Promise.all([p1, p2, p3])
     .then(results => {
       console.log(results); // [1, 2, 3]
     })
     .catch(error => {
       console.log(error);
     });
   ```
   
   #### 2. **`Promise.race`**
   
   `Promise.race` մեթոդը վերադարձնում է առաջին ավարտված Promise-ի արդյունքը։
   
   ```javascript
   const p1 = new Promise(resolve => setTimeout(() => resolve("P1"), 1000));
   const p2 = new Promise(resolve => setTimeout(() => resolve("P2"), 500));
   
   Promise.race([p1, p2])
     .then(result => {
       console.log(result); // "P2"
     });
   ```
   
   #### 3. **`Promise.allSettled`**
   
   `Promise.allSettled` մեթոդը սպասում է, որ բոլոր Promise-ները ավարտվեն, անկախ դրանց վիճակից։
   
   ```javascript
   const p1 = Promise.resolve("Success");
   const p2 = Promise.reject("Error");
   
   Promise.allSettled([p1, p2])
     .then(results => {
       console.log(results);
       // [
       //   { status: "fulfilled", value: "Success" },
       //   { status: "rejected", reason: "Error" }
       // ]
     });
   ```
   
   ---
   
   #### Promise-ի առավելությունները
   
   1. **Callback Hell-ի նվազեցում:**
      Promise-ները թույլ են տալիս կառավարել callback-ների բարդությունը՝ օգտագործելով շղթայականություն։
   
   2. **Կոդի ընթեռնելիություն:**
      Promise-ները ավելի ընթեռնելի և կանխատեսելի են դարձնում ասինխրոն կոդը։
   
   3. **Զուգահեռ գործողություններ:**
      Promise-ները թույլ են տալիս հեշտությամբ աշխատել միաժամանակ մի քանի ասինխրոն գործողությունների հետ։
   
   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

18. ### Ինչպես է աշխատում async/await-ը JavaScript-ում?


**`async/await`**-ը JavaScript-ի կառուցվածք է, որը տրամադրում է ավելի ընթեռնելի սինտաքս Promise-ների հետ աշխատելու համար։ Այն թույլ է տալիս գրել ասինխրոն կոդ, որը կարդացվում է ինչպես սինխրոն կոդ։
   
   - **`async` ֆունկցիան**: Վերադարձնում է `Promise`։
   - **`await` օպերատորը**: Օգտագործվում է `Promise`-ների լուծման (`resolve`) արդյունքը սպասելու համար։
   
   ---
   
   #### Ինչպես է աշխատում async/await-ը
   
   #### 1. `async`-ի աշխատանքը
   
   Ֆունկցիան, որը հայտարարվում է `async` բառով, ավտոմատ կերպով վերադարձնում է `Promise`։
   
   ```javascript
   async function greet() {
     return "Hello, World!";
   }
   
   greet().then(message => console.log(message)); // "Hello, World!"
   ```
   
   Եթե `async` ֆունկցիայի ներսում սխալ է նետվում (`throw`), այդ սխալը փոխանցվում է որպես մերժված (rejected) `Promise`:
   
   ```javascript
   async function throwError() {
     throw new Error("Something went wrong!");
   }
   
   throwError().catch(error => console.log(error.message)); // "Something went wrong!"
   ```
   
   #### 2. `await`-ի աշխատանքը
   
   `await`-ը ստիպում է `async` ֆունկցիային սպասել `Promise`-ի լուծմանը։
   
   ```javascript
   async function fetchData() {
     const data = await new Promise(resolve => {
       setTimeout(() => resolve("Data received!"), 2000);
     });
     console.log(data);
   }
   
   fetchData();
   // Output (2 վայրկյանից հետո):
   // "Data received!"
   ```
   
   ---
   
   #### Օրինակ՝ API հարցման հետ
   
   ```javascript
   async function getUserData() {
     try {
       const response = await fetch("https://jsonplaceholder.typicode.com/users/1");
       const data = await response.json();
       console.log(data);
     } catch (error) {
       console.error("Error fetching data:", error);
     }
   }
   
   getUserData();
   ```
   
   ---
   
   #### Generators և Async/Await-ի կապը
   
   **Generators**-ը JavaScript-ի ֆունկցիաներ են, որոնք կարող են դադարեցնել իրենց կատարումը (`yield`) և շարունակել այն՝ ապահովելով ասինխրոն ծրագրավորման հիմքը։
   
   `async/await`-ը կառուցվել է Generators-ի գաղափարի վրա, բայց տալիս է ավելի պարզ սինտաքս։
   
   #### Generators-ի աշխատանքը
   
   ```javascript
   function* generatorFunction() {
     yield "Step 1";
     yield "Step 2";
     return "Step 3";
   }
   
   const generator = generatorFunction();
   console.log(generator.next()); // { value: "Step 1", done: false }
   console.log(generator.next()); // { value: "Step 2", done: false }
   console.log(generator.next()); // { value: "Step 3", done: true }
   ```
   
   Generators-ը թույլ է տալիս ստեղծել ֆունկցիաներ, որոնք կարող են դադարեցնել իրենց ընթացքը՝ ասինխրոն տրամաբանության կառավարումը հեշտացնելու համար։
   
   ```javascript
   function* asyncGenerator() {
     const data = yield fetch("https://jsonplaceholder.typicode.com/users/1");
     console.log(data);
   }
   
   const gen = asyncGenerator();
   const promise = gen.next().value;
   promise
     .then(response => response.json())
     .then(data => gen.next(data));
   ```
   
   ---
   
   #### Async/Await-ի առավելությունները
   
   1. **Կոդի ընթեռնելիություն**:
      - `async/await`-ը ավելի ընթեռնելի է և հեշտ է հասկանալ, քան Promise-ների շղթայականությունը։
   
   2. **Սխալի կառավարում**:
      - `try/catch` բլոկները հեշտացնում են սխալների կառավարումը։
   
   3. **Generational գաղափարների պարզեցում**:
      - `async/await`-ը փոխարինում է Generators-ի բարդ սինտաքսը։


   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

19. ### Ինչ է DOM-ը և ինչ տարբերություն կա HTML-ի և DOM-ի միջև?
**DOM (Document Object Model)**-ը ծրագրային ինտերֆեյս է, որը ներկայացնում է HTML կամ XML փաստաթղթի կառուցվածքը ծառի տեսքով։ DOM-ը հնարավորություն է տալիս ծրագրավորողներին փոխել, ավելացնել կամ հեռացնել փաստաթղթի տարրերը ծրագրային մակարդակում։
   
   HTML-ը փաստաթղթի նշագրման լեզուն է, մինչդեռ DOM-ը դրա ծրագրային ներկայացումն է։
   
   ---
   
   #### Ինչ է DOM-ը
   
   1. **Ծառի կառուցվածք:**
      DOM-ը փաստաթղթի ամբողջական կառուցվածքը ներկայացնում է որպես ծառ՝ բաղկացած **ծնող (parent)**, **զավակ (child)** և **եղբայր (sibling)** հարաբերություններով։
   
   2. **Փոխազդեցություն:**
      DOM-ը թույլ է տալիս JavaScript-ին փոխազդել HTML-ի հետ՝ փոփոխելով տարրերը, ստիլերը, կամ իրադարձությունները։
   
   3. **Կենդանի ներկայացում:**
      DOM-ը "կենդանի" է, ինչը նշանակում է, որ ցանկացած փոփոխություն HTML փաստաթղթում անմիջապես անդրադառնում է DOM-ի վրա և հակառակը։
   
   ```html
   <!DOCTYPE html>
   <html>
     <head>
       <title>DOM Example</title>
     </head>
     <body>
       <h1>Hello, World!</h1>
       <p>This is a paragraph.</p>
     </body>
   </html>
   ```
   
   DOM-ը վերածում է վերևի HTML փաստաթղթին հետևյալ ծառի:
   
   ```
   <html>
   ├── <head>
   │   ├── <title> "DOM Example"
   ├── <body>
       ├── <h1> "Hello, World!"
       ├── <p> "This is a paragraph."
   ```
   
   ---
   
   #### HTML-ի և DOM-ի տարբերությունները
   
   | **Հատկանիշ**               | **HTML**                                           | **DOM**                                      |
   |-----------------------------|----------------------------------------------------|---------------------------------------------|
   | **Սահմանում**               | Թեգերի և բովանդակության նշագրման լեզու։           | HTML-ի ծրագրային ներկայացումը։              |
   | **Նպատակ**                 | Բրաուզերի համար կառուցվածքի ստեղծում։             | Ծրագրերի համար փաստաթղթի կառավարման միջոց։ |
   | **Կառուցվածք**              | Տեքստային ձևով։                                  | Ծառի կառուցվածք։                            |
   | **Փոփոխություն**            | Փոփոխվում է միայն տեքստային ֆայլում։              | Կարող է փոփոխվել JavaScript-ի միջոցով։     |
   | **Տեսանելիություն**          | Փաստաթուղթը բրաուզերում։                         | Փաստաթուղթը ծրագրային մակարդակում։          |
   
   ---
   
   #### Ինչպես է աշխատում DOM-ը
   
   #### 1. **Տարբեր մակարդակներ**
   
   DOM-ը բաղկացած է երեք հիմնական մակարդակներից՝
   
   - **Element Level (Տարրային մակարդակ):** HTML թեգերը, օրինակ՝ `<div>`, `<p>`։
   - **Attribute Level (Ատրիբուտային մակարդակ):** HTML թեգերի ատրիբուտները, օրինակ՝ `class`, `id`։
   - **Text Level (Տեքստային մակարդակ):** Տեքստը, որը տեղակայված է թեգերի ներսում։
   
   ```javascript
   const element = document.querySelector("h1");
   console.log(element.textContent); // "Hello, World!"
   ```
   
   #### 2. **Փոփոխություն DOM-ում**
   
   JavaScript-ը կարող է օգտագործվել DOM-ի տարրերը փոխելու համար՝ ավելացնելով, հեռացնելով կամ փոփոխելով դրանք։
   
   ```javascript
   // Փոխել տեքստը
   const heading = document.querySelector("h1");
   heading.textContent = "Hello, DOM!";
   
   // Ավելացնել նոր տարր
   const paragraph = document.createElement("p");
   paragraph.textContent = "This is a new paragraph.";
   document.body.appendChild(paragraph);
   
   // Հեռացնել տարր
   const oldParagraph = document.querySelector("p");
   document.body.removeChild(oldParagraph);
   ```
   
   #### 3. **Իրադարձություններ (Events):**
   
   DOM-ը նաև աջակցում է իրադարձությունների կառավարմանը, օրինակ՝ սեղմումներ, շարժումներ և այլն։
   
   ```javascript
   const button = document.querySelector("button");
   button.addEventListener("click", () => {
     alert("Button clicked!");
   });
   ```
   
   ---
   
   #### DOM-ի առավելություններ
   
   1. **Դինամիկ բովանդակություն:**
      Թույլ է տալիս դինամիկ փոխել փաստաթուղթը՝ առանց այն վերալցելու։
   
   2. **Իրադարձությունների կառավարում:**
      Թույլ է տալիս հեշտությամբ կառավարել իրադարձությունները բրաուզերի մեջ։
   
   3. **Ավտոմատ թարմացում:**
      Փոփոխությունները անմիջապես արտացոլվում են փաստաթղթում։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

20. ### Ինչ է ES6 մոդուլը և ինչպես է այն աշխատում?
**ES6 մոդուլները** (Modules) JavaScript-ում ներկայացնում են կոդի վերաօգտագործման (reuse) և կոդի կառուցվածքի (organization) արդիական մեխանիզմ։ Մոդուլները թույլ են տալիս բաժանել կոդը տարբեր ֆայլերի և վերահսկել, թե որոնք են ներմուծվում և արտահանվում։
   
   ES6 մոդուլները հանդիսանում են JavaScript-ի ստանդարտ մասը ECMAScript 2015 (ES6)-ից սկսած և ապահովում են հստակ կառուցվածք մեծ ծրագրերում։

---
   
   #### Ինչպես են աշխատում ES6 մոդուլները
   
   #### 1. Մոդուլի արտահանում (`export`)
   
   `export` բանալի բառը օգտագործվում է մոդուլի ներսում փոփոխականներ, ֆունկցիաներ կամ դասեր արտահանելու համար։ Կան երկու հիմնական տեսակ՝ **Named Export** և **Default Export**։
   
   #### Named Export
   
   Named Export-ը թույլ է տալիս արտահանել մի քանի փոփոխականներ կամ ֆունկցիաներ նույն ֆայլից։
   
   ```javascript
   // math.js
   export const add = (a, b) => a + b;
   export const subtract = (a, b) => a - b;
   ```
   
   #### Default Export
   
   Default Export-ը թույլ է տալիս արտահանել մեկ հիմնական արժեք։
   
   ```javascript
   // message.js
   export default function greet(name) {
     return `Hello, ${name}!`;
   }
   ```
   
   #### 2. Մոդուլի ներմուծում (`import`)
   
   `import` բանալի բառը օգտագործվում է մեկ այլ մոդուլից արտահանված արժեքները ներմուծելու համար։
   
   #### Named Import
   
   ```javascript
   // main.js
   import { add, subtract } from './math.js';
   
   console.log(add(5, 3)); // 8
   console.log(subtract(5, 3)); // 2
   ```
   
   #### Default Import
   
   ```javascript
   // main.js
   import greet from './message.js';
   
   console.log(greet("John")); // "Hello, John!"
   ```
   
   #### Named և Default համակցված Import
   
   ```javascript
   // main.js
   import greet, { add } from './math.js';
   
   console.log(greet("John"));
   console.log(add(10, 5));
   ```
   
   #### 3. Import Everything
   
   Եթե անհրաժեշտ է ներմուծել մոդուլի բոլոր արտահանված արժեքները, կարող եք օգտագործել `* as` սինտաքսը։
   
   ```javascript
   // main.js
   import * as math from './math.js';
   
   console.log(math.add(5, 3)); // 8
   console.log(math.subtract(5, 3)); // 2
   ```
   
   ---
   
   #### ES6 մոդուլների առանձնահատկությունները
   
   1. **Մեկուսացված տիրույթ (Scope):**
      Մոդուլում հայտարարված բոլոր փոփոխականները և ֆունկցիաները մեկուսացված են և հասանելի չեն գլոբալ տիրույթում։
   
   2. **Կոդի լազերային բեռնավորում (Lazy Loading):**
      Մոդուլները բեռնվում են միայն այն ժամանակ, երբ անհրաժեշտ է։
   
   3. **Statically Analyzable:**
      ES6 մոդուլները թույլ են տալիս տրանսպիլյատորներին և գործիքներին հեշտությամբ վերլուծել կախվածությունները։
   
   4. **Մեկ մոդուլ, մեկ ֆայլ:**
      Ամեն մոդուլ սովորաբար գտնվում է առանձին ֆայլում, ինչը հեշտացնում է կոդի կազմակերպումը։
   
   ---
   
   #### Browser Support
   
   ES6 մոդուլները աջակցվում են ժամանակակից բրաուզերներում՝ առանց տրանսպիլյացիայի։ Դուք կարող եք օգտագործել `<script type="module">` թեգը՝ բրաուզերում մոդուլներ բեռնելու համար։
   
   ```html
   <script type="module">
     import { add } from './math.js';
     console.log(add(5, 5));
   </script>
   ```

---
   
   #### CommonJS vs ES6 Modules
   
   | **Հատկանիշ**               | **CommonJS (Node.js)**                        | **ES6 Modules**                      |
   |-----------------------------|-----------------------------------------------|---------------------------------------|
   | **Սինտաքս**                | `require`, `module.exports`                  | `import`, `export`                   |
   | **Բեռնավորում**            | Սինխրոն                                      | Ասինխրոն                             |
   | **Բրաուզերային աջակցություն** | Չի աջակցվում                                  | Աջակցվում է                           |
   | **Statically Analyzable**   | Ոչ                                           | Այո                                   |

---
   
   #### Օրինակ՝ կիրառություն
   
   #### math.js
   ```javascript
   export const multiply = (a, b) => a * b;
   export const divide = (a, b) => a / b;
   ```
   
   #### main.js
   ```javascript
   import { multiply, divide } from './math.js';
   
   console.log(multiply(6, 3)); // 18
   console.log(divide(6, 3));   // 2
   ```

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

21. ### Ինչ է JavaScript-ում call, apply, bind մեթոդները?
   
`call`, `apply` և `bind` մեթոդները JavaScript-ի ֆունկցիոնալ մեթոդներ են, որոնք թույլ են տալիս կառավարել, թե ինչպես է ֆունկցիան կատարում իր **`this`** կոնտեքստը։ Դրանք բոլորն էլ թույլ են տալիս փոխել ֆունկցիայի կանչի համատեքստը՝ վերահսկելով, թե որ օբյեկտը պետք է դառնա `this`։

---
   
   #### 1. `call()`
   
   `call` մեթոդը անմիջապես կանչում է ֆունկցիան և թույլ է տալիս առաջին արգումենտով սահմանել `this`-ի արժեքը։ Հաջորդ արգումենտները փոխանցվում են ֆունկցիային որպես առանձին արժեքներ։
   
   #### Օրինակ
   
   ```javascript
   function greet(greeting, punctuation) {
     console.log(`${greeting}, ${this.name}${punctuation}`);
   }
   
   const user = { name: "John" };
   
   greet.call(user, "Hello", "!");
   // Output: "Hello, John!"
   ```
   
   #### Գործառույթներ
   - Կանչում է ֆունկցիան անմիջապես։
   - Արգումենտները փոխանցվում են առանձին-առանձին։
   
   ---
   
   #### 2. `apply()`
   
   `apply` մեթոդը նույնպես անմիջապես կանչում է ֆունկցիան, բայց արգումենտները փոխանցվում են որպես զանգված։
   
   #### Օրինակ
   
   ```javascript
   function greet(greeting, punctuation) {
     console.log(`${greeting}, ${this.name}${punctuation}`);
   }
   
   const user = { name: "Jane" };
   
   greet.apply(user, ["Hi", "!"]);
   // Output: "Hi, Jane!"
   ```
   
   #### Գործառույթներ
   - Կանչում է ֆունկցիան անմիջապես։
   - Արգումենտները փոխանցվում են զանգվածի տեսքով։
   
   ---
   
   #### 3. `bind()`
   
   `bind` մեթոդը չի կանչում ֆունկցիան անմիջապես։ Այն վերադարձնում է նոր ֆունկցիա, որի `this`-ը կապված է տրված արժեքին։
   
   #### Օրինակ
   
   ```javascript
   function greet(greeting, punctuation) {
     console.log(`${greeting}, ${this.name}${punctuation}`);
   }
   
   const user = { name: "Alice" };
   
   const boundGreet = greet.bind(user);
   boundGreet("Hey", "...");
   // Output: "Hey, Alice..."
   ```
   
   #### Գործառույթներ
   - Վերադարձնում է նոր ֆունկցիա՝ կապված նոր `this`-ով։
   - Կարելի է կանչել երբ ուզեք։
   
   ---
   
   #### Տարբերությունները
   
   | **Հատկանիշ**               | **`call`**                               | **`apply`**                              | **`bind`**                                |
   |-----------------------------|-------------------------------------------|-------------------------------------------|-------------------------------------------|
   | **Կանչում է ֆունկցիան**    | Այո                                      | Այո                                      | Ոչ                                       |
   | **Արգումենտների ձևը**      | Առանձին-առանձին                          | Զանգվածով                                | Առանձին-առանձին (կապված ֆունկցիայում)    |
   | **Վերադարձնում է**          | Ֆունկցիայի արդյունքը                      | Ֆունկցիայի արդյունքը                      | Նոր ֆունկցիա                              |
   
   ---
   
   #### Ինչպես են դրանք կապված միմյանց հետ
   
   - **`call`-ը** և **`apply`-ը** շատ նման են։ Տարբերությունն այն է, որ `call`-ը արգումենտները փոխանցում է առանձին-առանձին, իսկ `apply`-ը՝ զանգվածի տեսքով։
   - **`bind`-ը** տարբերվում է նրանով, որ ֆունկցիան անմիջապես չի կանչում, այլ վերադարձնում է նոր ֆունկցիա։
   
   ---
   
   #### Օգտագործման դեպքեր
   
   1. **Կոնտեքստի կառավարում:**
   
   ```javascript
   const obj = {
     x: 42,
     getX: function() {
       return this.x;
     }
   };
   
   const getX = obj.getX;
   console.log(getX()); // undefined (կոնտեքստը կորցված է)
   
   const boundGetX = getX.bind(obj);
   console.log(boundGetX()); // 42
   ```
   
   2. **Վերաօգտագործում տարբեր օբյեկտների համար:**
   
   ```javascript
   function introduce() {
     console.log(`My name is ${this.name}`);
   }
   
   const userOne = { name: "Alice" };
   const userTwo = { name: "Bob" };
   
   introduce.call(userOne); // "My name is Alice"
   introduce.call(userTwo); // "My name is Bob"
   ```
   
   3. **Մաթեմատիկական հաշվարկներ (apply):**
   
   ```javascript
   const numbers = [5, 6, 2, 3, 7];
   
   console.log(Math.max.apply(null, numbers)); // 7
   console.log(Math.min.apply(null, numbers)); // 2
   ```

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

22. ### Ինչ է `map`, `filter` և `reduce` մեթոդները JavaScript-ում?

   JavaScript-ում `map`, `filter` և `reduce` մեթոդները օգտագործվում են զանգվածների (arrays) վրա գործողությունների համար։ Դրանք օգնում են գրել կարճ, ընթեռնելի և ֆունկցիոնալ կոդ՝ զերծ մանուալ լուպերից։
   
   - **`map`**: Արտացոլում է զանգվածը՝ վերադարձնելով նոր զանգված, որի յուրաքանչյուր տարր հաշվարկվում է callback ֆունկցիայի միջոցով։
   - **`filter`**: Վերադարձնում է նոր զանգված, որը պարունակում է միայն այն տարրերը, որոնք անցնում են callback ֆունկցիայի տրամաբանական ստուգումը։
   - **`reduce`**: Սեղմում է (reduce) զանգվածը մեկ արժեքի՝ օգտագործելով callback ֆունկցիան։
   
   ---
   
   #### 1. `map` մեթոդը
   
   #### Ինչպես է աշխատում
   
   `map` մեթոդը աշխատում է այնպես, որ ստեղծում է նոր զանգված՝ ի սկզբանե կանչելով callback ֆունկցիան յուրաքանչյուր տարրի վրա։
   
   ```javascript
   const numbers = [1, 2, 3, 4];
   
   const squared = numbers.map(num => num * num);
   console.log(squared); // [1, 4, 9, 16]
   ```
   
   #### Սինտաքս
   ```javascript
   array.map((currentValue, index, array) => {
     // Վերադարձնում է նոր արժեք
   });
   ```
   
   - **currentValue**: Զանգվածի ընթացիկ տարրը։
   - **index**: Ընթացիկ տարրի ինդեքսը։
   - **array**: Բուն զանգվածը։
   
   #### Օրինակ՝ անունների մեծատառ փոխակերպում
   
   ```javascript
   const names = ["alice", "bob", "charlie"];
   
   const uppercased = names.map(name => name.toUpperCase());
   console.log(uppercased); // ["ALICE", "BOB", "CHARLIE"]
   ```
   
   ---
   
   #### 2. `filter` մեթոդը
   
   #### Ինչպես է աշխատում
   
   `filter` մեթոդը վերադարձնում է նոր զանգված՝ ներառելով միայն այն տարրերը, որոնք բավարարում են callback ֆունկցիայի տրամաբանական պայմանը։
   
   ```javascript
   const numbers = [10, 15, 20, 25];
   
   const evenNumbers = numbers.filter(num => num % 2 === 0);
   console.log(evenNumbers); // [10, 20]
   ```
   
   ### Սինտաքս
   ```javascript
   array.filter((currentValue, index, array) => {
     // Վերադարձնում է true կամ false
   });
   ```
   
   - **currentValue**: Զանգվածի ընթացիկ տարրը։
   - **index**: Ընթացիկ տարրի ինդեքսը։
   - **array**: Բուն զանգվածը։
   
   #### Օրինակ՝ մեծ թվերի ֆիլտրացում
   
   ```javascript
   const numbers = [5, 10, 15, 20];
   
   const greaterThan10 = numbers.filter(num => num > 10);
   console.log(greaterThan10); // [15, 20]
   ```
   
   ---
   
   #### 3. `reduce` մեթոդը
   
   #### Ինչպես է աշխատում
   
   `reduce` մեթոդը անցնում է զանգվածի բոլոր տարրերով և հաշվարկում մեկ արժեք՝ օգտագործելով callback ֆունկցիան։ Այն պահպանում է կուտակված արժեքը (accumulator), որը փոխանցվում է հաջորդ ընթացքին։
   
   ```javascript
   const numbers = [1, 2, 3, 4];
   
   const sum = numbers.reduce((accumulator, currentValue) => accumulator + currentValue, 0);
   console.log(sum); // 10
   ```
   
   #### Սինտաքս
   ```javascript
   array.reduce((accumulator, currentValue, index, array) => {
     // Վերադարձնում է նոր կուտակված արժեք
   }, initialValue);
   ```
   
   - **accumulator**: Կուտակիչը, որը պահպանում է նախորդ վերադարձված արժեքը։
   - **currentValue**: Զանգվածի ընթացիկ տարրը։
   - **index**: Ընթացիկ տարրի ինդեքսը։
   - **array**: Բուն զանգվածը։
   - **initialValue**: Սկզբնական արժեքը (optional)։
   
   #### Օրինակ՝ մաքսիմումի հաշվարկ
   
   ```javascript
   const numbers = [10, 5, 20, 15];
   
   const max = numbers.reduce((acc, num) => (num > acc ? num : acc), numbers[0]);
   console.log(max); // 20
   ```
   
   ---
   
   #### Տարբերությունները
   
   | **Մեթոդ**   | **Վերադարձնում է**                | **Օգտագործման նպատակ**                       |
   |--------------|-----------------------------------|---------------------------------------------|
   | **`map`**    | Նոր զանգված                      | Կիրառել ֆունկցիան յուրաքանչյուր տարրի վրա։  |
   | **`filter`** | Նոր զանգված                      | Ֆիլտրել տարրերը՝ թողնելով միայն համապատասխանները։ |
   | **`reduce`** | Մեկ արժեք                       | Կուտակել տվյալները մեկ արդյունքի։           |
   
   ---
   
   #### Ինչպես են աշխատում ներքին կառուցվածքում
   
   1. **`map`:** Ստեղծում է նոր զանգված՝ անցնելով յուրաքանչյուր տարրի վրա և պահելով վերադարձված արժեքները։
      - Օգտագործում է ներքին `for` ցիկլ։
   
   2. **`filter`:** Ստեղծում է նոր զանգված՝ պահելով միայն այն տարրերը, որոնց համար callback ֆունկցիան վերադարձնում է true։
      - Նույնպես օգտագործում է ներքին `for` ցիկլ։
   
   3. **`reduce`:** Օգտագործում է կուտակիչ՝ առաջընթացաբար հաշվարկելու համար բոլոր տարրերը մեկ արժեքի մեջ։
      - Յուրաքանչյուր քայլում թարմացնում է կուտակիչը։
   
   ---
   
   `map`, `filter` և `reduce` մեթոդները JavaScript-ում հզոր գործիքներ են զանգվածների հետ աշխատելու համար։
   - **`map`:** Օգտագործեք տարրերը փոխակերպելու համար։
   - **`filter`:** Օգտագործեք տարրերը ֆիլտրելու համար։
   - **`reduce`:** Օգտագործեք տվյալները կուտակելու համար մեկ արժեքի մեջ։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

23. ### Ինչ է տարբերությունը Shallow Copy-ի և Deep Copy-ի միջև?
   
   **Shallow Copy**-ն և **Deep Copy**-ն օբյեկտի կամ զանգվածի պատճեններ ստեղծելու երկու մեթոդներ են։ Տարբերությունը կայանում է նրանում, թե ինչպես են նրանք պատճենում տվյալների կառուցվածքը՝ հատկապես բարդ (nested) օբյեկտների դեպքում։
   
   ---
   
   #### Shallow Copy (Մակերեսային պատճեն)
   
   **Shallow Copy**-ն ստեղծում է նոր օբյեկտ կամ զանգված, որը պարունակում է միայն առաջին մակարդակի արժեքների պատճեն։ Եթե օբյեկտը կամ զանգվածը պարունակում են այլ օբյեկտներ կամ զանգվածներ, դրանք պատճենվում են միայն որպես հղում (reference), այլ ոչ թե արժեք։
   
   #### Օրինակ
   
   ```javascript
   const original = { name: "John", address: { city: "New York" } };
   const shallowCopy = { ...original };
   
   shallowCopy.name = "Alice";
   shallowCopy.address.city = "Los Angeles";
   
   console.log(original.name); // "John" (անփոփոխ է)
   console.log(original.address.city); // "Los Angeles" (փոխվել է)
   ```
   
   #### Նկարագրություն
   - **Primitive արժեքները** պատճենվում են որպես արժեք։
   - **Հղումային տիպերը** (օբյեկտներ, զանգվածներ) պատճենվում են որպես հղում։
   
   #### Օգտագործվող մեթոդներ
   - Spread օպերատոր (`...`):
     ```javascript
     const shallowCopy = { ...original };
     const shallowArrayCopy = [...array];
     ```
   - `Object.assign`:
     ```javascript
     const shallowCopy = Object.assign({}, original);
     ```
   
   ---
   
   #### Deep Copy (Խոր պատճեն)
   
   **Deep Copy**-ն ստեղծում է նոր օբյեկտ կամ զանգված՝ ռեկուրսիվ կերպով պատճենելով բոլոր մակարդակները։ Բոլոր հղումային տիպերը պատճենվում են որպես անկախ նոր օբյեկտներ կամ զանգվածներ։
   
   #### Օրինակ
   
   ```javascript
   const original = { name: "John", address: { city: "New York" } };
   
   const deepCopy = JSON.parse(JSON.stringify(original));
   
   deepCopy.name = "Alice";
   deepCopy.address.city = "Los Angeles";
   
   console.log(original.name); // "John" (անփոփոխ է)
   console.log(original.address.city); // "New York" (անփոփոխ է)
   ```
   
   ### Նկարագրություն
   - Բոլոր մակարդակները պատճենվում են որպես անկախ արժեքներ։
   - Հիմնական արժեքները և բարդ կառուցվածքները փոխկապակցված չեն մնում։
   
   #### Օգտագործվող մեթոդներ
   - **`JSON.parse(JSON.stringify())`:** Հեշտ մեթոդ է, բայց չի աջակցում ֆունկցիաներ կամ `undefined` արժեքներ։
     ```javascript
     const deepCopy = JSON.parse(JSON.stringify(original));
     ```
   - **Ռեկուրսիա:** Մանրակրկիտ մոտեցում, որը հարմարեցված է բարդ կառուցվածքների համար։
     ```javascript
     function deepClone(obj) {
       if (obj === null || typeof obj !== "object") {
         return obj;
       }
   
       const copy = Array.isArray(obj) ? [] : {};
       for (let key in obj) {
         if (obj.hasOwnProperty(key)) {
           copy[key] = deepClone(obj[key]);
         }
       }
       return copy;
     }
   
     const deepCopy = deepClone(original);
     ```
   - **Լիբրարիաներ (e.g., Lodash):**
     ```javascript
     const _ = require('lodash');
     const deepCopy = _.cloneDeep(original);
     ```
   
   ---
   
   ## Տարբերությունները
   
   | **Հատկանիշ**           | **Shallow Copy**                             | **Deep Copy**                                |
   |-------------------------|-----------------------------------------------|---------------------------------------------|
   | **Մակարդակ**           | Պատճենում է միայն առաջին մակարդակը          | Պատճենում է բոլոր մակարդակները              |
   | **Հղումներ**           | Խոր կառուցվածքների հղումները պահպանվում են   | Խոր կառուցվածքները լիովին պատճենվում են     |
   | **Արագություն**         | Ավելի արագ                                  | Ավելի դանդաղ (ռեկուրսիվ ընթացքը)            |
   | **Օգտագործման դեպքեր** | Հեշտ և մակերեսային փոփոխությունների համար   | Բարդ և խորը կառուցվածքների պատճենման համար |
   
   ---
   
   ## Եզրակացություն
   
   - **Shallow Copy**-ն հարմար է այն դեպքերի համար, երբ օբյեկտը կամ զանգվածը չունի nested կառուցվածքներ կամ երբ դուք չեք ցանկանում դրանք փոփոխել։
   - **Deep Copy**-ն անհրաժեշտ է, երբ պահանջվում է ամբողջական, անկախ պատճեն՝ ներառյալ խորը կառուցվածքները։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---


24. ### Ինչ է Prototype-ը JavaScript-ում?

   
   **Prototype**-ը JavaScript-ի օբյեկտների հիմքում ընկած մեխանիզմ է, որը թույլ է տալիս օբյեկտներին ժառանգել հատկություններ և մեթոդներ այլ օբյեկտներից։ Prototype-ը հանդիսանում է JavaScript-ի `prototype-based` բնույթի հիմքը և կարևոր դեր է խաղում ծրագրի կառուցվածքում։
   
   JavaScript-ի յուրաքանչյուր օբյեկտ ունի թաքնված հատկություն, որը մատչելի է `[[Prototype]]` անունով։ Այս հատկությունը մատնանշում է մեկ այլ օբյեկտ, որը կոչվում է **Prototype**։
   
   ---
   
   #### Ինչպես է աշխատում Prototype-ը
   
   #### 1. Prototype շղթա
   
   Եթե օբյեկտի վրա կանչվում է հատկություն կամ մեթոդ, և այն բացակայում է այդ օբյեկտում, JavaScript-ը որոնում է այդ հատկությունը օբյեկտի `[[Prototype]]`-ում։ Այս գործընթացը շարունակվում է մինչև հասնի շղթայի վերջ։ Եթե հատկությունը չի գտնվում ոչ մի մակարդակում, վերադարձվում է `undefined`։
   
   ```javascript
   const parent = {
     greet: function() {
       console.log("Hello from parent!");
     }
   };
   
   const child = Object.create(parent);
   
   child.greet(); // "Hello from parent!"
   ```
   
   #### 2. Օբյեկտի ստեղծում և Prototype-ի կապ
   
   Օբյեկտ ստեղծելու ժամանակ նրա `[[Prototype]]`-ը սահմանվում է նրա կոնստրուկտորի `prototype` հատկությանը։
   
   ```javascript
   function Person(name) {
     this.name = name;
   }
   
   Person.prototype.sayHello = function() {
     console.log(`Hello, my name is ${this.name}`);
   };
   
   const john = new Person("John");
   
   john.sayHello(); // "Hello, my name is John"
   console.log(john.__proto__ === Person.prototype); // true
   ```
   
   ---
   
   #### Prototype-ների հիմնական հատկությունները
   
   1. **`prototype` հատկությունը կոնստրուկտոր ֆունկցիաների համար:**
      - Ամեն ֆունկցիա (որը որպես կոնստրուկտոր օգտագործվում է) ունի հատուկ հատկություն՝ `prototype`, որը հանդիսանում է ստեղծված օբյեկտների հիմքը։
   
      ```javascript
      function Animal(type) {
        this.type = type;
      }
   
      console.log(Animal.prototype); // {constructor: ƒ}
      ```
   
   2. **`__proto__` հատկությունը օբյեկտների համար:**
      - Ամեն օբյեկտ ունի թաքնված `__proto__` հատկություն, որը մատնանշում է նրա `[[Prototype]]`։
   
      ```javascript
      const obj = {};
      console.log(obj.__proto__ === Object.prototype); // true
      ```
   
   3. **Prototype շղթայի վերջը:**
      - `Object.prototype` հանդիսանում է Prototype շղթայի վերջնակետը։
      - Եթե հատկությունը հասանելի չէ, JavaScript-ը որոնումը դադարեցնում է այնտեղ։
   
      ```javascript
      console.log(Object.prototype.__proto__); // null
      ```
   
   ---
   
   #### Օգտագործման դեպքեր
   
   #### 1. Հատկություններ և մեթոդներ կիսելու համար
   
   Prototype-ը թույլ է տալիս ընդհանուր հատկություններ և մեթոդներ կիսել օբյեկտների միջև՝ նվազեցնելով հիշողության օգտագործումը։
   
   ```javascript
   function Car(make, model) {
     this.make = make;
     this.model = model;
   }
   
   Car.prototype.getDetails = function() {
     return `${this.make} ${this.model}`;
   };
   
   const car1 = new Car("Toyota", "Corolla");
   const car2 = new Car("Honda", "Civic");
   
   console.log(car1.getDetails()); // "Toyota Corolla"
   console.log(car2.getDetails()); // "Honda Civic"
   ```
   
   #### 2. ժառանգում (Inheritance)
   
   Prototype-ը հիմնական մեթոդ է ժառանգում իրականացնելու համար։
   
   ```javascript
   function Animal(name) {
     this.name = name;
   }
   
   Animal.prototype.speak = function() {
     console.log(`${this.name} makes a noise.`);
   };
   
   function Dog(name, breed) {
     Animal.call(this, name);
     this.breed = breed;
   }
   
   Dog.prototype = Object.create(Animal.prototype);
   Dog.prototype.constructor = Dog;
   
   Dog.prototype.speak = function() {
     console.log(`${this.name} barks.`);
   };
   
   const dog = new Dog("Buddy", "Golden Retriever");
   dog.speak(); // "Buddy barks."
   ```
   
   ---
   
   #### ES6 դասեր և Prototype
   
   ES6 դասերը կառուցված են Prototype-ի վրա։ Դասի մեթոդները ավտոմատ ավելացվում են դրա `prototype`-ում։
   
   ```javascript
   class Person {
     constructor(name) {
       this.name = name;
     }
   
     sayHello() {
       console.log(`Hello, my name is ${this.name}`);
     }
   }
   
   const alice = new Person("Alice");
   alice.sayHello(); // "Hello, my name is Alice"
   console.log(Object.getPrototypeOf(alice) === Person.prototype); // true
   ```
   
   ---
   
   #### Prototype-ի առավելություններ
   
   1. **Հիշողության օպտիմալացում:**
      Հատկությունները և մեթոդները պահպանվում են մեկ անգամ `prototype`-ում, ինչը նվազեցնում է հիշողության օգտագործումը։
   
   2. **Կոդի վերաօգտագործում:**
      Prototype-ը թույլ է տալիս կիսել ընդհանուր մեթոդներ և հատկություններ բազմակի օբյեկտների միջև։
   
   3. **Ժառանգում (Inheritance):**
      Prototype-ը թույլ է տալիս ստեղծել ժառանգական կառուցվածքներ։
   
   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

25. ### Ինչ է JavaScript-ում event bubbling-ը և event capturing-ը 
   
   JavaScript-ում իրադարձությունները (events) տարածվում են փաստաթղթում երկու տարբեր ձևերով՝ **Event Bubbling** (իրադարձության բաբլինգ) և **Event Capturing** (իրադարձության կպչում): Այս մեխանիզմները կառավարում են, թե ինչպես է իրադարձությունը շարժվում DOM ծառով՝ տարրերից դեպի վեր կամ ներքև։

   ---
   
   #### Event Bubbling
   
   **Event Bubbling**-ը այն մեխանիզմն է, որտեղ իրադարձությունը սկսվում է իր նպատակային տարրից (target element) և տարածվում դեպի իր ծնող տարրերը՝ հասնելով մինչև արմատային տարրը (usually `document`)։
   
   #### Ինչպես է աշխատում
   
   Եթե իրադարձությունը կապված է որևէ DOM տարրի հետ, այդ իրադարձությունը կկատարվի ոչ միայն այդ տարրի, այլև նրա բոլոր ծնողների վրա։
   
   ```html
   <div id="parent">
     <button id="child">Click Me</button>
   </div>
   ```
   
   ```javascript
   const parent = document.getElementById("parent");
   const child = document.getElementById("child");
   
   parent.addEventListener("click", () => {
     console.log("Parent clicked");
   });
   
   child.addEventListener("click", () => {
     console.log("Child clicked");
   });
   
   // Երբ սեղմում ենք "Click Me" կոճակը, ելքը կլինի:
   // "Child clicked"
   // "Parent clicked"
   ```

   #### Հատկանիշներ
   - Իրադարձությունը սկսվում է նպատակային տարրից և շարժվում դեպի վեր՝ դեպի նրա ծնողներն ու արմատային տարրը։
   - Բաբլինգը հարմար է իրադարձությունների համապարփակ վերահսկման համար։

   ---

   #### Event Capturing (aka Event Trickling)

   **Event Capturing**-ը այն մեխանիզմն է, որտեղ իրադարձությունը սկսվում է արմատային տարրից (`document`) և շարժվում դեպի իր նպատակային տարրը։
   
   #### Ինչպես է աշխատում
   
   Capturing-ը տեղի է ունենում նախքան բաբլինգը, և դուք կարող եք օգտագործել այն, որպեսզի սկզբում ծածկեք իրադարձությունները։
   
   ```html
   <div id="parent">
     <button id="child">Click Me</button>
   </div>
   ```
   
   ```javascript
   const parent = document.getElementById("parent");
   const child = document.getElementById("child");
   
   parent.addEventListener("click", () => {
     console.log("Parent clicked during capturing phase");
   }, true); 
   
   child.addEventListener("click", () => {
     console.log("Child clicked");
   });
   
   // Երբ սեղմում ենք "Click Me" կոճակը, ելքը կլինի:
   // "Parent clicked during capturing phase"
   // "Child clicked"
   ```
   
   #### Հատկանիշներ
   - Իրադարձությունը սկսվում է արմատային տարրից և շարժվում ներքև՝ նպատակային տարրի ուղղությամբ։
   - Capturing-ը հնարավոր է ակտիվացնել, երբ `addEventListener`-ում փոխանցվում է `true` որպես երրորդ պարամետր։
   
   ---
   
   #### Event Propagation Phases
   
   DOM իրադարձությունների տարածումը բաղկացած է երեք փուլից՝
   
   1. **Capturing Phase:** Իրադարձությունը սկսվում է արմատից և շարժվում ներքև՝ դեպի նպատակային տարր։
   2. **Target Phase:** Իրադարձությունը հասնում է նպատակային տարրին։
   3. **Bubbling Phase:** Իրադարձությունը սկսվում է նպատակային տարրից և շարժվում դեպի վեր՝ դեպի ծնողներ։
   
   ```javascript
   const parent = document.getElementById("parent");
   const child = document.getElementById("child");
   
   parent.addEventListener("click", () => {
     console.log("Parent (Bubbling Phase)");
   });
   
   parent.addEventListener("click", () => {
     console.log("Parent (Capturing Phase)");
   }, true);
   
   child.addEventListener("click", () => {
     console.log("Child (Target Phase)");
   });
   
   // Երբ սեղմում ենք "Click Me" կոճակը, ելքը կլինի:
   // "Parent (Capturing Phase)"
   // "Child (Target Phase)"
   // "Parent (Bubbling Phase)"
   ```

   ---
   
   #### Preventing Event Propagation
   
   Իրադարձությունների տարածումը կարելի է կանգնեցնել՝ օգտագործելով `stopPropagation` մեթոդը։
   
   #### Օրինակ
   
   ```javascript
   child.addEventListener("click", (event) => {
     console.log("Child clicked");
     event.stopPropagation();
   });
   
   parent.addEventListener("click", () => {
     console.log("Parent clicked");
   });
   
   // Երբ սեղմում ենք "Click Me", ելքը կլինի:
   // "Child clicked"
   ```

   ---
   
   #### Event Delegation
   
   **Event Delegation**-ը տեխնիկա է, որտեղ իրադարձությունը կցվում է ծնող տարրին, և այն մշակում է իրադարձությունները նրա զավակների համար՝ օգտագործելով բաբլինգի մեխանիզմը։
   
   #### Օրինակ
   
   ```html
   <ul id="list">
     <li>Item 1</li>
     <li>Item 2</li>
     <li>Item 3</li>
   </ul>
   ```
   
   ```javascript
   const list = document.getElementById("list");
   
   list.addEventListener("click", (event) => {
     if (event.target.tagName === "LI") {
       console.log(`Clicked on ${event.target.textContent}`);
     }
   });
   ```

   ---
   
   #### Եզրակացություն
   
   - **Event Bubbling**: Իրադարձությունը տարածվում է ներքևից վեր։
   - **Event Capturing**: Իրադարձությունը տարածվում է վերևից ներքև։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

26. ### Ինչ է IIFE (Immediately Invoked Function Expression)?
   
   **IIFE (Immediately Invoked Function Expression)**-ը JavaScript-ում հատուկ ֆունկցիոնալ արտահայտություն է, որը ստեղծվում և անմիջապես կանչվում է։ IIFE-ի հիմնական նպատակը տիրույթի (scope) մեկուսացումն է և գլոբալ տիրույթում փոփոխականների հետ հակասություններից խուսափելը։
   
   IIFE-ն սինտաքսորեն կառուցվում է որպես ֆունկցիա, որը շրջապատված է փակագծերով և անմիջապես կանչվում է փակագծերով։
   
   ```javascript
   (function() {
     console.log("This is an IIFE!");
   })();
   // Output: "This is an IIFE!"
   ```

   ---
   
   #### Ինչպես է աշխատում IIFE-ն
   
   #### Սինտաքս
   
   IIFE-ն կառուցվում է երկու հիմնական մասից՝
   
   1. **Ֆունկցիոնալ արտահայտություն (Function Expression):**
      Ֆունկցիան փաթեթավորվում է փակագծերով՝ ստիպելով JavaScript-ին դիտարկել այն որպես արտահայտություն։
   
      ```javascript
      (function() {
        // ֆունկցիայի մարմին
      });
      ```
   
   2. **Կանչման գործողություն (Invocation):**
      Ֆունկցիան անմիջապես կանչվում է փակագծերով՝
   
      ```javascript
      (function() {
        // ֆունկցիայի մարմին
      })();
      ```
   
   #### Օրինակ
   
   ```javascript
   (function(name) {
     console.log(`Hello, ${name}!`);
   })("John");
   // Output: "Hello, John!"
   ```

   ---
   
   #### Օգտագործման դեպքեր
   
   #### 1. Տիրույթի մեկուսացում
   
   IIFE-ն հաճախ օգտագործվում է տիրույթի մեկուսացման համար, որպեսզի կանխվեն փոփոխականների բախումները։
   
   ```javascript
   (function() {
     const privateVariable = "This is private";
     console.log(privateVariable);
   })();
   
   console.log(typeof privateVariable); // "undefined"
   ```
   
   #### 2. Մոդուլային կոդ
   
   IIFE-ն կարող է օգտագործվել մոդուլային կառուցվածք ապահովելու համար։
   
   ```javascript
   const Module = (function() {
     const privateVar = "I am private";
   
     return {
       getPrivateVar: function() {
         return privateVar;
       }
     };
   })();
   
   console.log(Module.getPrivateVar()); // "I am private"
   ```
   
   #### 3. Առանց գլոբալ տիրույթի աղտոտման
   
   IIFE-ն ապահովում է, որ ձեր կոդը չաղտոտի գլոբալ տիրույթը, հատկապես երբ աշխատում եք բրաուզերի միջավայրում։
   
   ```javascript
   (function() {
     const a = 10;
     const b = 20;
     console.log(a + b); // 30
   })();
   
   console.log(typeof a); // "undefined"
   ```

   ---
   
   #### Սինտաքսի տարբերակներ
   
   #### 1. Անվանյալ ֆունկցիա (Named Function)
   
   ```javascript
   (function namedIIFE() {
     console.log("IIFE with a name");
   })();
   ```
   
   #### 2. Arrow Function սինտաքս (Arrow Function IIFE)
   
   ```javascript
   (() => {
     console.log("Arrow Function IIFE");
   })();
   ```

   ---
   
   #### Առավելություններ
   
   1. **Տիրույթի մեկուսացում:**
      IIFE-ն թույլ է տալիս սահմանել լոկալ փոփոխականներ առանց գլոբալ տիրույթում խառնաշփոթ առաջացնելու։
   
   2. **Կոդի պարզություն և անվտանգություն:**
      Բարդ ծրագրերում IIFE-ն թույլ է տալիս վերահսկել փոփոխականների հասանելիությունը։
   
   3. **Անմիջական կատարում:**
      IIFE-ն ապահովում է ֆունկցիայի անմիջապես կատարումը՝ չսպասելով հետագա կանչերին։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

27. ### Ինչ է JavaScript-ում WeakMap-ը և WeakSet-ը?

   **WeakMap**-ը և **WeakSet**-ը JavaScript-ում հատուկ տեսակների տվյալների կառուցվածքներ են, որոնք թույլ են տալիս պահել օբյեկտների հղումներ, առանց դրանց վրա պահել հիշողության կառավարման պատասխանատվությունը։ Դրանք նախագծված են այնպես, որ **garbage collection**-ը (հիշողության ավտոմատ մաքրում) կարողանա ճիշտ աշխատել՝ հանելով այն օբյեկտները, որոնք այլևս օգտագործման մեջ չեն։

   ---
   
   #### WeakMap
   
   #### Ինչ է WeakMap-ը?
   
   **WeakMap**-ը հանդիսանում է տվյալների կառուցվածք, որը թույլ է տալիս պահել "key-value" զույգեր, որտեղ **key**-երը պարտադիր պետք է լինեն օբյեկտներ։
   
   #### Հիմնական հատկանիշներ
   
   1. **Անվտանգ հղումներ (Weak References):**
      - `WeakMap`-ի մեջ պահվող օբյեկտները թույլ են կապվում։ Եթե ոչ մի այլ հղում չկա այդ օբյեկտի վրա, ապա այն կհեռացվի **garbage collector**-ի կողմից։
   
   2. **Անհասանելի հատկանիշներ:**
      - `WeakMap`-ի բովանդակությունը անհասանելի է և չի կարող իտերացիայի ենթարկվել։
   
   3. **Հասանելիություն միայն մեթոդներով:**
      - `WeakMap`-ում կարող եք մուտք գործել միայն նրա առաջարկվող մեթոդներով։
   
   #### Օգտագործվող մեթոդներ
   
   - **`set(key, value)`**: Ավելացնում է "key-value" զույգ։
   - **`get(key)`**: Վերադարձնում է `key`-ին համապատասխան արժեքը։
   - **`delete(key)`**: Հեռացնում է "key-value" զույգը։
   - **`has(key)`**: Վերադարձնում է `true`, եթե `key`-ը առկա է։
   
   #### Օրինակ
   
   ```javascript
   let weakMap = new WeakMap();
   let obj = { name: "John" };
   
   weakMap.set(obj, "Developer");
   
   console.log(weakMap.get(obj)); // "Developer"
   console.log(weakMap.has(obj)); // true
   
   obj = null; // Հղումը հանվեց
   
   // Garbage collector-ը կհեռացնի obj-ը WeakMap-ից։
   console.log(weakMap.has(obj)); // false
   ```

   ---
   
   #### WeakSet
   
   #### Ինչ է WeakSet-ը?
   
   **WeakSet**-ը տվյալների կառուցվածք է, որը թույլ է տալիս պահել միայն օբյեկտների հղումներ։
   
   #### Հիմնական հատկանիշներ
   
   1. **Անվտանգ հղումներ (Weak References):**
      - WeakSet-ի մեջ պահվող օբյեկտները թույլ են կապվում։ Եթե ոչ մի այլ հղում չկա այդ օբյեկտի վրա, ապա այն կհեռացվի **garbage collector**-ի կողմից։
   
   2. **Անհասանելի բովանդակություն:**
      - WeakSet-ի բովանդակությունը անհասանելի է և չի կարող իտերացիայի ենթարկվել։
   
   3. **Կրկնվող արժեքներ:**
      - WeakSet-ը չի թույլատրում կրկնվող օբյեկտներ։
   
   #### Օգտագործվող մեթոդներ
   
   - **`add(value)`**: Ավելացնում է նոր արժեք։
   - **`delete(value)`**: Հեռացնում է արժեքը։
   - **`has(value)`**: Վերադարձնում է `true`, եթե արժեքը առկա է։
   
   #### Օրինակ
   
   ```javascript
   let weakSet = new WeakSet();
   let obj1 = { id: 1 };
   let obj2 = { id: 2 };
   
   weakSet.add(obj1);
   weakSet.add(obj2);
   
   console.log(weakSet.has(obj1)); // true
   
   obj1 = null; // Հղումը հանվեց
   
   // Garbage collector-ը կհեռացնի obj1-ը WeakSet-ից։
   console.log(weakSet.has(obj1)); // false
   ```

   ---
   
   #### WeakMap և WeakSet-ի տարբերությունները Map-ի և Set-ի հետ
   
   | **Հատկանիշ**            | **Map**                          | **WeakMap**                      | **Set**                          | **WeakSet**                      |
   |--------------------------|-----------------------------------|-----------------------------------|-----------------------------------|-----------------------------------|
   | **Կանոն key-երի համար** | Կարող է լինել ցանկացած արժեք      | Միայն օբյեկտ                    | Կարող է լինել ցանկացած արժեք      | Միայն օբյեկտ                    |
   | **Garbage Collection**   | Չի աջակցում                      | Աջակցում է                      | Չի աջակցում                      | Աջակցում է                      |
   | **Իտերացիա**            | Այո                              | Ոչ                               | Այո                              | Ոչ                               |
   | **Հատկանիշների հասանելիություն** | Բաց (Iterable)                  | Փակ (Non-Iterable)               | Բաց (Iterable)                  | Փակ (Non-Iterable)               |

   ---
   
   #### Օգտագործման դեպքեր
   
   #### WeakMap-ի Օգտագործում
   
   1. **Օբյեկտների Մասնավոր Տվյալների Կառավարում:**
      WeakMap-ը հաճախ օգտագործվում է օբյեկտների մասնավոր տվյալների պահպանման համար։
   
   ```javascript
   const privateData = new WeakMap();
   
   class User {
     constructor(name) {
       privateData.set(this, { name });
     }
   
     getName() {
       return privateData.get(this).name;
     }
   }
   
   const user = new User("Alice");
   console.log(user.getName()); // "Alice"
   ```
   
   #### WeakSet-ի Օգտագործում
   
   1. **Օբյեկտների Թույլ Հղումների Կառավարում:**
      WeakSet-ը կարող է օգտագործվել օբյեկտների եզակի հավաքածուներ պահպանելու համար։
   
   ```javascript
   let activeUsers = new WeakSet();
   
   let user1 = { id: 1 };
   let user2 = { id: 2 };
   
   activeUsers.add(user1);
   activeUsers.add(user2);
   
   console.log(activeUsers.has(user1)); // true
   
   user1 = null;
   // Garbage collector-ը կհեռացնի user1-ը WeakSet-ից։
   ```

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

28. ### Ինչ է Execution Context-ը JavaScript-ում?
   
   **Execution Context**-ը (Կատարման Կոնտեքստ) JavaScript-ի մեխանիզմ է, որը սահմանում է այն միջավայրը, որտեղ կոդը կատարվում է։ Այն ներառում է բոլոր անհրաժեշտ տվյալները, որոնք անհրաժեշտ են կոդի ճիշտ կատարման համար։
   
   JavaScript-ում Execution Context-ը հանդիսանում է մի քանի մակարդակով կառավարվող գործընթաց, որը ներառում է փոփոխականների, ֆունկցիաների, և օբյեկտների տիրույթի սահմանումը։

   ---
   
   #### Execution Context-ի տեսակները
   
   #### 1. Գլոբալ Execution Context (Գլոբալ Կատարման Կոնտեքստ)
   
   Սա այն միջավայրն է, որտեղ JavaScript-ի կոդը սկսում է իր կատարման գործընթացը։
   
   - Գլոբալ Execution Context-ը ստեղծվում է ծրագրի սկիզբում։
   - Այն ներառում է գլոբալ տիրույթում հայտարարված փոփոխականները, ֆունկցիաները և `this`-ը։
   
   ```javascript
   var globalVar = "I am global";
   
   function globalFunction() {
     console.log(globalVar);
   }
   
   globalFunction();
   ```
   
   **Նկարագրություն:**
   - Գլոբալ տիրույթում `this`-ը մատնանշում է `window` օբյեկտը (բրաուզերային միջավայրում) կամ `global` օբյեկտը (Node.js-ում)։
   
   #### 2. Ֆունկցիայի Execution Context
   
   Ամեն անգամ, երբ կանչվում է ֆունկցիա, ստեղծվում է նոր Execution Context։
   
   - Ֆունկցիայի Execution Context-ը ներառում է բոլոր ֆունկցիոնալ փոփոխականները և դրանց արժեքները։
   - Այն սահմանում է `this`-ը, որը կախված է կանչի վայրից։
   
   ```javascript
   function testFunction() {
     var localVar = "I am local";
     console.log(localVar);
   }
   
   testFunction();
   ```
   
   **Նկարագրություն:**
   - Execution Context-ը ժամանակավոր միջավայր է, որը կոդի կատարման ավարտից հետո ջնջվում է։
   
   #### 3. ԵՎԵՍԻԿ Execution Context (Eval Execution Context)
   
   Երբ օգտագործվում է `eval()` ֆունկցիան, այն ստեղծում է իր սեփական Execution Context-ը։
   
   ```javascript
   eval("var evalVar = 'I am eval';");
   console.log(evalVar); // "I am eval"
   ```

   ---
   
   #### Execution Context-ի Կառուցվածքը
   
   Execution Context-ը բաղկացած է հետևյալ երեք հիմնական մասերից՝
   
   #### 1. Variable Environment (Փոփոխականների Միջավայր)
   
   Սա այն տարածքն է, որտեղ պահվում են փոփոխականները և ֆունկցիաները։
   
   - Գլոբալ փոփոխականները պահվում են գլոբալ տիրույթում։
   - Լոկալ փոփոխականները պահվում են ֆունկցիայի տիրույթում։
   
   ```javascript
   function demo() {
     var x = 10;
     let y = 20;
     const z = 30;
   }
   ```
   
   #### 2. Lexical Environment (Լեքսիկական Միջավայր)
   
   Սա ներառում է բոլոր լեքսիկական տիրույթները, որտեղ հայտարարվել են փոփոխականները։
   
   ```javascript
   function outer() {
     var outerVar = "I am outer";
   
     function inner() {
       console.log(outerVar); // "I am outer"
     }
   
     inner();
   }
   
   outer();
   ```
   
   #### 3. `this` Binding
   
   `this`-ի արժեքը սահմանվում է կախված Execution Context-ի տեսակից։
   
   - Գլոբալ Execution Context-ում `this`-ը մատնանշում է գլոբալ օբյեկտը։
     - Ֆունկցիայի Execution Context-ում `this`-ը կախված է կանչի վայրից։
   
   ```javascript
   function showThis() {
     console.log(this);
   }
   
   showThis(); // Window (բրաուզերում)
   ```

   ---
   
   #### Execution Stack (Կատարման Ստեկ)
   
   Execution Context-ները կառավարվում են Execution Stack-ով (կատարման ստեկով):
   
   - Ամեն անգամ, երբ կանչվում է նոր ֆունկցիա, նրա Execution Context-ը ավելացվում է ստեկի գագաթին։
     - Կատարման ավարտից հետո այն հեռացվում է ստեկից։
   
   ```javascript
   function first() {
     console.log("First function");
     second();
   }
   
   function second() {
     console.log("Second function");
   }
   
   first();
   
   // Execution Stack:
   // 1. Գլոբալ Execution Context
   // 2. first Execution Context
   // 3. second Execution Context
   ```

   ---
   
   #### Hoisting-ը Execution Context-ում
   
   **Hoisting**-ը JavaScript-ի մեխանիզմ է, որտեղ փոփոխականներն ու ֆունկցիաները "տեղափոխվում" են իրենց տիրույթի վերև։
   
   ```javascript
   console.log(a); // undefined
   var a = 10;
   
   hoistedFunction(); // "I am hoisted"
   
   function hoistedFunction() {
     console.log("I am hoisted");
   }
   ```
   
   ---
   
   #### Եզրակացություն
   
   Execution Context-ը JavaScript-ի հիմնարար մեխանիզմ է, որը պատասխանատու է կոդի կատարման միջավայրի սահմանման համար։
   
   - **Գլոբալ Execution Context:** Ստեղծվում է ծրագրի մեկնարկին և պարունակում է գլոբալ տիրույթը։
   - **Ֆունկցիայի Execution Context:** Ստեղծվում է ամեն ֆունկցիայի կանչի ժամանակ։
   - Execution Context-ները կառավարվում են Execution Stack-ի միջոցով։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

29. ### Ինչ է Scope-ը և Scope Chain-ը JavaScript-ում?
   
   **Scope**-ը JavaScript-ում սահմանում է, թե որտեղից կարող են փոփոխականները, ֆունկցիաները և օբյեկտները հասանելի լինել ծրագրում։ Scope-ը կառավարվում է JavaScript-ի իրականացրած **lexical scoping**-ի միջոցով, որը նշանակում է, որ փոփոխականների հասանելիությունը որոշվում է կոդի կառուցվածքով։
   
   Scope-ը ապահովում է կոդի մաքրություն, սահմանափակում է փոփոխականների հասանելիությունը և կանխում է գլոբալ տիրույթի աղտոտումը։
   
   ---
   
   #### Scope-ի տեսակները JavaScript-ում
   
   #### 1. Գլոբալ Scope (Global Scope)
   
   Գլոբալ Scope-ում հայտարարված փոփոխականները հասանելի են ծրագրի ցանկացած կետից։
   
   - Եթե փոփոխականը հայտարարվում է տիրույթի սահմաններից դուրս, այն դառնում է գլոբալ։
   - Գլոբալ փոփոխականները JavaScript-ում դառնում են `window` օբյեկտի հատկություն (բրաուզերային միջավայրում)։
   
   ```javascript
   var globalVar = "I am global";
   
   function test() {
     console.log(globalVar); // "I am global"
   }
   
   test();
   console.log(window.globalVar); // "I am global" (բրաուզերում)
   ```
   
   **Նշում:** Խուսափեք շատ գլոբալ փոփոխականների օգտագործումից, քանի որ դրանք կարող են առաջացնել բախումներ։
   
   #### 2. Ֆունկցիայի Scope (Function Scope)
   
   Ֆունկցիայի Scope-ում հայտարարված փոփոխականները հասանելի են միայն տվյալ ֆունկցիայի ներսում։
   
   - `var`, `let`, և `const`-ով հայտարարված փոփոխականները, եթե գտնվում են ֆունկցիայի ներսում, ունեն լոկալ տիրույթ։
   
   ```javascript
   function localScope() {
     var localVar = "I am local";
     console.log(localVar); // "I am local"
   }
   
   localScope();
   console.log(localVar); // ReferenceError: localVar is not defined
   ```
   
   #### 3. Բլոկի Scope (Block Scope)
   
   Բլոկի տիրույթը վերաբերում է `{}` փակագծերով սահմանված ցանկացած բլոկի։
   
   - `let` և `const`-ով հայտարարված փոփոխականները ունեն բլոկային տիրույթ։
   - `var`-ը չի ապահովում բլոկային տիրույթ։
   
   ```javascript
   {
     let blockScoped = "I am block scoped";
     const anotherBlockScoped = "Me too";
     console.log(blockScoped); // "I am block scoped"
   }
   
   console.log(blockScoped); // ReferenceError: blockScoped is not defined
   ```
   
   #### 4. Մոդուլի Scope (Module Scope)
   
   ES6 մոդուլներում փոփոխականները ունեն իրենց սեփական տիրույթը, և դրանք հասանելի չեն գլոբալ տիրույթում։
   
   ```javascript
   // module.js
   export const moduleScoped = "I am module scoped";
   
   // main.js
   import { moduleScoped } from "./module.js";
   console.log(moduleScoped); // "I am module scoped"
   ```
   
   ---
   
   #### Scope Chain-ի նկարագրություն
   
   **Scope Chain**-ը սահմանում է, թե ինչպես է JavaScript-ը որոնում փոփոխականները։ Երբ ֆունկցիան կամ բլոկը փորձում է օգտագործել փոփոխական, JavaScript-ը ստուգում է հետևյալ հերթականությամբ՝
   
   1. Լոկալ (local) տիրույթում՝ ֆունկցիայի կամ բլոկի ներսում։
   2. Ծնող ֆունկցիայի կամ բլոկի տիրույթում։
   3. Գլոբալ տիրույթում։
   
   Եթե փոփոխականը չի գտնվում ոչ մի տիրույթում, ստացվում է ReferenceError։
   
   #### Օրինակ՝ Scope Chain-ի աշխատանք
   
   ```javascript
   const globalVar = "I am global";
   
   function outerFunction() {
     const outerVar = "I am outer";
   
     function innerFunction() {
       const innerVar = "I am inner";
       console.log(innerVar); // "I am inner"
       console.log(outerVar); // "I am outer"
       console.log(globalVar); // "I am global"
     }
   
     innerFunction();
   }
   
   outerFunction();
   ```
   
   **Նկարագրություն:**
   - `innerFunction`-ը որոնում է `innerVar` իր սեփական տիրույթում։
   - Այնուհետև այն որոնում է `outerVar` ծնող ֆունկցիայի տիրույթում։
   - Վերջում որոնվում է `globalVar` գլոբալ տիրույթում։
   
   ---
   
   #### Lexical Scope
   
   JavaScript-ը օգտագործում է **lexical scoping**, ինչը նշանակում է, որ ֆունկցիայի տիրույթը որոշվում է նրա հայտարարության վայրում, այլ ոչ թե կանչի վայրում։
   
   ```javascript
   function outerFunction() {
     const outerVar = "I am outer";
   
     function innerFunction() {
       console.log(outerVar); // "I am outer"
     }
   
     return innerFunction;
   }
   
   const myFunction = outerFunction();
   myFunction();
   ```
   
   Lexical scoping-ի շնորհիվ `innerFunction`-ը միշտ կարող է հասանելի լինել `outerVar`-ին, անկախ նրանից, թե որտեղից է կանչվում։
   
   ---
   
   #### JavaScript-ի Scope-ի խնդիրները և լուծումները
   
   #### 1. Գլոբալ փոփոխականների բախում
   
   Գլոբալ փոփոխականները կարող են առաջացնել բախումներ, երբ տարբեր ծրագրավորողներ օգտագործում են նույն փոփոխական անունը։
   
   **Լուծում:**
   - Օգտագործեք IIFE (Immediately Invoked Function Expression):
   
   ```javascript
   (function() {
     const localVar = "I am local";
     console.log(localVar); // "I am local"
   })();
   
   console.log(localVar); // ReferenceError: localVar is not defined
   ```
   
   #### 2. `var`-ի խնդիրները բլոկային տիրույթում
   
   `var`-ը չունի բլոկային տիրույթ, ինչը կարող է առաջացնել անսպասելի վարքագիծ։
   
   **Լուծում:**
   - Օգտագործեք `let` կամ `const`:
   
   ```javascript
   for (let i = 0; i < 5; i++) {
     setTimeout(() => console.log(i), 1000); // 0, 1, 2, 3, 4
   }
   ```
   
   ---
   
   #### Scope Chain-ի օպտիմալացում
   
  **Փոփոխականները սահմանեք այն տիրույթում, որտեղից դրանք օգտագործվում են ամենաշատը։**
   
      ```javascript
      function optimizedFunction() {
        const frequentlyUsed = 42;
   
        function inner() {
          console.log(frequentlyUsed);
        }
   
        inner();
      }
      ```

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---


30. ### Ինչ է JavaScript-ի strict mode-ը?

   **Strict Mode**-ը (Խիստ ռեժիմ) JavaScript-ում հատուկ գործող ռեժիմ է, որը ներկայացվեց ECMAScript 5-ում։ Այն նախատեսված է կոդի սխալների կանխարգելման և JavaScript-ի ավելի անվտանգ վարք ապահովելու համար։
   
   Strict Mode-ը սահմանում է խիստ կանոններ՝ արգելելով որոշ գործողություններ և ներկայացնելով լրացուցիչ ստուգումներ։
   
   ---
   
   #### Ինչպես ակտիվացնել Strict Mode-ը
   
   #### Գլոբալ մակարդակում
   
   Strict Mode-ը կարելի է ակտիվացնել ամբողջ սկրիպտի համար՝ հայտարարելով `'use strict';` անմիջապես սկրիպտի սկզբում։
   
   ```javascript
   'use strict';
   
   x = 10; // ReferenceError: x is not defined
   ```
   
   #### Ֆունկցիայի մակարդակում
   
   Strict Mode-ը կարող է կիրառվել միայն ֆունկցիայի ներսում՝ հայտարարելով `'use strict';` ֆունկցիայի մարմնի սկզբում։
   
   ```javascript
   function myFunction() {
     'use strict';
     y = 20; // ReferenceError: y is not defined
   }
   
   myFunction();
   ```
   
   #### Մոդուլների մեջ
   
   ECMAScript 6 մոդուլները ավտոմատ աշխատում են Strict Mode-ով, այնպես որ անհրաժեշտ չէ այն հայտարել։
   
   ---
   
   #### Strict Mode-ի առանձնահատկությունները
   
   1. **Փոփոխականների հայտարումը պարտադիր է:**
      Անհայտարարված փոփոխականներ օգտագործելու փորձը առաջացնում է ReferenceError։
   
      ```javascript
      'use strict';
   
      myVar = 100; // ReferenceError: myVar is not defined
      ```
   
   2. **Սխալ գրությունների կանխում:**
      Strict Mode-ը օգնում է կանխել փոփոխականների անվանական սխալները։
   
      ```javascript
      'use strict';
   
      const obj = { name: "John" };
      Object.defineProperty(obj, "age", { writable: false, value: 30 });
   
      obj.age = 25; // TypeError: Cannot assign to read-only property 'age'
      ```
   
   3. **Արգելված կրկնակի սեփական անուններ:**
      Strict Mode-ը չի թույլատրում ֆունկցիաների պարամետրերի կամ օբյեկտների կրկնվող անուններ։
   
      ```javascript
      'use strict';
   
      function myFunc(a, a) {
        // SyntaxError: Duplicate parameter name not allowed in this context
      }
      ```
   
   4. **`this` արժեքի սահմանափակում:**
      Strict Mode-ում `this`-ը անորոշ համատեքստերում (undefined) սահմանվում է որպես `undefined` և ոչ թե գլոբալ օբյեկտ։
   
      ```javascript
      'use strict';
   
      function myFunc() {
        console.log(this);
      }
   
      myFunc(); // undefined
      ```
   
   5. **Արգելում է `with` հայտարարությունը:**
      `with` հայտարարությունը արգելված է, քանի որ այն բարդացնում է փոփոխականների որոնումը։
   
      ```javascript
      'use strict';
   
      with (Math) {
        // SyntaxError: Strict mode code may not include a with statement
        x = cos(2);
      }
      ```
   
   6. **Արգելված է ֆունկցիաների հռչակումը բլոկի ներսում:**
      Բլոկի ներսում ֆունկցիա հռչակելը strict mode-ում առաջացնում է սխալ։
   
      ```javascript
      'use strict';
   
      if (true) {
        function test() {} // SyntaxError
      }
      ```
   
   ---
   
   #### Strict Mode-ը նորագույն JavaScript տարբերակներում
   
   1. **ECMAScript 6 (ES6) և մոդուլներ:**
      ES6-ից սկսած, բոլոր մոդուլները ավտոմատ աշխատում են Strict Mode-ով։ Այսինքն՝ դուք կարիք չունեք հայտարել `'use strict';` մոդուլի սկիզբում։
   
      ```javascript
      // module.js (ES6 Module)
      export function test() {
        console.log(this); // undefined, because of strict mode
      }
      ```
   
   2. **Class-եր:**
      ES6-ից սկսած բոլոր դասերը (classes) նույնպես աշխատում են Strict Mode-ով՝ անկախ նրանից, արդյոք դուք օգտագործում եք `'use strict';`։
   
      ```javascript
      class Person {
        constructor(name) {
          this.name = name;
        }
      }
   
      const person = new Person("John");
      console.log(person.name); // "John"
      ```
   
   ---
   
   #### Strict Mode-ը Framework-ներում
   
   1. **React:**
      React-ում Strict Mode-ը օգտագործվում է `React.StrictMode` կոմպոնենտի միջոցով՝ ծրագրային սխալները հայտնաբերելու և դեպրեկացված մեթոդները կանխելու համար։
   
      ```javascript
      import React from 'react';
      import ReactDOM from 'react-dom';
   
      ReactDOM.render(
        <React.StrictMode>
          <App />
        </React.StrictMode>,
        document.getElementById('root')
      );
      ```
   
      React.StrictMode-ը չի ազդեցում արտադրական կոդի վրա։
   
   2. **Angular:**
      Angular-ում strict mode-ը կարող է միացվել `ng new` հրամանի ժամանակ՝ ավելացնելով `--strict` դրոշակը։
   
      ```bash
      ng new my-app --strict
      ```
   
      Strict Mode-ը Angular-ում ավելացնում է լրացուցիչ ստուգումներ `TypeScript`-ի և Angular-ի կոնֆիգուրացիաներում։
   
   3. **Vue.js:**
      Vue 3-ը աջակցում է ES6 մոդուլներին և ավտոմատ աշխատում է Strict Mode-ով, քանի որ այն կառուցված է մոդուլային կառուցվածքի վրա։
   
   ---
   
   #### Strict Mode-ի առավելություններ
   
   1. **Կոդի ընթեռնելիություն և կանխատեսելիություն:**
      Strict Mode-ը օգնում է խուսափել չնախատեսված վարքագծից։
   
   2. **Կատարողականության բարելավում:**
      Շատ բրաուզերներ օպտիմալացնում են Strict Mode-ի կոդը, քանի որ այն ապահովում է կանխատեսելի վարքագիծ։
   
   3. **Սխալների հայտնաբերում վաղ փուլում:**
      Strict Mode-ը ներկայացնում է սինտաքսային և կատարման ստուգումներ, որոնք կանխում են սխալները։
   
   4. **Ավելի անվտանգ կոդ:**
      Strict Mode-ը արգելում է վտանգավոր գործողությունները, ինչպիսիք են՝ անտեսանելի գլոբալ փոփոխականների ստեղծումը։
   
   ---
   
   #### Եզրակացություն
   
   Strict Mode-ը հզոր գործիք է, որը թույլ է տալիս JavaScript-ում գրել ավելի անվտանգ, ընթեռնելի և կանխատեսելի կոդ։ Այն հատկապես օգտակար է խոշոր նախագծերում, որտեղ սխալների հայտնաբերումն ու կառավարմանը մեծ դեր ունեն։ Ժամանակակից ֆրեյմվորքները և ES6+ մոդուլները ավտոմատ աշխատում են Strict Mode-ով՝ դարձնելով այն անբաժան JavaScript ծրագրավորման գործընթացից։

   ---


**[⬆ Back to Top](#բովանդակություն)**

   ---

31. ### Ինչ է CORS-ը և ինչու է այն կարևոր?

   **CORS** (Cross-Origin Resource Sharing)-ը մեխանիզմ է, որը թույլ է տալիս բրաուզերին ապահով կերպով օգտագործել ռեսուրսներ (օրինակ՝ տվյալներ, նկարներ, API) մի ծագման (origin) սերվերից, որը տարբերվում է այն սերվերից, որտեղից բեռնվել է կայքը։
   
   CORS-ը հիմնված է HTTP վերնագրերի վրա, որոնք սահմանում են, թե որ ծագումներն են թույլատրվում մուտք գործել սերվերի ռեսուրսներին և ինչպես։

   ---
   
   #### Ինչու է CORS-ը կարևոր?
   
   CORS-ը շատ կարևոր է վեբ անվտանգության համար, քանի որ այն պաշտպանում է վեբ ծրագրերը չարտոնված մուտքերից։
   
   #### Առանց CORS-ի
   Առանց CORS-ի, JavaScript-ը բրաուզերում չէր կարող օգտագործել այլ ծագման API-ներ։
   
   #### Օրինակ՝ խնդրի առաջացում
   
   Եթե ձեր կայքը բեռնվել է `https://example.com`-ից և փորձում է մուտք գործել API, որը գտնվում է `https://api.anotherdomain.com`-ում, բրաուզերը ավտոմատ կերպով արգելափակում է այդ հարցումը, եթե CORS կարգավորումները թույլ չեն տալիս։
   
   ```javascript
   fetch('https://api.anotherdomain.com/data')
     .then(response => response.json())
     .then(data => console.log(data))
     .catch(error => console.error('Error:', error));
   ```
   
   #### Արդյունք՝ առանց CORS-ի
   
   ```plaintext
   Access to fetch at 'https://api.anotherdomain.com/data' from origin 'https://example.com' has been blocked by CORS policy.
   ```
   
   ---
   
   #### Ինչպես է աշխատում CORS-ը
   
   CORS-ը սահմանվում է սերվերի կողմից։ Երբ բրաուզերը ուղարկում է հարցում այլ ծագման, սերվերը պատասխանում է համապատասխան HTTP վերնագրերով, որոնք բրաուզերին ասում են՝ արդյոք թույլատրվում է մուտքը։
   
   #### HTTP վերնագրեր
   
   1. **`Access-Control-Allow-Origin`:**
      Սահմանում է, թե որ ծագումները կարող են մուտք գործել ռեսուրսին։
   
      ```http
      Access-Control-Allow-Origin: https://example.com
      ```
   
   2. **`Access-Control-Allow-Methods`:**
      Սահմանում է թույլատրելի HTTP մեթոդները՝ օրինակ `GET`, `POST`, `PUT`, և այլն։
   
      ```http
      Access-Control-Allow-Methods: GET, POST
      ```
   
   3. **`Access-Control-Allow-Headers`:**
      Սահմանում է թույլատրելի մաքսային վերնագրերը։
   
      ```http
      Access-Control-Allow-Headers: Content-Type, Authorization
      ```
   
   4. **`Access-Control-Allow-Credentials`:**
      Թույլ է տալիս ուղարկել հավաստագրեր (credentials), ինչպիսիք են `cookies`-երը։
   
      ```http
      Access-Control-Allow-Credentials: true
      ```
   
   ---
   
   #### Հիմնական գործընթաց
   
   #### 1. **Simple Requests (Պարզ հարցումներ)**
   
   Եթե հարցումը բրաուզերի կողմից համարվում է "պարզ", այն անմիջապես ուղարկվում է սերվերին։
   
   **Պարզ հարցումների պայմաններ:**
   - HTTP մեթոդը `GET`, `POST`, կամ `HEAD` է։
   - Բովանդակության տեսակը `text/plain`, `application/x-www-form-urlencoded`, կամ `multipart/form-data` է։
   
   #### 2. **Preflight Requests (Նախնական հարցումներ)**
   
   Եթե հարցումը պարունակում է մաքսային վերնագրեր կամ օգտագործում է ոչ "պարզ" մեթոդներ (օրինակ՝ `PUT`, `DELETE`), բրաուզերը նախ ուղարկում է "Preflight" հարցում։
   
   ```http
   OPTIONS /data HTTP/1.1
   Host: api.anotherdomain.com
   Origin: https://example.com
   Access-Control-Request-Method: POST
   Access-Control-Request-Headers: Content-Type
   ```
   
   Սերվերի պատասխան՝
   
   ```http
   HTTP/1.1 200 OK
   Access-Control-Allow-Origin: https://example.com
   Access-Control-Allow-Methods: GET, POST
   Access-Control-Allow-Headers: Content-Type
   ```

   ---
   
   #### Ինչպես կարգավորել CORS-ը
   
   CORS-ը սահմանվում է սերվերի կողմում։
   
   #### Օրինակ՝ Node.js + Express
   
   ```javascript
   const express = require('express');
   const cors = require('cors');
   const app = express();
   
   // Թույլատրել բոլոր ծագումները
   app.use(cors());
   
   // Կամ՝ սահմանափակել կոնկրետ ծագումներ
   app.use(cors({ origin: 'https://example.com' }));
   
   app.get('/data', (req, res) => {
     res.json({ message: 'This is CORS-enabled!' });
   });
   
   app.listen(3000, () => console.log('Server running on port 3000'));
   ```

   ---
   
   #### CORS-ի առավելություններ
   
   1. **Անվտանգություն:**
      - CORS-ը պաշտպանում է սերվերը չարտոնված ծագումներից։
   
   2. **Կառավարում:**
      - Սերվերը կարող է վերահսկել, թե որ ծագումները կամ մեթոդները կարող են մուտք գործել ռեսուրսին։
   
   3. **Ճկունություն:**
      - Թույլ է տալիս սահմանափակել կամ ընդլայնել մուտք գործելու հնարավորությունները՝ կախված ծրագրի կարիքներից։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

32. ### Ինչ է Module Pattern-ը JavaScript-ում?

   
   **Module Pattern**-ը JavaScript-ում կիրառվում է կոդի կազմակերպման և տվյալների մեկուսացման համար։ Այն թույլ է տալիս ստեղծել մասնավոր (private) փոփոխականներ և մեթոդներ՝ միաժամանակ տրամադրելով հրապարակային (public) ինտերֆեյս։
   
   Module Pattern-ը հաճախ օգտագործվում է այնպիսի ծրագրերում, որտեղ անհրաժեշտ է պահպանել տվյալների գաղտնիությունը և կանխել գլոբալ տիրույթի աղտոտումը։

   ---
   
   #### Ինչու է Module Pattern-ը կարևոր?
   
   1. **Գլոբալ տիրույթի աղտոտման կանխում:**
      - Module Pattern-ը օգնում է պահպանել փոփոխականները լոկալ տիրույթում՝ կանխելով բախումները։
   
   2. **Տվյալների գաղտնիություն (Encapsulation):**
      - Փոփոխականներն ու ֆունկցիաները, որոնք չպետք է հասանելի լինեն դրսից, կարող են մնալ մասնավոր։
   
   3. **Կոդի կազմակերպում:**
      - Ապահովում է կոդի բաժանումը տրամաբանական միավորների, ինչը դարձնում է ծրագիրը ավելի ընթեռնելի և կառավարելի։
   
   ---
   
   #### Ինչպես է աշխատում Module Pattern-ը?
   
   Module Pattern-ը օգտագործում է **Immediately Invoked Function Expression (IIFE)** մեխանիզմը՝ մեկուսացված տիրույթ ստեղծելու համար։
   
   #### Կառուցվածք
   
   ```javascript
   const Module = (function() {
     // Մասնավոր փոփոխականներ և մեթոդներ
     let privateVar = "This is private";
   
     function privateMethod() {
       console.log(privateVar);
     }
   
     // Հանրային ինտերֆեյս
     return {
       publicMethod: function() {
         console.log("Accessing private method:");
         privateMethod();
       },
   
       setPrivateVar: function(value) {
         privateVar = value;
       },
   
       getPrivateVar: function() {
         return privateVar;
       }
     };
   })();
   
   // Օգտագործում
   Module.publicMethod(); // "Accessing private method:" "This is private"
   Module.setPrivateVar("New private value");
   console.log(Module.getPrivateVar()); // "New private value"
   ```

   ---
   
   #### Module Pattern-ի առավելություններ
   
   1. **Գաղտնիություն:**
      - Մասնավոր փոփոխականները և մեթոդները հասանելի չեն լինում դրսից։
   
   2. **Կոդի մաքրություն:**
      - Կոդը բաժանվում է տրամաբանական հատվածների՝ հեշտացնելով նրա ընթեռնելիությունը։
   
   3. **Կրկնակի օգտագործում:**
      - Module Pattern-ը հիանալի է տրամաբանական միավորներ կառուցելու և վերաօգտագործելու համար։
   
   4. **Անկախություն:**
      - Կանխում է գլոբալ փոփոխականների բախումը։
   
   ---
   
   #### Module Pattern-ի թերությունները
   
   1. **Դանդաղություն մեծ ծրագրերում:**
      - Ամեն նոր մոդուլ ստեղծելիս կարող է ավելացնել լրացուցիչ բեռնավորվածություն։
   
   2. **Մասնավոր տարրերի թեստավորում:**
      - Մասնավոր փոփոխականներն ու մեթոդները դժվար է թեստավորել։
   
   3. **Կոդի բարդություն:**
      - Module Pattern-ը կարող է ավելացնել կոդի բարդությունը սկսնակների համար։
   
   ---
   
   #### Module Pattern-ի օգտագործման դեպքեր
   
   1. **Տվյալների անվտանգ պահպանում:**
      Օրինակ՝ վավերացնող կոդում կամ API բանալիները գաղտնի պահելու համար։
   
   2. **Կոդի կազմակերպում մեծ ծրագրերում:**
      Օգտագործվում է մեծ ծրագրերում կոդը բաժանելու տրամաբանական մոդուլների։
   
   3. **Տեղեկատվական վահանակներ (Dashboard):**
      Ապահովում է տեսողական և գործառնական տվյալների կառավարման մոդուլներ։
   
   ---
   
   #### Module Pattern-ը ES6-ում
   
   ES6-ում Module Pattern-ը հաճախ կիրառվում է `export` և `import` սինտաքսի միջոցով։
   
   #### Օրինակ՝ ES6 Մոդուլ
   
   ```javascript
   // module.js
   const privateVar = "This is private";
   
   function privateMethod() {
     console.log(privateVar);
   }
   
   export function publicMethod() {
     console.log("Accessing private method:");
     privateMethod();
   }
   ```
   
   ```javascript
   // main.js
   import { publicMethod } from './module.js';
   
   publicMethod(); // "Accessing private method:" "This is private"
   ```

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

33. ### Ինչ տարբերություն կա mutable և immutable օբյեկտների միջև?
   
   **Mutable** և **Immutable** օբյեկտները երկու հիմնական կատեգորիաներ են JavaScript-ում, որոնք սահմանում են, թե ինչպես են տվյալները պահվում և փոփոխվում հիշողության մեջ։
   
   - **Mutable (Փոփոխվող):** Օբյեկտները, որոնք կարելի է փոխել տեղում՝ առանց նոր instance ստեղծելու։
   - **Immutable (Անփոփոխ):** Օբյեկտները, որոնք չեն փոխվում տեղում, և ցանկացած փոփոխություն ստեղծում է նոր instance։

   ---
   
   #### Mutable օբյեկտներ
   
   #### Նկարագրություն
   
   Mutable օբյեկտները թույլ են տալիս տվյալները փոխել տեղում՝ առանց նոր instance ստեղծելու։
   
   - Օբյեկտների և զանգվածների մեծ մասը JavaScript-ում mutable են։
   - Փոփոխությունները ազդում են օբյեկտի բոլոր հղումների վրա, որոնք պահում են նույն instance-ը։
   
   #### Օրինակ
   
   ```javascript
   let obj = { name: "Alice" };
   obj.name = "Bob";
   
   console.log(obj.name); // "Bob"
   ```
   
   ```javascript
   let array = [1, 2, 3];
   array.push(4);
   
   console.log(array); // [1, 2, 3, 4]
   ```
   
   #### Առավելություններ
   
   1. Ավելի քիչ հիշողություն է օգտագործվում, քանի որ փոփոխությունները կատարվում են տեղում։
   2. Արդյունավետ են մեծ տվյալների կառավարման համար։
   
   #### Թերություններ
   
   1. Կարող է առաջացնել սխալներ՝ փոփոխությունների հետ կապված, եթե նույն instance-ը օգտագործվում է տարբեր վայրերում։
   2. Հիշողության կառավարումը դառնում է ավելի բարդ։
   
   ---
   
   #### Immutable օբյեկտներ
   
   #### Նկարագրություն
   
   Immutable օբյեկտները չեն փոփոխվում տեղում։ Օրինակ՝ յուրաքանչյուր փոփոխություն ստեղծում է նոր instance։
   
   - Primitive արժեքները (օրինակ՝ `string`, `number`, `boolean`) immutable են JavaScript-ում։
   - Նույնպես կարելի է ստեղծել immutable կառուցվածքներ `Object.freeze` կամ հատուկ գրադարանների միջոցով։
   
   #### Օրինակ
   
   #### Primitive արժեքներ
   
   ```javascript
   let str = "Hello";
   let newStr = str + " World";
   
   console.log(str); // "Hello"
   console.log(newStr); // "Hello World"
   ```
   
   #### Object.freeze()
   
   ```javascript
   const obj = Object.freeze({ name: "Alice" });
   obj.name = "Bob"; // Չի փոխվում
   
   console.log(obj.name); // "Alice"
   ```
   
   #### Using Libraries (Immutable.js)
   
   ```javascript
   const { Map } = require('immutable');
   
   const map1 = Map({ name: "Alice" });
   const map2 = map1.set("name", "Bob");
   
   console.log(map1.get("name")); // "Alice"
   console.log(map2.get("name")); // "Bob"
   ```
   
   #### Առավելություններ
   
   1. Ավելի հեշտ է հետևել փոփոխություններին, քանի որ փոփոխություններն են ստեղծում նոր instance։
   2. Կանխում է անցանկալի կողմնակի ազդեցությունները։
   3. Հարմար է ֆունկցիոնալ ծրագրավորման մոտեցումների համար։
   
   #### Թերություններ
   
   1. Արդյունավետության խնդիրներ մեծ տվյալների հետ աշխատելիս, քանի որ փոփոխությունները ստեղծում են նոր instance։
   2. Ավելի շատ հիշողություն է օգտագործվում։
   
   ---
   
   #### Հիմնական Տարբերությունները
   
   | **Հատկանիշ**             | **Mutable**                          | **Immutable**                      |
   |---------------------------|---------------------------------------|-------------------------------------|
   | **Փոփոխություն տեղում**    | Այո                                   | Ոչ                                 |
   | **Instance-ի քանակը**     | Միայն մեկ                            | Յուրաքանչյուր փոփոխություն ստեղծում է նորը |
   | **Կողմնակի ազդեցություններ** | Հնարավոր է                           | Չի լինում                           |
   | **Օրինակներ**             | Object, Array                        | String, Number, Immutable.js        |

   ---


**[⬆ Back to Top](#բովանդակություն)**

   ---

34. ### Ինչպես են աշխատում setters և getters JavaScript-ում?

   **Setters** և **Getters**-ը JavaScript-ում հատուկ մեթոդներ են, որոնք օգտագործվում են օբյեկտների հատկությունների արժեքները ստանալու (get) կամ սահմանելու (set) համար։ Դրանք թույլ են տալիս վերահսկել, թե ինչպես են հատկությունները ընթերցվում կամ փոփոխվում՝ առանց ուղղակիորեն մուտք գործելու տվյալ օբյեկտի հատկությունները։
   
   Setters-ը և Getters-ը կիրառվում են, երբ ցանկանում ենք ապահովել տվյալների գաղտնիություն և վերահսկում, ինչպես նաև տրամադրել հատկությունների հաշվարկային կամ վավերացված արժեքներ։
   
   ---
   
   #### Սինտաքս
   
   Setters և Getters օգտագործելու համար ստեղծվում են համապատասխան `get` և `set` մեթոդներ օբյեկտի հատկությունների վրա։
   
   ```javascript
   let obj = {
     // Getter մեթոդ
     get propertyName() {
       return this._propertyName;
     },
   
     // Setter մեթոդ
     set propertyName(value) {
       this._propertyName = value;
     }
   };
   ```
   
   - **`get` մեթոդը** օգտագործվում է հատկության արժեքը ստանալու համար։
   - **`set` մեթոդը** օգտագործվում է հատկության արժեքը փոփոխելու համար։
   - Սովորաբար `_propertyName`-ը կիրառվում է որպես մասնավոր փոփոխական (private variable), որը պահում է հատկության արժեքը։

   ---
   
   #### Օրինակներ
   
   #### 1. Հիմնական Օրինակ
   
   Ստեղծենք օբյեկտ, որը պարունակում է `name` հատկություն, որը կարելի է ստանալ կամ փոփոխել `get` և `set` մեթոդներով։
   
   ```javascript
   let user = {
     _name: "Alice",
   
     // Getter մեթոդ՝ արժեք ստանալու համար
     get name() {
       return this._name;
     },
   
     // Setter մեթոդ՝ արժեք փոփոխելու համար
     set name(value) {
       if (value.length > 0) {
         this._name = value;
       } else {
         console.log("Name cannot be empty");
       }
     }
   };
   
   console.log(user.name); // "Alice"
   user.name = "Bob";
   console.log(user.name); // "Bob"
   user.name = ""; // "Name cannot be empty"
   ```
   
   #### 2. Հաշվարկային Հատկություններ
   
   Setters և Getters մեթոդները կարող են կիրառվել հաշվարկային հատկությունների համար, ինչպիսիք են տարածքը կամ ծավալը։
   
   ```javascript
   let rectangle = {
     _width: 0,
     _height: 0,
   
     // Getter՝ տարածքը հաշվարկելու համար
     get area() {
       return this._width * this._height;
     },
   
     // Setter՝ լայնությունը սահմանելու համար
     set width(value) {
       this._width = value;
     },
   
     // Setter՝ բարձրությունը սահմանելու համար
     set height(value) {
       this._height = value;
     }
   };
   
   rectangle.width = 10;
   rectangle.height = 5;
   console.log(rectangle.area); // 50
   ```
   
   #### 3. Օգտագործումը class-երում
   
   Setters և Getters մեթոդները հաճախ օգտագործվում են JavaScript-ի class-երում՝ օբյեկտների վրա հավելյալ վերահսկում ապահովելու համար։
   
   ```javascript
   class User {
     constructor(name) {
       this._name = name;
     }
   
     // Getter մեթոդ՝ արժեք ստանալու համար
     get name() {
       return this._name;
     }
   
     // Setter մեթոդ՝ արժեք փոփոխելու համար
     set name(value) {
       if (value.length > 0) {
         this._name = value;
       } else {
         console.log("Name cannot be empty");
       }
     }
   }
   
   let user = new User("Alice");
   console.log(user.name); // "Alice"
   user.name = "Charlie";
   console.log(user.name); // "Charlie"
   user.name = ""; // "Name cannot be empty"
   ```

   ---
   
   #### Ինչու օգտագործել Setters և Getters
   
   Setters և Getters մեթոդները JavaScript-ում ունեն մի քանի կարևոր առավելություններ՝
   
   1. **Տվյալների Վավերացում (Validation):**
      - `set` մեթոդի միջոցով կարող եք սահմանափակել, թե ինչ արժեքներ կարող են մուտք գործել օբյեկտի հատկությանը։
   
      ```javascript
      let user = {
        _age: 0,
   
        set age(value) {
          if (value > 0) {
            this._age = value;
          } else {
            console.log("Age must be a positive number");
          }
        },
   
        get age() {
          return this._age;
        }
      };
   
      user.age = 25;
      console.log(user.age); // 25
      user.age = -5; // "Age must be a positive number"
      ```
   
   2. **Կոդի Կարդացելիություն (Readability):**
      - Օգտագործելով `get` և `set`, կարող եք գրել ավելի ընթեռնելի կոդ՝ առանց մեթոդներ կանչելու։
   
      ```javascript
      console.log(user.age); // Ավելի ընթեռնելի, քան user.getAge()
      ```
   
   3. **Հաշվարկային Հատկություններ (Computed Properties):**
      - Կարող եք օգտագործել `get` մեթոդը՝ հաշվողական հատկություններ դինամիկ ստեղծելու համար։
   
   4. **Մասնավոր Տվյալների Կառավարում:**
      - Մասնավոր հատկությունները հնարավոր է կառավարել միայն `get` և `set` մեթոդների միջոցով։
   
   ---
   
   #### Թերություններ
   
   1. **Բարդություն:**
      - Setters և Getters-ը կարող են ավելի բարդ թվալ սկսնակ ծրագրավորողների համար։
   
   2. **Արդյունավետության խնդիրներ:**
      - Եթե `get` կամ `set` մեթոդները կատարում են բարդ հաշվարկներ, դրանք կարող են նվազեցնել ծրագրի արդյունավետությունը։
   
   ---


**[⬆ Back to Top](#բովանդակություն)**

   ---

35. ### Ինչ է տարբերություն function declaration-ի և function expression-ի միջև?

   
   JavaScript-ում ֆունկցիաները կարելի է հայտարարել երկու հիմնական ձևերով՝ **Function Declaration** (ֆունկցիայի հայտարարում) և **Function Expression** (ֆունկցիայի արտահայտություն): Չնայած դրանք երկուսն էլ ծառայում են ֆունկցիաներ ստեղծելու համար, դրանք ունեն տարբեր վարքագիծ և օգտագործման դեպքեր։

   ---
   
   #### Function Declaration
   
   **Function Declaration**-ը ֆունկցիայի ստեղծման գործընթաց է, որտեղ ֆունկցիան հայտարարվում է իր անունով և կարող է օգտագործվել իր հայտարարման նախքան։
   
   #### Սինտաքս
   
   ```javascript
   function functionName(parameters) {
     // ֆունկցիայի մարմին
   }
   ```
   
   #### Օրինակ
   
   ```javascript
   function greet() {
     console.log("Hello!");
   }
   
   greet(); // "Hello!"
   ```
   
   #### Հատկանիշներ
   
   1. **Hoisting (բարձրացում):**
      - Function Declaration-ները "բարձրացվում" են իրենց տիրույթի սկզբին։ Սա նշանակում է, որ կարող եք օգտագործել ֆունկցիան, նախքան այն հայտարարվել է։
   
      ```javascript
      greet(); // "Hello!"
   
      function greet() {
        console.log("Hello!");
      }
      ```
   
   2. **Տիրույթ:**
      - Function Declaration-ները հասանելի են իրենց ամբողջ տիրույթում։
   
   3. **Ֆունկցիայի անուն:**
      - Ֆունկցիան պետք է ունենա անուն։
   
   ---
   
   #### Function Expression
   
   **Function Expression**-ը ֆունկցիա է, որը հայտարարվում է որպես արտահայտություն և կարող է վերագրվել փոփոխականին։
   
   #### Սինտաքս
   
   ```javascript
   const functionName = function(parameters) {
     // ֆունկցիայի մարմին
   };
   ```
   
   #### Օրինակ
   
   ```javascript
   const greet = function() {
     console.log("Hello!");
   };
   
   greet(); // "Hello!"
   ```
   
   #### Հատկանիշներ
   
   1. **Hoisting (բարձրացում):**
      - Function Expression-ները չեն "բարձրացվում"։ Սա նշանակում է, որ ֆունկցիան հնարավոր չէ կանչել, նախքան այն հայտարարվել է։
   
      ```javascript
      greet(); // ReferenceError: Cannot access 'greet' before initialization
   
      const greet = function() {
        console.log("Hello!");
      };
      ```
   
   2. **Տիրույթ:**
      - Function Expression-ները հասանելի են միայն այն բլոկում, որտեղ հայտարարվել են։
   
   3. **Անանուն ֆունկցիաներ:**
      - Function Expression-ները կարող են լինել անանուն (այսինքն՝ ֆունկցիան չունի անուն):
   
      ```javascript
      const greet = function() {
        console.log("Hello!");
      };
      ```

   ---
   
   #### Հիմնական Տարբերությունները
   
   | **Հատկանիշ**              | **Function Declaration**                       | **Function Expression**                       |
   |----------------------------|-----------------------------------------------|-----------------------------------------------|
   | **Սինտաքս**               | `function name() {}`                          | `const name = function() {}`                 |
   | **Hoisting**               | "Բարձրացվում է" տիրույթի սկզբին               | Չի "բարձրացվում"                              |
   | **Անանուն ֆունկցիաներ**   | Պարտադիր անունով                              | Կարող է լինել անանուն                          |
   | **Օգտագործման տեղը**       | Հասանելի է ամբողջ տիրույթում                  | Հասանելի է միայն այն հատվածում, որտեղ հայտարարվել է |

   ---
   
   #### Arrow Function Expression
   
   Function Expression-ի ենթատեսակ է նաև **Arrow Function**-ը, որը ներդրվել է ES6-ում։ Այն ապահովում է ավելի կարճ սինտաքս և չի կապում իր սեփական `this` արժեքը։
   
   #### Օրինակ
   
   ```javascript
   const greet = () => {
     console.log("Hello!");
   };
   
   greet(); // "Hello!"
   ```

   ---
   
   #### Եզրակացություն
   
   - **Function Declaration**-ները հարմար են այն դեպքերում, երբ ֆունկցիան պետք է հասանելի լինի ամբողջ տիրույթում և օգտագործվի մինչև իր հայտարարումը։
   - **Function Expression**-ները ավելի ճկուն են և կարող են օգտագործվել դինամիկ կամ լոկալ ֆունկցիաներ ստեղծելու համար։
   - Ընտրությունը կախված է ծրագրի կառուցվածքից և պահանջներից։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

36. ### Ինչ է Higher Order Function-ը JavaScript-ում?

   
   **Higher Order Function**-ը (HOF) JavaScript-ում ֆունկցիա է, որը կատարում է առնվազն հետևյալ գործողություններից մեկը՝
   
   1. Ստանում է մեկ կամ ավելի ֆունկցիա որպես պարամետր։
   2. Վերադարձնում է նոր ֆունկցիա որպես արդյունք։
   
   Higher Order Function-ները կարևոր են ֆունկցիոնալ ծրագրավորման մեջ և թույլ են տալիս գրել մաքուր, մոդուլային և վերաօգտագործելի կոդ։

   ---
   
   #### Հիմնական առանձնահատկություններ
   
   1. **Ֆունկցիաներ՝ որպես առաջին կարգի օբյեկտներ (First-Class Objects):**
      JavaScript-ում ֆունկցիաները կարող են պահվել փոփոխականներում, փոխանցվել որպես պարամետրեր և վերադարձվել այլ ֆունկցիաներից։
   
   2. **Հարմարավետություն կոմպոզիցիայի համար:**
      Higher Order Function-ները հնարավորություն են տալիս կոդը բաժանել փոքր, վերաօգտագործելի մասերի։
   
   ---
   
   #### Օրինակներ
   
   #### 1. Օրինակ՝ Փոխանցում ֆունկցիա որպես պարամետր
   
   ```javascript
   function greet(name) {
     return `Hello, ${name}!`;
   }
   
   function processUserInput(callback) {
     const name = "Alice";
     console.log(callback(name));
   }
   
   processUserInput(greet);
   // Output: "Hello, Alice!"
   ```
   
   #### 2. Օրինակ՝ Վերադարձնում է ֆունկցիա
   
   ```javascript
   function multiplier(factor) {
     return function(number) {
       return number * factor;
     };
   }
   
   const double = multiplier(2);
   const triple = multiplier(3);
   
   console.log(double(5)); // 10
   console.log(triple(5)); // 15
   ```
   
   #### 3. Array Higher Order Functions
   
   JavaScript-ում ներկառուցված Higher Order Function-ներ են `map`, `filter`, և `reduce` մեթոդները։
   
   #### Օրինակ՝ `map`
   
   ```javascript
   const numbers = [1, 2, 3, 4, 5];
   const squared = numbers.map(num => num * num);
   
   console.log(squared); // [1, 4, 9, 16, 25]
   ```
   
   #### Օրինակ՝ `filter`
   
   ```javascript
   const numbers = [1, 2, 3, 4, 5];
   const evenNumbers = numbers.filter(num => num % 2 === 0);
   
   console.log(evenNumbers); // [2, 4]
   ```
   
   #### Օրինակ՝ `reduce`
   
   ```javascript
   const numbers = [1, 2, 3, 4, 5];
   const sum = numbers.reduce((acc, num) => acc + num, 0);
   
   console.log(sum); // 15
   ```
   
   ---
   
   #### Ինչու օգտագործել Higher Order Function-ներ
   
   1. **Կոդի վերաօգտագործում:**
      Higher Order Function-ները թույլ են տալիս մեկ անգամ գրել ընդհանուր լուծումներ և օգտագործել դրանք տարբեր դեպքերում։
   
   2. **Կոդի մաքրություն և ընթեռնելիություն:**
      Կոդը դառնում է ավելի ընթեռնելի և մոդուլային՝ բաժանելով խնդիրները ավելի փոքր մասերի։
   
   3. **Դինամիկություն:**
      Higher Order Function-ները թույլ են տալիս ծրագրին դինամիկ կերպով փոխել իր վարքագիծը։

   ---
   
   #### Հիմնական տարբերություններ սովորական ֆունկցիաներից
   
   | **Հատկանիշ**              | **Սովորական Ֆունկցիա**                | **Higher Order Function**            |
   |---------------------------|--------------------------------------|--------------------------------------|
   | **Ֆունկցիա ստանում է որպես պարամետր** | Ոչ                                   | Այո                                  |
   | **Վերադարձնում է ֆունկցիա** | Ոչ                                   | Այո                                  |
   | **Օգտագործման դեպքեր**     | Հիմնական հաշվարկներ                  | Մոդուլային և վերաօգտագործելի լուծումներ |

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

37. ### Ինչ է Currying-ը JavaScript-ում?

   **Currying**-ը ֆունկցիաների փոխակերպման տեխնիկա է, որը թույլ է տալիս ֆունկցիան ընդունել մեկական պարամետր՝ փոխարենը միանգամից ստանալ բոլոր պարամետրերը։ Currying-ի դեպքում ֆունկցիան վերադարձնում է նոր ֆունկցիա, որը սպասում է հաջորդ պարամետրի փոխանցմանը։
   
   Currying-ը հաճախ օգտագործվում է ֆունկցիոնալ ծրագրավորման մեջ, որտեղ մեծ ուշադրություն է դարձվում փոքր և մոդուլային ֆունկցիաների օգտագործմանը։

   ---
   
   #### Ինչու օգտագործել Currying
   
   1. **Կոդի վերաօգտագործում:**
      - Currying-ը թույլ է տալիս ստեղծել մասնագիտացված ֆունկցիաներ ավելի մեծ ֆունկցիաներից։
   
   2. **Կոդի ընթեռնելիություն:**
      - Currying-ի միջոցով ֆունկցիաների լոգիկան դառնում է ավելի պարզ և ընթեռնելի։
   
   3. **Ֆունկցիոնալ ծրագրավորում:**
      - Ֆունկցիոնալ ծրագրավորման մոտեցումները հաճախ հիմնված են Currying-ի վրա, ինչը հեշտացնում է ֆունկցիաների կոմպոզիցիան։

   ---
   
   #### Օրինակ՝ Currying-ի պարզ կիրառում
   
   ```javascript
   function multiply(a) {
     return function(b) {
       return a * b;
     };
   }
   
   const multiplyByTwo = multiply(2);
   console.log(multiplyByTwo(5)); // 10
   
   const multiplyByThree = multiply(3);
   console.log(multiplyByThree(5)); // 15
   ```
   
   #### Բացատրություն
   
   - Առաջին կանչով `multiply(2)` ֆունկցիան պահպանում է `a = 2` արժեքը։
     - Վերադարձված ֆունկցիան սպասում է երկրորդ պարամետրի `b`-ի արժեքին։
   
   ---
   
   #### Օրինակ՝ Ներդրված ֆունկցիաների օգտագործում
   
   Currying-ի դեպքում կարող եք ստեղծել ավելի բարդ կառուցվածքներ՝ վերբեռնելով բազմաթիվ պարամետրեր։
   
   ```javascript
   function add(a) {
     return function(b) {
       return function(c) {
         return a + b + c;
       };
     };
   }
   
   console.log(add(1)(2)(3)); // 6
   ```
   
   ---
   
   #### Currying՝ Օգտագործելով Arrow Function
   
   JavaScript-ում կարող եք օգտագործել Arrow Function-ներ՝ Currying-ը պարզեցնելու համար։
   
   ```javascript
   const add = a => b => c => a + b + c;
   
   console.log(add(1)(2)(3)); // 6
   ```
   
   ---
   
   #### Առավելություններ
   
   1. **Հարմար է մասնակի կիրառման համար (Partial Application):**
      - Currying-ը թույլ է տալիս ստեղծել նոր ֆունկցիաներ՝ տալով միայն մի մաս պարամետրերի։
   
      ```javascript
      const greet = greeting => name => `${greeting}, ${name}!`;
   
      const sayHello = greet("Hello");
      console.log(sayHello("Alice")); // "Hello, Alice!"
      console.log(sayHello("Bob"));   // "Hello, Bob!"
      ```
   
   2. **Կոմպոզիցիա (Composition):**
      - Currying-ը հեշտացնում է ֆունկցիաների կոմպոզիցիան, որտեղ մեկ ֆունկցիայի արդյունքը փոխանցվում է որպես պարամետր մյուսին։
   
   3. **Լոգիկայի պարզեցում:**
      - Բարդ ֆունկցիաները կարելի է բաժանել ավելի փոքր մասերի՝ ավելի հեշտ վերահսկելի դարձնելու համար։

   ---
   
   #### Currying-ի և Normale ֆունկցիաների տարբերությունը
   
   | **Հատկանիշ**                | **Նորմալ Ֆունկցիա**                   | **Curried Ֆունկցիա**                 |
   |-----------------------------|--------------------------------------|-------------------------------------|
   | **Պարամետրերի փոխանցում**    | Բոլոր պարամետրերը միանգամից           | Մեկական պարամետր                  |
   | **Կառուցվածք**               | Պարզ                                  | Ներդրված ֆունկցիաներ               |
   | **Օգտագործման դեպքեր**       | Սովորական ֆունկցիաներ                 | Ֆունկցիոնալ ծրագրավորում, մասնակի կիրառություն |

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---


38. ### Ինչ է JavaScript-ի Task Queue-ը?

   
   **Task Queue**-ը JavaScript-ում կարևոր մասն է, որը կառավարում է այն գործառույթների հերթականությունը, որոնք սպասում են կատարման։ Task Queue-ը աշխատում է **Event Loop**-ի հետ համատեղ՝ ապահովելով ասինխրոն գործառույթների ճիշտ կատարման հաջորդականությունը։
   
   Task Queue-ը հիմնականում պատասխանատու է այն callback-ների կառավարման համար, որոնք պետք է կատարվեն, երբ առաջադրանքը (task) ավարտվում է, օրինակ՝ **setTimeout**, **setInterval**, կամ **DOM Event**-եր։
   
   ---
   
   #### Ինչպես է աշխատում Task Queue-ը
   
   1. Երբ ծրագրում հանդիպում է ասինխրոն գործողություն (օրինակ՝ **setTimeout**, **fetch**), այն փոխանցվում է համապատասխան **Web API**-ին կամ **Node.js API**-ին։
   2. Ասինխրոն գործողությունը կատարվում է API-ի կողմից։
   3. Երբ գործողությունը ավարտվում է, նրա callback-ը տեղափոխվում է Task Queue։
   4. **Event Loop**-ը ստուգում է՝ արդյոք Call Stack-ը (կատարման ստեկը) դատարկ է։
   5. Եթե Call Stack-ը դատարկ է, Event Loop-ը տեղափոխում է Task Queue-ից առաջին callback-ը Call Stack և կատարում այն։

   ---
   
   #### Task Queue-ի հիմնական բաղադրիչները
   
   1. **Call Stack (Կատարման Ստեկ):**
      - Կառավարում է սինխրոն կոդը։ Սկզբում բոլոր ֆունկցիաները կատարվում են այստեղ։
   
   2. **Web APIs:**
      - Սինխրոն գործողությունների համար պատասխանատու են JavaScript-ի միջավայրի առաջարկած API-ները։
   
   3. **Task Queue:**
      - Սպասում են callback-երը, մինչև Call Stack-ը դատարկվի։
   
   4. **Event Loop:**
      - Ապահովում է Task Queue-ից Call Stack-ի միջև համագործակցությունը։

   ---
   
   #### Task Queue-ի Օրինակ
   
   ```javascript
   console.log("Start");
   
   setTimeout(() => {
     console.log("Callback from setTimeout");
   }, 0);
   
   console.log("End");
   ```
   
   **Արդյունք:**
   
   ```plaintext
   Start
   End
   Callback from setTimeout
   ```
   
   **Բացատրություն:**
   1. "Start"-ը և "End"-ը անմիջապես կատարվում են, քանի որ դրանք սինխրոն կոդ են։
   2. **setTimeout**-ը փոխանցում է callback-ը Task Queue-ին, բայց այն կատարվում է միայն այն բանից հետո, երբ Call Stack-ը դատարկվում է։

   ---
   
   #### Task Queue-ի և Microtask Queue-ի Տարբերությունները
   
   JavaScript-ում գոյություն ունի նաև **Microtask Queue**։ Այն հիմնականում օգտագործվում է **Promises**, **MutationObserver**-ի և այլնի համար։
   
   #### Հիմնական տարբերությունները
   
   | **Հատկանիշ**              | **Task Queue**                         | **Microtask Queue**                     |
   |---------------------------|----------------------------------------|----------------------------------------|
   | **Օգտագործվում է**         | setTimeout, setInterval, I/O          | Promises, MutationObserver             |
   | **Կատարման առաջնահերթություն** | Կատարվում է հետո                     | Կատարվում է անմիջապես                  |
   
   #### Օրինակ՝ Task Queue vs Microtask Queue
   
   ```javascript
   console.log("Start");
   
   setTimeout(() => {
     console.log("Task Queue");
   }, 0);
   
   Promise.resolve().then(() => {
     console.log("Microtask Queue");
   });
   
   console.log("End");
   ```
   
   **Արդյունք:**
   
   ```plaintext
   Start
   End
   Microtask Queue
   Task Queue
   ```
   
   **Բացատրություն:**
   - **Promises**-ի callback-ը (Microtask) կատարվում է մինչև Task Queue-ի callback-ը։
   
   ---
   
   #### Ինչու է Task Queue-ը կարևոր
   
   1. **Ասինխրոնության կառավարում:**
      - Task Queue-ը ապահովում է ասինխրոն գործողությունների կարգավորված կատարման հաջորդականությունը։
   
   2. **UI-ի արձագանքման բարելավում:**
      - Task Queue-ը թույլ է տալիս բրաուզերին վերաանկարչել UI-ն և կատարել ֆունկցիաներ՝ առանց սառեցնելու։
   
   3. **Կոդի կանխատեսելիություն:**
      - Կատարումն ավելի հեշտ է հասկանալ Event Loop-ի և Task Queue-ի մեխանիզմների շնորհիվ։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---


39. ### Ինչ է JavaScript-ում տարբեր սխալների տեսակները (SyntaxError, ReferenceError, TypeError)?

   JavaScript-ում սխալները (errors) հանդիպում են կոդի գրության կամ կատարման ընթացքում և բաժանվում են տարբեր տեսակների՝ կախված սխալի բնույթից։ Ճիշտ հասկանալը, թե ինչ են նշանակում տարբեր սխալները, կարևոր է ծրագրավորողների համար, քանի որ դա օգնում է գտնել և շտկել խնդիրները։

   ---
   
   #### 1. SyntaxError (Սինտաքսի սխալ)
   
   **SyntaxError**-ը տեղի է ունենում, երբ կոդի սինտաքսը սխալ է, այսինքն՝ JavaScript-ի շարժիչը չի կարողանում հասկանալ գրված կոդը։
   
   #### Երբ է առաջանում
   - Երբ բացակայում են անհրաժեշտ փակագծերը կամ կետադրական նշանները։
   - Երբ օգտագործվում են ոչ վավեր JavaScript-ի սինտաքս։
   
   #### Օրինակներ
   
   #### Բացակայում է փակագիծը
   ```javascript
   console.log("Hello World"; // SyntaxError: Unexpected token ')'
   ```
   
   #### Անվավեր ֆունկցիա
   ```javascript
   function() {
     console.log("Invalid function");
   } // SyntaxError: Function statements require a name
   ```
   
   #### Արգելված վերապահված բառերի օգտագործում
   ```javascript
   var let = 5; // SyntaxError: Unexpected strict mode reserved word
   ```
   
   #### Ինչպես շտկել
   - Ուշադիր ստուգեք կոդի սինտաքսը։
   - Օգտագործեք IDE-ներ կամ լինթերներ, որոնք կարող են գտնել սինտաքսի սխալները։

   ---
   
   #### 2. ReferenceError (Հղման սխալ)
   
   **ReferenceError**-ը տեղի է ունենում, երբ փորձ է կատարվում մուտք գործել փոփոխական կամ ֆունկցիա, որը չի հայտարարվել։
   
   #### Երբ է առաջանում
   - Երբ փոփոխականը կամ ֆունկցիան չի հայտարարվել, բայց օգտագործվում է։
   - Երբ փորձ է կատարվում մուտք գործել բլոկի տիրույթում հայտարարված փոփոխականը՝ տիրույթից դուրս։
   
   #### Օրինակներ
   
   #### Փոփոխականը չի հայտարարվել
   ```javascript
   console.log(x); // ReferenceError: x is not defined
   ```
   
   #### Փոփոխականը հասանելի չէ իր տիրույթից դուրս
   ```javascript
   {
     let y = 10;
   }
   console.log(y); // ReferenceError: y is not defined
   ```
   
   #### Տառասխալ փոփոխականի անունում
   ```javascript
   let name = "Alice";
   console.log(nam); // ReferenceError: nam is not defined
   ```
   
   #### Ինչպես շտկել
   - Համոզվեք, որ փոփոխականները կամ ֆունկցիաները հայտարարված են նախքան դրանց օգտագործումը։
   - Ստուգեք տառասխալները։
   - Օգտագործեք JavaScript-ի լինթեր՝ տիրույթային խնդիրները հայտնաբերելու համար։
   
   ---
   
   #### 3. TypeError (Տիպի սխալ)
   
   **TypeError**-ը տեղի է ունենում, երբ գործողությունը անհնար է օբյեկտի կամ տվյալների տիպի համար։
   
   #### Երբ է առաջանում
   - Երբ փորձ է կատարվում կանչել ֆունկցիա, որը գոյություն չունի։
   - Երբ փորձ է կատարվում հատկություն մուտքագրել `undefined` կամ `null` արժեքի վրա։
   - Երբ գործողությունը չի համընկնում տվյալների տիպի հետ։
   
   #### Օրինակներ
   
   #### Փորձ կանչել ֆունկցիա, որը գոյություն չունի
   ```javascript
   let num = 5;
   num(); // TypeError: num is not a function
   ```
   
   #### Փորձ մուտք գործել հատկություն `undefined`-ի վրա
   ```javascript
   let obj;
   console.log(obj.name); // TypeError: Cannot read properties of undefined (reading 'name')
   ```
   
   #### Չհամապատասխանող գործողություն
   ```javascript
   let x = 10;
   x.toUpperCase(); // TypeError: x.toUpperCase is not a function
   ```
   
   #### Ինչպես շտկել
   - Համոզվեք, որ գործողությունները համընկնում են տվյալների տիպի հետ։
   - Ստուգեք, որ օբյեկտները և դրանց հատկությունները ճիշտ կերպով հասանելի են։
   - Արժեքները ստուգեք `undefined` կամ `null` լինելու համար՝ նախքան դրանց վրա գործողություններ կատարելը։
   
   ```javascript
   let obj;
   if (obj && obj.name) {
     console.log(obj.name);
   }
   ```
   
   ---

   #### Այլ Սխալների Տեսակներ
   
   JavaScript-ում կան նաև այլ սխալներ, որոնք արժե նշել.
   
   1. **RangeError:**
      - Առաջանում է, երբ արժեքը դուրս է գալիս թույլատրելի միջակայքից։
      ```javascript
      let num = 1;
      num.toFixed(100); // RangeError: toFixed() digits argument must be between 0 and 100
      ```
   
   2. **EvalError:**
      - Առաջանում է, երբ ոչ ճիշտ կերպով օգտագործվում է `eval()`-ը (հազվադեպ հանդիպող սխալ):
   
   3. **URIError:**
      - Առաջանում է, երբ URI-ի հետ կապված մեթոդներում (օր.`decodeURIComponent`) օգտագործվում է անվավեր սինտաքս։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

40. ### Ինչ է JavaScript-ի Garbage Collection-ը?

   
   **Garbage Collection**-ը (GC) JavaScript-ի մեխանիզմ է, որը ավտոմատ կերպով կառավարում է հիշողությունը՝ ազատելով այն օբյեկտներից, որոնք այլևս օգտագործման մեջ չեն։ JavaScript-ը ունի ավտոմատ հիշողության կառավարում, ինչը նշանակում է, որ ծրագրավորողները պարտադիր չեն, որ մաքրեն չօգտագործվող տվյալները, բայց պետք է հասկանան GC-ի աշխատանքը՝ օպտիմալ կոդ գրելու համար։
   
   ---
   
   #### Ինչպես է աշխատում Garbage Collection-ը
   
   JavaScript-ը օգտագործում է **Reachability (Հասանելիություն)**-ի վրա հիմնված ալգորիթմներ՝ որոշելու, թե որ օբյեկտները պետք է հեռացվեն հիշողությունից։
   
   #### Reachability-ի մեխանիզմը
   
   Օբյեկտը համարվում է հասանելի, եթե այն կարող է հասանելի լինել ծրագրում որևէ կետից։ Հիմնական հասանելի օբյեկտներն են՝
   
   1. **Global Object:**
      - Օրինակ՝ բրաուզերում դա `window` օբյեկտն է։
   
   2. **Կատարման Stack (Call Stack):**
      - Ակտիվ ֆունկցիաների փոփոխականները և պարամետրերը։
   
   3. **Կապված Closure-ներ:**
      - Ֆունկցիաները, որոնք պահպանում են իրենց ծնող տիրույթները։
   
   Հասանելի օբյեկտները կոչվում են **Root**։ Եթե օբյեկտը չի կարող հասանելի լինել ոչ մի Root-ից, այն համարվում է անօգտագործվող և ենթակա է հեռացման։

   ---
   
   #### Garbage Collection-ի Ալգորիթմներ
   
   JavaScript-ի շարժիչները (օրինակ՝ V8-ը) օգտագործում են տարբեր ալգորիթմներ Garbage Collection-ը իրականացնելու համար։
   
   #### 1. Mark-and-Sweep
   
   Այս հիմնական ալգորիթմը հետևյալ քայլերով է աշխատում՝
   
   1. Սկսում է Root օբյեկտներից։
   2. Նշում (mark) է բոլոր օբյեկտները, որոնք հասանելի են Root-ներից։
   3. Հեռացնում է բոլոր չնշված օբյեկտները։
   
   ```plaintext
   Root -> Object A -> Object B
   Root -> Object C
   
   Object D (չնշված) -> Հեռացվում է
   ```
   
   #### 2. Reference Counting
   
   Reference Counting ալգորիթմը հետևում է, թե քանի հղում ունի յուրաքանչյուր օբյեկտ։ Եթե օբյեկտի հղումների քանակը դառնում է 0, այն հեռացվում է։
   
   #### Թերություններ
   - **Circular References (Շրջանակային հղումներ):** Reference Counting-ը չի կարողանում կառավարել շրջանաձև հղումները։
   
   ```javascript
   let objA = {};
   let objB = {};
   
   objA.ref = objB;
   objB.ref = objA;
   
   objA = null;
   objB = null;
   // Շրջանաձև հղումները խանգարում են հեռացմանը
   ```
   
   ---
   
   #### Garbage Collection-ի Օրինակ
   
   ```javascript
   function createObject() {
     let obj = { name: "Alice" };
     console.log(obj.name);
   }
   
   createObject();
   // obj-ն այլևս հասանելի չէ և կհանվի հիշողությունից
   ```

   ---
   
   #### Circular References-ի Կառավարում
   
   JavaScript-ի ժամանակակից շարժիչները (օրինակ՝ V8) կարողանում են հայտնաբերել և կառավարել շրջանաձև հղումները։
   
   ```javascript
   let objA = { name: "A" };
   let objB = { name: "B" };
   
   objA.ref = objB;
   objB.ref = objA;
   
   objA = null;
   objB = null;
   // Շրջանաձև հղումները կհանվեն V8-ի միջոցով
   ```

   ---
   
   #### Ավելի Օպտիմալ Հիշողության Կառավարում
   
   Թեև Garbage Collection-ը ավտոմատ է, ծրագրավորողները կարող են գրել ավելի արդյունավետ կոդ՝ հետևյալ սկզբունքներով՝
   
   1. **Օգտագործվող Օբյեկտների Մաքրում:**
      - Ազատեք փոփոխականների հղումները, երբ դրանք այլևս չեն օգտագործվում։
   
      ```javascript
      let obj = { name: "Alice" };
      obj = null; // Հղումը հանվեց
      ```
   
   2. **Closure-ների ճիշտ օգտագործում:**
      - Խուսափեք closure-ներում ավելորդ տվյալների պահպանումից։
   
   3. **Զգուշություն Circular References-ից:**
      - Կարիք չկա ձեռքով կառավարել դրանք ժամանակակից շարժիչներում, բայց լավ պրակտիկան կարևոր է։
   
   ---
   
   #### Թերություններ
   
   1. **Ավելի մեծ ծախսեր մեծ ծրագրերում:**
      - Garbage Collection-ը կարող է ժամանակ առնել՝ դանդաղեցնելով ծրագիրը։
   
   2. **Հիշողության արտահոսք (Memory Leak):**
      - Չնայած GC-ը ավտոմատ է, սխալ կոդը կարող է ստեղծել հիշողության արտահոսք։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

41. ### Ինչ է Promise Chaining-ը JavaScript-ում?

   
   **Promise Chaining**-ը JavaScript-ում տեխնիկա է, որը թույլ է տալիս կապել մի քանի ասինխրոն գործողություններ այնպես, որ հաջորդ գործողությունը կատարվի նախորդի ավարտից հետո։ Դա իրականացվում է `then()` մեթոդի միջոցով, որը վերադարձնում է նոր **Promise**, որը կարելի է շարունակում օգտագործել հաջորդ `then()`-ում։
   
   Promise Chaining-ը օգնում է խուսափել "callback hell"-ից, որտեղ ներդրված callback-ների պատճառով կոդը դառնում է դժվար ընթեռնելի։
   
   ---
   
   #### Ինչպես է աշխատում Promise Chaining-ը
   
   Promise Chaining-ը կառուցվում է մի քանի քայլերից. յուրաքանչյուր `then()`-ը սպասում է նախորդ Promise-ի կատարմանը և վերադարձնում է նոր Promise:
   
   #### Օրինակ
   
   ```javascript
   const fetchData = () => {
     return new Promise((resolve, reject) => {
       setTimeout(() => resolve("Step 1: Data fetched"), 1000);
     });
   };
   
   fetchData()
     .then((result) => {
       console.log(result);
       return "Step 2: Data processed";
     })
     .then((result) => {
       console.log(result);
       return "Step 3: Finished";
     })
     .then((result) => {
       console.log(result);
     })
     .catch((error) => {
       console.error("Error:", error);
     });
   ```
   
   **Արդյունք:**
   
   ```plaintext
   Step 1: Data fetched
   Step 2: Data processed
   Step 3: Finished
   ```
   
   ---
   
   #### Promise Chaining-ի Հատկություններ
   
   1. **Վերադարձնում է նոր Promise:**
      - `then()`-ը միշտ վերադարձնում է նոր Promise, որը հնարավոր է շարունակել։
   
   2. **Error Handling (Սխալների կառավարում):**
      - Եթե որևէ Promise ավարտվում է սխալով, ապա հաջորդ `then()`-ները չեն կատարվում, և սխալը փոխանցվում է `catch()`-ին։
   
   #### Օրինակ՝ Error Handling
   
   ```javascript
   const stepOne = () => {
     return new Promise((resolve, reject) => {
       setTimeout(() => reject("Error in Step 1"), 1000);
     });
   };
   
   stepOne()
     .then((result) => {
       console.log(result);
       return "Step 2";
     })
     .then((result) => {
       console.log(result);
     })
     .catch((error) => {
       console.error("Caught error:", error);
     });
   ```
   
   **Արդյունք:**
   
   ```plaintext
   Caught error: Error in Step 1
   ```
   
   ---
   
   #### Բարդ Օրինակ՝ Fetch API-ի Օգտագործում
   
   Promise Chaining-ը հաճախ կիրառվում է API հարցումների (requests) արդյունքները շղթայաբար մշակելու համար։
   
   ```javascript
   fetch("https://jsonplaceholder.typicode.com/posts/1")
     .then((response) => {
       if (!response.ok) {
         throw new Error("Network response was not ok");
       }
       return response.json();
     })
     .then((data) => {
       console.log("Post Title:", data.title);
       return fetch("https://jsonplaceholder.typicode.com/users/1");
     })
     .then((response) => response.json())
     .then((user) => {
       console.log("User Name:", user.name);
     })
     .catch((error) => {
       console.error("Error:", error);
     });
   ```
   
   **Արդյունք:**
   
   ```plaintext
   Post Title: sunt aut facere repellat provident occaecati excepturi optio reprehenderit
   User Name: Leanne Graham
   ```

   ---
   
   #### Խուսափել Callback Hell-ից
   
   Promise Chaining-ը ավելի ընթեռնելի է դարձնում կոդը՝ համեմատած callback-ների հետ։
   
   #### Callback Hell
   
   ```javascript
   setTimeout(() => {
     console.log("Step 1");
     setTimeout(() => {
       console.log("Step 2");
       setTimeout(() => {
         console.log("Step 3");
       }, 1000);
     }, 1000);
   }, 1000);
   ```
   
   #### Promise Chaining
   
   ```javascript
   new Promise((resolve) => {
     setTimeout(() => resolve("Step 1"), 1000);
   })
     .then((result) => {
       console.log(result);
       return new Promise((resolve) => setTimeout(() => resolve("Step 2"), 1000));
     })
     .then((result) => {
       console.log(result);
       return new Promise((resolve) => setTimeout(() => resolve("Step 3"), 1000));
     })
     .then((result) => {
       console.log(result);
     });
   ```

   ---
   
   #### Կարգավիճակների (States) Ճշգրտում
   
   Promise-ների տարբեր կարգավիճակներն են՝
   
   1. **Pending:** Սկզբնական վիճակ, երբ Promise-ը դեռ չի կատարվել կամ մերժվել։
   2. **Fulfilled:** Promise-ը կատարվել է և վերադարձրել արդյունք։
   3. **Rejected:** Promise-ը մերժվել է և վերադարձրել սխալ։
   
   Promise Chaining-ը աշխատում է հենց այս կարգավիճակների հիման վրա՝ փոխանցելով արդյունքը կամ սխալը հաջորդ քայլին։

   ---
**[⬆ Back to Top](#բովանդակություն)**

   ---

42. ### Ինչ է Microtasks-ը JavaScript-ում?
   
   **Microtasks**-ը JavaScript-ում ասինխրոն գործողությունների տեսակ է, որոնք ունեն ավելի բարձր առաջնահերթություն, քան սովորական **tasks**-երը (օրինակ՝ `setTimeout` կամ `setInterval`)։ Microtasks-ը կատարվում են **Event Loop**-ի ընթացքում անմիջապես այն պահին, երբ Call Stack-ը դառնում է դատարկ, բայց առաջ այն tasks-ից, որոնք գտնվում են Task Queue-ում։
   
   Microtasks-ը ստեղծվում են հիմնականում հետևյալ գործողություններից՝
   
   1. **Promises** (օր.`.then`, `.catch`, `.finally`)
   2. **MutationObserver**
   3. **queueMicrotask()**
   
   ---
   
   #### Ինչպես է աշխատում Microtasks Queue-ը
   
   Microtasks-ը պահվում են **Microtask Queue**-ում։ Երբ Call Stack-ը դատարկվում է, Event Loop-ը ստուգում է Microtask Queue-ը և կատարում այնտեղ գտնվող բոլոր Microtasks-երը՝ նախքան Task Queue-ի գործողություններին անցնելը։

   ---
   
   #### Օրինակ՝ Microtasks-ի օգտագործում
   
   #### Օրինակ՝ Promise
   
   ```javascript
   console.log("Start");
   
   Promise.resolve().then(() => {
     console.log("Microtask 1");
   }).then(() => {
     console.log("Microtask 2");
   });
   
   console.log("End");
   ```
   
   **Արդյունք:**
   
   ```plaintext
   Start
   End
   Microtask 1
   Microtask 2
   ```
   
   **Բացատրություն:**
   1. "Start"-ը և "End"-ը կատարվում են անմիջապես, քանի որ դրանք սինխրոն գործողություններ են։
   2. Promise-ի `.then()` callback-ները դառնում են Microtasks և կատարվում են Call Stack-ի դատարկվելուց հետո։
   
   ---
   
   #### Task vs Microtask
   
   #### Հիմնական տարբերությունները
   
   | **Հատկանիշ**              | **Task** (օր.`setTimeout`)            | **Microtask** (օր.`Promise.then`)       |
   |---------------------------|---------------------------------------|----------------------------------------|
   | **Queue**                 | Task Queue                           | Microtask Queue                        |
   | **Առաջնահերթություն**      | Կատարվում է հետո                     | Կատարվում է անմիջապես                  |
   | **Օգտագործման դեպքեր**     | setTimeout, setInterval              | Promise, MutationObserver, queueMicrotask |
   
   #### Օրինակ՝ Task vs Microtask
   
   ```javascript
   console.log("Start");
   
   setTimeout(() => {
     console.log("Task");
   }, 0);
   
   Promise.resolve().then(() => {
     console.log("Microtask");
   });
   
   console.log("End");
   ```
   
   **Արդյունք:**
   
   ```plaintext
   Start
   End
   Microtask
   Task
   ```
   
   **Բացատրություն:**
   - Promise-ի `.then()` callback-ը (Microtask) կատարվում է Task Queue-ի առաջ, նույնիսկ եթե Task-ը ունի 0 միլիվայրկյան սպասում։
   
   ---
   
   #### queueMicrotask()
   
   `queueMicrotask`-ը մեթոդ է, որը թույլ է տալիս ձեռքով ավելացնել Microtask Queue-ում նոր callback։
   
   #### Օրինակ
   
   ```javascript
   console.log("Start");
   
   queueMicrotask(() => {
     console.log("Microtask");
   });
   
   console.log("End");
   ```
   
   **Արդյունք:**
   
   ```plaintext
   Start
   End
   Microtask
   ```
   
   **Բացատրություն:**
   - `queueMicrotask`-ի callback-ը կատարվում է Call Stack-ի դատարկվելուց հետո՝ Task Queue-ի առաջ։
   
   ---
   
   #### Օգտագործման դեպքեր
   
   1. **Promises-ի կառավարում:**
      - Ապահովում է ավելի բարձր առաջնահերթությամբ callback-ների կատարումը։
   
   2. **DOM փոփոխությունների հետևում:**
      - `MutationObserver`-ի միջոցով հնարավոր է հետևել DOM-ի փոփոխություններին Microtask Queue-ի միջոցով։
   
   3. **Մանր բեռնավորված գործողություններ:**
      - Երբ անհրաժեշտ է իրականացնել շատ փոքր գործողություն, որը պետք է կատարվի անմիջապես, առանց սպասելու Task Queue-ի հերթին։
   
   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

43. ### Ինչ է Callback Hell-ը և ինչպես կարող ենք այն խուսափել?

   
   **Callback Hell**-ը JavaScript-ում խնդիր է, որը առաջանում է, երբ callback-ները (ֆունկցիաներ, որոնք փոխանցվում են որպես պարամետր) ներդրված են մեկից ավելի մակարդակներով։ Սա կարող է կոդը դարձնել բարդ, դժվար ընթեռնելի և կառավարելի։
   
   Callback Hell-ը հաճախ հանդիպում է, երբ աշխատում ենք ասինխրոն գործողությունների հետ, օրինակ՝ **setTimeout**, **XHR** կամ **fs** մոդուլի ֆունկցիաներ։

   ---
   
   #### Օրինակ՝ Callback Hell
   
   ```javascript
   setTimeout(() => {
     console.log("Step 1");
     setTimeout(() => {
       console.log("Step 2");
       setTimeout(() => {
         console.log("Step 3");
         setTimeout(() => {
           console.log("Step 4");
         }, 1000);
       }, 1000);
     }, 1000);
   }, 1000);
   ```
   
   #### Խնդիր
   - Կոդը դառնում է "սանդղաձև" և դժվար է ընթերցվում։
   - Դժվար է ավելացնել կամ փոփոխել որևէ մակարդակ։
   - Կոդը դառնում է անկայուն՝ սխալների կառավարման բարդության պատճառով։

   ---
   
   #### Ինչպես խուսափել Callback Hell-ից
   
   #### 1. Օգտագործեք Named Functions
   Instead of inline callback functions, define and use named functions.
   
   ```javascript
   function step1() {
     console.log("Step 1");
     setTimeout(step2, 1000);
   }
   
   function step2() {
     console.log("Step 2");
     setTimeout(step3, 1000);
   }
   
   function step3() {
     console.log("Step 3");
     setTimeout(step4, 1000);
   }
   
   function step4() {
     console.log("Step 4");
   }
   
   setTimeout(step1, 1000);
   ```
   
   #### Առավելություններ
   - Կոդը դառնում է ավելի հստակ և ընթեռնելի։
   - Հեշտ է փոփոխել կամ վերահսկել որոշակի քայլեր։
   
   ---
   
   #### 2. Օգտագործեք Promises
   **Promises**-ը JavaScript-ում ներդրվել է, որպեսզի կառավարի callback-ների բարդությունը։ Promises-ը թույլ է տալիս գրել կոդ, որը մաքուր է և կանխատեսելի։
   
   ```javascript
   const step1 = () => {
     return new Promise((resolve) => {
       setTimeout(() => {
         console.log("Step 1");
         resolve();
       }, 1000);
     });
   };
   
   const step2 = () => {
     return new Promise((resolve) => {
       setTimeout(() => {
         console.log("Step 2");
         resolve();
       }, 1000);
     });
   };
   
   const step3 = () => {
     return new Promise((resolve) => {
       setTimeout(() => {
         console.log("Step 3");
         resolve();
       }, 1000);
     });
   };
   
   step1()
     .then(step2)
     .then(step3)
     .then(() => {
       console.log("Step 4");
     });
   ```
   
   #### Առավելություններ
   - Կոդը դառնում է ավելի մաքուր և ընթեռնելի։
   - Ապահովում է սխալների կառավարում `catch()`-ի միջոցով։
   
   ---
   
   #### 3. Օգտագործեք Async/Await
   **Async/Await**-ը ES8-ում ներդրված սինտաքս է, որը դարձնում է Promise-ի հետ աշխատելը ավելի հեշտ։
   
   ```javascript
   const step = (message) => {
     return new Promise((resolve) => {
       setTimeout(() => {
         console.log(message);
         resolve();
       }, 1000);
     });
   };
   
   const runSteps = async () => {
     await step("Step 1");
     await step("Step 2");
     await step("Step 3");
     console.log("Step 4");
   };
   
   runSteps();
   ```
   
   #### Առավելություններ
   - Կոդը ընթեռնելի է, ինչպես սինխրոն կոդը։
   - Ավելի հեշտ է կառավարել բարդ ասինխրոն գործողությունները։

   ---
   
   #### Եզրակացություն
   
   **Callback Hell**-ը JavaScript-ում բարդացնում է կոդի ընթերցելիությունը և կառավարման գործընթացը, բայց կարելի է խուսափել հետևյալ միջոցներով՝
   
   1. Օգտագործեք **Named Functions**՝ պարզեցնելու ներդրված callback-ները։
   2. Օգտագործեք **Promises**՝ callback-ների փոխարեն։
   3. Օգտագործեք **Async/Await**՝ Promise-ի հետ աշխատելու համար ավելի ընթերցելի սինտաքսով։

---

**[⬆ Back to Top](#բովանդակություն)**

---

44. ### Ինչ տարբերություն կա setTimeout, setInterval և requestAnimationFrame միջև?
   
   JavaScript-ը ապահովում է մի քանի մեթոդներ՝ ասինխրոն ժամանակի վրա հիմնված գործողություններ կատարելու համար։ Դրանցից են՝ **setTimeout**, **setInterval** և **requestAnimationFrame**։ Յուրաքանչյուր մեթոդ ունի իր կիրառման դեպքերը և տարբերությունները։
   
   ---
   
   #### 1. **setTimeout**
   
   #### Նկարագրություն
   **setTimeout**-ը օգտագործվում է միանգամյա գործողություն կատարելու համար որոշակի ժամանակային հետաձգումով։
   
   #### Սինտաքս
   ```javascript
   setTimeout(callback, delay, ...args);
   ```
   - `callback`: ֆունկցիան, որը պետք է կատարվի։
   - `delay`: ժամանակի հետաձգումը միլիվայրկյաններով։
   - `args`: պարամետրեր, որոնք կփոխանցվեն callback ֆունկցիային։
   
   #### Օրինակ
   ```javascript
   setTimeout(() => {
     console.log("Executed after 2 seconds");
   }, 2000);
   ```
   
   #### Հատկանիշներ
   - Կատարվում է միայն մեկ անգամ՝ նշված ժամանակից հետո։
   - Հարմար է ասինխրոն գործողություններ թեստավորելու համար։
   
   ---
   
   ### 2. **setInterval**
   
   #### Նկարագրություն
   **setInterval**-ը օգտագործվում է պարբերական գործողություններ կատարելու համար՝ նշված ժամանակահատվածով։
   
   #### Սինտաքս
   ```javascript
   setInterval(callback, delay, ...args);
   ```
   - `callback`: ֆունկցիան, որը պետք է կատարվի։
   - `delay`: ժամանակի ինտերվալը միլիվայրկյաններով։
   - `args`: պարամետրեր, որոնք կփոխանցվեն callback ֆունկցիային։
   
   #### Օրինակ
   ```javascript
   setInterval(() => {
     console.log("Executed every 1 second");
   }, 1000);
   ```
   
   #### Հատկանիշներ
   - Կատարվում է բազմիցս՝ ամեն անգամ նշված ինտերվալից հետո։
   - Կատարումը շարունակվում է մինչև այն չդադարեցվի `clearInterval()`-ի միջոցով։
   
   #### Դադարեցում
   ```javascript
   const intervalId = setInterval(() => {
     console.log("Running...");
   }, 1000);
   
   setTimeout(() => {
     clearInterval(intervalId);
     console.log("Interval cleared");
   }, 5000);
   ```

   ---
   
   #### 3. **requestAnimationFrame**
   
   #### Նկարագրություն
   **requestAnimationFrame**-ը օգտագործվում է վիզուալ անիմացիաներ ստեղծելու համար։ Այն հարմարեցված է բրաուզերի վերաանկարչման արագությանը և ապահովում է ավելի սահուն անիմացիա։
   
   #### Սինտաքս
   ```javascript
   requestAnimationFrame(callback);
   ```
   - `callback`: ֆունկցիան, որը պետք է կատարվի հաջորդ frame-ի ընթացքում։
   
   #### Օրինակ
   ```javascript
   let start = null;
   function animate(timestamp) {
     if (!start) start = timestamp;
     const progress = timestamp - start;
     console.log(`Progress: ${progress}ms`);
   
     if (progress < 2000) {
       requestAnimationFrame(animate);
     }
   }
   
   requestAnimationFrame(animate);
   ```
   
   #### Հատկանիշներ
   - Հարմար է FPS-ի (Frames Per Second) վերահսկման համար։
   - Ավտոմատ դադարում է աշխատել, երբ էջը թաքնված է (visibility change), ինչը օգնում է նվազեցնել էներգիայի օգտագործումը։

   ---
   
   #### Տարբերությունները
   
   | **Հատկանիշ**                | **setTimeout**                   | **setInterval**                  | **requestAnimationFrame**         |
   |-----------------------------|----------------------------------|----------------------------------|----------------------------------|
   | **Օգտագործման նպատակ**       | Միանգամյա գործողություն           | Պարբերական գործողություն          | Վիզուալ անիմացիաներ               |
   | **Հաճախականություն**         | Միայն մեկ անգամ                 | Ամեն անգամ ինտերվալից հետո       | Հարմարեցվում է բրաուզերի FPS-ին     |
   | **Կառավարման մեթոդ**         | clearTimeout()                  | clearInterval()                 | cancelAnimationFrame()            |
   | **Էներգիայի արդյունավետություն** | Չի վերահսկվում                   | Չի վերահսկվում                   | Ավելի արդյունավետ                  |
   | **Ժամանակի ճշտություն**      | Կախված է բրաուզերից              | Կախված է բրաուզերից              | Ապահովում է ավելի սահուն փորձ       |

   ---
   
   #### Եզրակացություն
   
   - Օգտագործեք **setTimeout**, երբ անհրաժեշտ է գործողություն կատարել միայն մեկ անգամ՝ որոշակի ժամանակից հետո։
   - Օգտագործեք **setInterval**, երբ անհրաժեշտ է պարբերական գործողություններ կատարել՝ առանց բարդության։
   - Օգտագործեք **requestAnimationFrame**, երբ աշխատում եք անիմացիաների կամ վիզուալ թարմացումների հետ, քանի որ այն ապահովում է ավելի սահուն աշխատանք և ավելի լավ կատարում։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

45. ### Ինչ է Service Worker-ը JavaScript-ում?

   **Service Worker**-ը JavaScript-ում ֆոնային սցենար է, որը թույլ է տալիս վեբ ծրագրերին աշխատել առանց ինտերնետի կամ ցածր ցանցային կապի պայմաններում։ Այն հիմնականում օգտագործվում է Progressive Web App (PWA)-ներում՝ աջակցելով քեշավորման, ֆոնային համաժամացման և push ծանուցումների։
   
   Service Worker-ը աշխատում է առանձին թելի վրա (thread) և չունի անմիջական մուտք դեպի DOM։

   ---
   
   #### Հիմնական Հատկանիշներ
   
   1. **Ֆոնային գործընթաց:**
      - Աշխատում է վեբ էջից անկախ և շարունակվում է նույնիսկ այն դեպքում, երբ էջը փակված է։
   
   2. **Քեշավորում (Caching):**
      - Օգտագործվում է ռեսուրսների տեղական պահեստավորման համար, ինչը թույլ է տալիս ծրագրին աշխատել offline ռեժիմում։
   
   3. **Ծանուցումներ (Push Notifications):**
      - Աջակցում է push ծանուցումների, որոնք օգտատերերին կարող են տեղեկացնել առանց կայքը բացելու։
   
   4. **Ֆոնային համաժամացում (Background Sync):**
      - Հնարավորություն է տալիս տվյալների համաժամացում կատարել, երբ ցանցային կապը վերականգնվում է։

   ---
   
   #### Ինչպես է աշխատում Service Worker-ը
   
   Service Worker-ը անցնում է երեք հիմնական փուլով՝
   
   1. **Տեղադրում (Install):**
      - Service Worker-ը սկզբում գրանցվում է և կատարվում է նրա setup-ը։
   
   2. **Ակտիվացում (Activate):**
      - Service Worker-ը ակտիվանում է և սկսում վերահսկել կայքը։
   
   3. **Միջամտություն (Fetch Events):**
      - Service Worker-ը սկսում է միջամտել ցանցային հարցումներին և կառավարում ռեսուրսները։

   ---
   
   #### Service Worker-ի Օրինակ
   
   #### 1. Գրանցում
   
   ```javascript
   if ('serviceWorker' in navigator) {
     navigator.serviceWorker.register('/service-worker.js')
       .then(registration => {
         console.log('Service Worker registered with scope:', registration.scope);
       })
       .catch(error => {
         console.error('Service Worker registration failed:', error);
       });
   }
   ```
   
   #### 2. Service Worker Ֆայլ
   
   ```javascript
   self.addEventListener('install', event => {
     console.log('Service Worker installing...');
   
     event.waitUntil(
       caches.open('v1').then(cache => {
         return cache.addAll([
           '/',
           '/index.html',
           '/styles.css',
           '/script.js'
         ]);
       })
     );
   });
   
   self.addEventListener('activate', event => {
     console.log('Service Worker activated.');
   });
   
   self.addEventListener('fetch', event => {
     event.respondWith(
       caches.match(event.request).then(response => {
         return response || fetch(event.request);
       })
     );
   });
   ```

   ---
   
   #### Service Worker-ի Հիմնական Միջոցառումներ
   
   1. **install:**
      - Գործարկվում է, երբ Service Worker-ը գրանցվում է։ Հիմնականում օգտագործվում է ռեսուրսների քեշավորման համար։
   
   2. **activate:**
      - Գործարկվում է, երբ Service Worker-ը ակտիվանում է և սկսում վերահսկել էջը։
   
   3. **fetch:**
      - Միջամտում է ցանցային հարցումներին։ Կարող է վերադարձնել տեղական քեշից կամ ցանցից ստացված պատասխան։
   
   4. **message:**
      - Օգտագործվում է էջի և Service Worker-ի միջև հաղորդակցության համար։

   ---
   
   #### Արժեքները և Թերությունները
   
   #### Արժեքներ
   - **Offline աջակցություն:**
      - Ծրագիրը կարող է աշխատել առանց ինտերնետի։
   
   - **Ցանցային տրաֆիկի օպտիմալացում:**
      - Քեշավորման միջոցով նվազեցնում է ցանցային հարցումները։
   
   - **Արագություն:**
      - Քեշից ռեսուրսները բեռնումը ավելի արագ է, քան ցանցից։
   
   #### Թերություններ
   - **Բարդություն:**
      - Ծրագրավորողներից պահանջում է լրացուցիչ գիտելիքներ Service Worker-ի աշխատանքի մասին։
   
   - **Սկզբնական բեռնում:**
      - Առաջին բեռնումը կարող է ավելի երկար տևել՝ ռեսուրսների քեշավորման պատճառով։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---


46. ### Ինչ տարբեր եղանակներ կան զանգվածի վրայով անցնելու համար JavaScript-ում?

   JavaScript-ում զանգվածի (array) տարրերի միջոցով անցնելու համար կան բազմաթիվ եղանակներ։ Յուրաքանչյուր մեթոդ ունի իր կիրառման դեպքերը և տարբերությունները։

   ---
   
   #### 1. **for Լուփ**
   
   #### Նկարագրություն
   Հիմնական ցիկլ, որը թույլ է տալիս անցնել զանգվածի տարրերի միջոցով ըստ ինդեքսի։
   
   #### Օրինակ
   ```javascript
   const array = [1, 2, 3, 4, 5];
   
   for (let i = 0; i < array.length; i++) {
     console.log(array[i]);
   }
   ```
   
   #### Առավելություններ
   - Կառավարման լրիվություն (մուտք դեպի ինդեքս, պայմաններ փոփոխելու հնարավորություն)։
   
   #### Թերություններ
   - Կոդը կարող է դառնալ ավելի քիչ ընթեռնելի՝ երկար սինտաքսի պատճառով։
   
   ---
   
   #### 2. **for...of Լուփ**
   
   #### Նկարագրություն
   Հեշտ ընթեռնելի ցիկլ, որը թույլ է տալիս անցնել զանգվածի տարրերի միջոցով առանց ինդեքսի։
   
   #### Օրինակ
   ```javascript
   const array = [1, 2, 3, 4, 5];
   
   for (const value of array) {
     console.log(value);
   }
   ```
   
   #### Առավելություններ
   - Ավելի կարճ և ընթեռնելի։
   - Հարմար է, երբ անհրաժեշտ չէ ինդեքսի հասանելիություն։
   
   #### Թերություններ
   - Չի տրամադրում մուտք ինդեքսին։

   ---
   
   #### 3. **forEach() Մեթոդ**
   
   #### Նկարագրություն
   `forEach()`-ը զանգվածի մեթոդ է, որը կարճ ձև է ապահովում տարրերի վրա գործելու համար։
   
   #### Օրինակ
   ```javascript
   const array = [1, 2, 3, 4, 5];
   
   array.forEach((value, index) => {
     console.log(`Index: ${index}, Value: ${value}`);
   });
   ```
   
   #### Առավելություններ
   - Կոդը կարճ և պարզ է։
   - Ներառում է callback ֆունկցիա՝ մուտք դեպի արժեքը և ինդեքսը։
   
   #### Թերություններ
   - Չի վերադարձնում նոր զանգված։
   - Չի աշխատում `break` կամ `continue`։
   
   ---
   
   #### 4. **map() Մեթոդ**
   
   #### Նկարագրություն
   `map()`-ը ստեղծում է նոր զանգված՝ կիրառելով callback ֆունկցիան յուրաքանչյուր տարրի վրա։
   
   #### Օրինակ
   ```javascript
   const array = [1, 2, 3, 4, 5];
   
   const squared = array.map(value => value * value);
   console.log(squared); // [1, 4, 9, 16, 25]
   ```
   
   #### Առավելություններ
   - Վերադարձնում է նոր զանգված։
   - Օգտագործվում է տվյալների փոփոխման համար։
   
   #### Թերություններ
   - Չի փոփոխում սկզբնական զանգվածը։
   
   ---
   
   #### 5. **filter() Մեթոդ**
   
   #### Նկարագրություն
   `filter()`-ը ստեղծում է նոր զանգված, որը պարունակում է միայն այն տարրերը, որոնք բավարարում են որոշակի պայման։
   
   #### Օրինակ
   ```javascript
   const array = [1, 2, 3, 4, 5];
   
   const evenNumbers = array.filter(value => value % 2 === 0);
   console.log(evenNumbers); // [2, 4]
   ```
   
   #### Առավելություններ
   - Վերադարձնում է նոր զանգված միայն ընտրված տարրերով։
   
   #### Թերություններ
   - Տրամադրում է միայն ֆիլտրացիա, ոչ փոփոխություն։
   
   ---
   
   #### 6. **reduce() Մեթոդ**
   
   #### Նկարագրություն
   `reduce()`-ը հաշվարկում է մի արժեք՝ կիրառելով callback ֆունկցիան տարրերի վրա։
   
   #### Օրինակ
   ```javascript
   const array = [1, 2, 3, 4, 5];
   
   const sum = array.reduce((accumulator, value) => accumulator + value, 0);
   console.log(sum); // 15
   ```
   
   #### Առավելություններ
   - Հարմար է կուտակային հաշվարկների համար։
   
   #### Թերություններ
   - Ավելի բարդ է սկսնակների համար։
   
   ---
   
   #### 7. **while Լուփ**
   
   #### Նկարագրություն
   Ցիկլ, որը կատարվում է մինչև որոշակի պայմանը դառնում է կեղծ։
   
   #### Օրինակ
   ```javascript
   const array = [1, 2, 3, 4, 5];
   let i = 0;
   
   while (i < array.length) {
     console.log(array[i]);
     i++;
   }
   ```
   
   #### Առավելություններ
   - Կատարումը լիովին վերահսկելի է։
   
   #### Թերություններ
   - Կարող է հանգեցնել անվերջ ցիկլի։
   
   ---
   
   #### 8. **do...while Լուփ**
   
   #### Նկարագրություն
   Ցիկլ, որը կատարվում է առնվազն մեկ անգամ՝ մինչև պայմանը կդառնա կեղծ։
   
   #### Օրինակ
   ```javascript
   const array = [1, 2, 3, 4, 5];
   let i = 0;
   
   do {
     console.log(array[i]);
     i++;
   } while (i < array.length);
   ```
   
   #### Առավելություններ
   - Համոզված է, որ կկատարվի առնվազն մեկ անգամ։
   
   #### Թերություններ
   - Կարող է հանգեցնել անվերջ ցիկլի, եթե սխալ ձևավորվի։
   
   ---
   
   #### Եզրակացություն
   
   JavaScript-ում զանգվածների միջոցով անցնելու բազմաթիվ մեթոդներ թույլ են տալիս ընտրել համապատասխան լուծումը՝ կախված ծրագրի պահանջներից։
   
   - **for** և **while** ցիկլերը ապահովում են մեծ ճկունություն։
   - **forEach**, **map**, և **filter** մեթոդները ավելի հարմար են ֆունկցիոնալ ծրագրավորման համար։
   - **reduce**-ը հզոր գործիք է տվյալների հաշվարկների համար։
   
   Ուղղակի ընտրեք մեթոդը՝ հիմնվելով նախագծի պահանջների և կոդի ընթեռնելիության վրա։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---


47. ### Ինչ է Web Storage-ը (localStorage և sessionStorage)?

   **Web Storage**-ը API է, որը թույլ է տալիս վեբ ծրագրերին տվյալներ պահպանել բրաուզերում։ Այն ապահովում է տվյալների պահեստավորում առանց սերվերի, օգտագործվում է տվյալների արագ մուտքագրման և բրաուզերի մեջ օգտատիրոջ հատուկ պարամետրերի պահպանման համար։ Web Storage-ը ներառում է երկու հիմնական տեսակ՝
   
   1. **localStorage**
   2. **sessionStorage**
   
   ---
   
   #### Հիմնական Հատկանիշներ
   
   | **Հատկանիշ**             | **localStorage**                                      | **sessionStorage**                                     |
   |--------------------------|-----------------------------------------------------|-----------------------------------------------------|
   | **Տվյալների պահպանման տևողություն** | Պահպանվում են մինչև ձեռքով հեռացվի։                  | Պահպանվում են մինչև բրաուզերի ներդիրը փակվի։         |
   | **Հասանելիություն**        | Հասանելի է նույն տիրույթի բոլոր էջերից։               | Հասանելի է միայն այն ներդիրից, որտեղ ստեղծվել է։    |
   | **Հիշողության սահմանափակում** | Մոտավորապես 5MB (կախված բրաուզերից)։               | Մոտավորապես 5MB (կախված բրաուզերից)։               |
   | **API մեթոդներ**          | `setItem`, `getItem`, `removeItem`, `clear`, `key` | Նույնը՝ ինչպես localStorage-ի դեպքում։             |
   
   ---
   
   #### localStorage
   
   #### Նկարագրություն
   **localStorage**-ը թույլ է տալիս տվյալների պահպանումը, որոնք հասանելի են մինչև դրանք մաքրվեն ձեռքով կամ ծրագրի միջոցով։
   
   #### Օրինակներ
   
   #### Տվյալների պահպանում
   ```javascript
   // Տվյալների ավելացում
   localStorage.setItem('username', 'JohnDoe');
   
   // Տվյալների ընթերցում
   const username = localStorage.getItem('username');
   console.log(username); // "JohnDoe"
   
   // Տվյալների հեռացում
   localStorage.removeItem('username');
   
   // Բոլոր տվյալների մաքրում
   localStorage.clear();
   ```
   
   #### Քանի՞ բանալի է պահվում
   ```javascript
   console.log(localStorage.length); // Պահված բանալիների քանակը
   ```

   ---
   
   #### sessionStorage
   
   #### Նկարագրություն
   **sessionStorage**-ը թույլ է տալիս տվյալների պահպանում բրաուզերի ներդիրի (tab) շրջանակներում։ Երբ ներդիրը փակվում է, տվյալները կորում են։
   
   #### Օրինակներ
   
   #### Տվյալների պահպանում
   ```javascript
   // Տվյալների ավելացում
   sessionStorage.setItem('sessionId', '12345');
   
   // Տվյալների ընթերցում
   const sessionId = sessionStorage.getItem('sessionId');
   console.log(sessionId); // "12345"
   
   // Տվյալների հեռացում
   sessionStorage.removeItem('sessionId');
   
   // Բոլոր տվյալների մաքրում
   sessionStorage.clear();
   ```

   ---
   
   #### Web Storage-ի Մեթոդներ
   
   | **Մեթոդ**             | **Նկարագրություն**                                                                      |
   |------------------------|---------------------------------------------------------------------------------------|
   | `setItem(key, value)`  | Պահպանում է նոր բանալի-արժեք զույգ։                                                  |
   | `getItem(key)`         | Վերադարձնում է բանալու արժեքը։                                                        |
   | `removeItem(key)`      | Հեռացնում է տվյալ բանալու արժեքը։                                                     |
   | `clear()`              | Մաքրում է բոլոր պահված տվյալները։                                                    |
   | `key(index)`           | Վերադարձնում է բանալու անունը՝ ըստ տրված ինդեքսի։                                     |

   ---
   
   #### Web Storage-ի Առավելություններ
   
   1. **Արագություն:**
      - Տվյալները պահվում են տեղական բրաուզերում, ինչը ավելի արագ է, քան սերվերի վրա դիմելը։
   
   2. **Կառավարման պարզություն:**
      - Պարզ API մեթոդներ, որոնք հեշտ են օգտագործման համար։
   
   3. **Կապի պահանջ չլինելը:**
      - Տվյալները հասանելի են նույնիսկ ցանցային կապի բացակայության դեպքում։
   
   4. **Համեմատաբար մեծ պահեստավորման ծավալ:**
      - Մոտ 5MB բրաուզերների մեծ մասում։

   ---
   
   #### Web Storage-ի Թերություններ
   
   1. **Անվտանգություն:**
      - Տվյալները պահպանվում են անկոդավորված։ Չպետք է պահել զգայուն տվյալներ։
   
   2. **Սահմանափակ տիրույթ:**
      - Տվյալները հասանելի են միայն նույն տիրույթից։
   
   3. **Ներդիրների միջև անհամաձայնություն (sessionStorage):**
      - sessionStorage-ի տվյալները հասանելի չեն այլ ներդիրներում։

   ---
   
   #### Եզրակացություն
   
   **localStorage** և **sessionStorage** API-ները հզոր գործիքներ են, որոնք թույլ են տալիս տվյալների պահպանման պարզ և արագ միջոց վեբ ծրագրերում։
   
   - **localStorage**-ը հարմար է երկարաժամկետ տվյալների պահպանման համար։
   - **sessionStorage**-ը հարմար է կարճաժամկետ, session-ի շրջանակներում գործող տվյալների համար։
   
   Հաշվի առեք անվտանգության նկատառումները և օգտագործեք Web Storage-ը տվյալների պահպանման համար, որոնք չեն պարունակում զգայուն տեղեկատվություն։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

48. ### Ինչ է Proxy-ը և Reflect-ը JavaScript-ում?
   
   **Proxy**-ը JavaScript-ում օգտագործվում է օբյեկտների վրա միջամտելու կամ փոփոխելու գործողությունները։ Այն թույլ է տալիս կառավարել օբյեկտների որոշակի գործողություններ, օրինակ՝ հատկությունների մուտքագրում, փոփոխում կամ հեռացում։ Proxy-ները աշխատում են որպես "դահիճ" օբյեկտների և դրանց արտաքին մուտքերի միջև։

   ---
   
   #### Սինտաքս
   ```javascript
   const proxy = new Proxy(target, handler);
   ```
   - **`target`**: Օբյեկտը, որը Proxy-ն պետք է վերահսկի։
   - **`handler`**: Օբյեկտ, որը պարունակում է մեթոդներ՝ գործողությունները վերահսկելու համար։
   
   ---
   
   #### Օրինակներ
   
   #### Հատկության ընթերցում (get)
   ```javascript
   const target = {
     name: "Alice"
   };
   
   const handler = {
     get: (obj, prop) => {
       return prop in obj ? obj[prop] : `Property ${prop} does not exist.`;
     }
   };
   
   const proxy = new Proxy(target, handler);
   
   console.log(proxy.name); // "Alice"
   console.log(proxy.age);  // "Property age does not exist."
   ```
   
   #### Հատկության փոփոխում (set)
   ```javascript
   const target = {
     age: 25
   };
   
   const handler = {
     set: (obj, prop, value) => {
       if (prop === "age" && typeof value !== "number") {
         throw new Error("Age must be a number.");
       }
       obj[prop] = value;
       return true;
     }
   };
   
   const proxy = new Proxy(target, handler);
   
   proxy.age = 30; // OK
   console.log(proxy.age); // 30
   
   proxy.age = "thirty"; // Error: Age must be a number.
   ```
   
   #### Հատկության ջնջում (deleteProperty)
   ```javascript
   const target = {
     name: "Alice"
   };
   
   const handler = {
     deleteProperty: (obj, prop) => {
       if (prop === "name") {
         throw new Error("Cannot delete name property.");
       }
       delete obj[prop];
       return true;
     }
   };
   
   const proxy = new Proxy(target, handler);
   
   delete proxy.name; // Error: Cannot delete name property.
   ```

   ---
   
   #### Handler-ի մեթոդներ
   Proxy-ի **handler** օբյեկտը ներառում է բազմաթիվ մեթոդներ, որոնք կարելի է օգտագործել՝ օբյեկտի գործողությունները վերահսկելու համար։
   
   | **Մեթոդ**               | **Նկարագրություն**                                              |
   |--------------------------|-----------------------------------------------------------------|
   | `get`                   | Կոչվում է, երբ հատկությունը ընթերցվում է։                       |
   | `set`                   | Կոչվում է, երբ հատկությունը փոփոխվում է։                       |
   | `deleteProperty`        | Կոչվում է, երբ հատկությունը ջնջվում է։                          |
   | `has`                   | Կոչվում է, երբ ստուգվում է, թե հատկությունը առկա է օբյեկտում։   |
   | `apply`                 | Կոչվում է, երբ Proxy-ն գործարկվում է որպես ֆունկցիա։            |
   | `construct`             | Կոչվում է, երբ Proxy-ն գործարկվում է որպես կոնստրուկտոր։        |

   ---
   
   #### Reflect
   
   #### Նկարագրություն
   **Reflect**-ը JavaScript-ում ներկառուցված օբյեկտ է, որը ապահովում է մեթոդներ օբյեկտների վրա գործողություններ կատարելու համար։ Reflect-ը նախատեսված է Proxy-ի հետ աշխատելու և նրա կողմից իրականացվող գործողությունները պարզեցնելու համար։

   ---
   
   #### Հիմնական Մեթոդներ
   Reflect-ը պարունակում է նույն մեթոդները, որոնք կարող են օգտագործվել Proxy-ում։
   
   | **Մեթոդ**               | **Նկարագրություն**                                              |
   |--------------------------|-----------------------------------------------------------------|
   | `Reflect.get`           | Վերադարձնում է օբյեկտի հատկության արժեքը։                      |
   | `Reflect.set`           | Սահմանում է օբյեկտի հատկության արժեքը։                        |
   | `Reflect.deleteProperty`| Ջնջում է օբյեկտի հատկությունը։                                 |
   | `Reflect.has`           | Ստուգում է, թե հատկությունը առկա է օբյեկտում։                 |
   | `Reflect.apply`         | Կիրառում է ֆունկցիան որոշակի this-ի և պարամետրերի վրա։         |
   | `Reflect.construct`     | Օգտագործվում է նոր օբյեկտ ստեղծելու համար։                     |

   ---
   
   #### Օրինակներ
   
   #### Reflect.get և Reflect.set
   ```javascript
   const target = {
     name: "Alice",
     age: 25
   };
   
   console.log(Reflect.get(target, "name")); // "Alice"
   
   Reflect.set(target, "age", 30);
   console.log(target.age); // 30
   ```
   
   #### Reflect.deleteProperty
   ```javascript
   const target = {
     name: "Alice",
     age: 25
   };
   
   Reflect.deleteProperty(target, "age");
   console.log(target); // { name: "Alice" }
   ```
   
   #### Proxy և Reflect համատեղ օգտագործում
   ```javascript
   const target = {
     name: "Alice",
     age: 25
   };
   
   const handler = {
     get: (obj, prop) => {
       console.log(`Getting property: ${prop}`);
       return Reflect.get(obj, prop);
     },
     set: (obj, prop, value) => {
       console.log(`Setting property: ${prop} to ${value}`);
       return Reflect.set(obj, prop, value);
     }
   };
   
   const proxy = new Proxy(target, handler);
   
   proxy.name; // Getting property: name
   proxy.age = 30; // Setting property: age to 30
   ```

   ---
   
   #### Proxy vs Reflect
   
   | **Հատկանիշ**              | **Proxy**                                        | **Reflect**                                    |
   |---------------------------|------------------------------------------------|-----------------------------------------------|
   | **Օգտագործման նպատակ**     | Օբյեկտների վրա գործողությունները վերահսկելու համար։ | Օբյեկտների գործողությունները իրականացնելու համար։|
   | **Կիրառման եղանակ**        | Ապահովում է վերահսկողության մեխանիզմ։             | Ապահովում է պարզ ինտերֆեյս գործողությունների համար։|
   | **API-ի տրամադրած մեթոդներ**| handler մեթոդներ                                | Օբյեկտների գործողություններ (get, set, apply, և այլն) |

   ---
   
   #### Եզրակացություն
   
   - **Proxy**-ն հզոր գործիք է, որը թույլ է տալիս վերահսկել օբյեկտների հետ կատարվող գործողությունները։
   - **Reflect**-ը ապահովում է օբյեկտների վրա գործողությունների ստանդարտացված API, որը պարզեցնում է Proxy-ի հետ աշխատելու գործընթացը։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---


49. ### Ինչ է Generators-ը JavaScript-ում?

   
   **Generators**-ը JavaScript-ում հատուկ ֆունկցիաներ են, որոնք թույլ են տալիս `function*` սինտաքսով ստեղծել ֆունկցիաներ, որոնք կարող են դադարեցվել և վերսկսվել։ Generators-ը հնարավորություն է տալիս քայլ առ քայլ արտադրել արժեքներ `yield` բանալի բառի միջոցով։

   ---
   
   #### Սինտաքս
   
   ```javascript
   function* generatorFunction() {
     yield value1;
     yield value2;
     return value3;
   }
   ```
   
   - **`function*`**: Գեներատորի ֆունկցիայի հստակ սինտաքս։
   - **`yield`**: Կանգնեցնում է ֆունկցիայի կատարումը և վերադարձնում արժեք։
   - **`return`**: Վերադարձնում է վերջնական արժեքը և դադարեցնում գեներատորի աշխատանքը։

   ---
   
   #### Գործարկում
   
   Generators-ը վերադարձնում է հատուկ օբյեկտ՝ **Iterator**, որը կարող է կառավարվել `next()` մեթոդի միջոցով։
   
   ```javascript
   const gen = generatorFunction();
   
   console.log(gen.next()); // { value: value1, done: false }
   console.log(gen.next()); // { value: value2, done: false }
   console.log(gen.next()); // { value: value3, done: true }
   ```
   
   - **`value`**: Վերադարձված արժեքը։
   - **`done`**: Ցույց է տալիս՝ արդյոք գեներատորը ավարտվել է։
   
   ---
   
   #### Օրինակներ
   
   #### 1. Հիմնական Օրինակ
   ```javascript
   function* simpleGenerator() {
     yield 1;
     yield 2;
     yield 3;
   }
   
   const gen = simpleGenerator();
   
   console.log(gen.next()); // { value: 1, done: false }
   console.log(gen.next()); // { value: 2, done: false }
   console.log(gen.next()); // { value: 3, done: false }
   console.log(gen.next()); // { value: undefined, done: true }
   ```
   
   #### 2. Անսահման Գեներատոր
   ```javascript
   function* infiniteGenerator() {
     let i = 0;
     while (true) {
       yield i++;
     }
   }
   
   const gen = infiniteGenerator();
   
   console.log(gen.next().value); // 0
   console.log(gen.next().value); // 1
   console.log(gen.next().value); // 2
   ```
   
   #### 3. Օգտագործում `for...of` ցիկլում
   Generators-ը կարելի է հեշտությամբ ինտեգրել `for...of` ցիկլի հետ։
   
   ```javascript
   function* numberGenerator() {
     yield 1;
     yield 2;
     yield 3;
   }
   
   for (const value of numberGenerator()) {
     console.log(value);
   }
   // Output: 1, 2, 3
   ```
   
   #### 4. Տվյալների Ֆիլտրման Օրինակ
   ```javascript
   function* filterGenerator(arr, predicate) {
     for (const item of arr) {
       if (predicate(item)) {
         yield item;
       }
     }
   }
   
   const gen = filterGenerator([1, 2, 3, 4, 5], x => x % 2 === 0);
   
   console.log([...gen]); // [2, 4]
   ```

   ---
   
   #### Գեներատորների Օգտագործման Դեպքեր
   
   1. **Անսահման հաջորդականություններ:**
      - Օրինակ՝ ֆիբոնաչիի հաջորդականություն կամ մեծ տվյալների հոսք։
   
   2. **Ասինխրոն կոդի կառավարում:**
      - Generators-ը կարող է օգտագործվել `async/await`-ի նախորդակեպերում՝ ասինխրոն գործողությունների կառավարում ապահովելու համար։
   
   3. **Կոմպլեքս տվյալների ընթացքի կառավարում:**
      - Օգտակար է, երբ անհրաժեշտ է տվյալների հոսքի վերահսկում (streaming data)։
   
   ---
   
   #### Generators և Iterators
   
   #### Տարբերությունը
   - **Iterators**-ը պարզ կառուցվածքներ են, որոնք օգտագործվում են տարրերի հաջորդական ստացման համար։
   - **Generators**-ը ավելի հզոր են, քանի որ կարող են `yield`-ով դադարեցնել կատարումը և պահպանել իրենց վիճակը։
   
   #### Օրինակ՝ Iterator առանց Generator
   ```javascript
   const iterator = {
     current: 0,
     next() {
       if (this.current < 3) {
         return { value: this.current++, done: false };
       }
       return { value: undefined, done: true };
     }
   };
   
   console.log(iterator.next()); // { value: 0, done: false }
   console.log(iterator.next()); // { value: 1, done: false }
   console.log(iterator.next()); // { value: 2, done: false }
   console.log(iterator.next()); // { value: undefined, done: true }
   ```
   
   #### Նույնը՝ Generator-ով
   ```javascript
   function* generator() {
     yield 0;
     yield 1;
     yield 2;
   }
   
   const gen = generator();
   
   console.log(gen.next()); // { value: 0, done: false }
   console.log(gen.next()); // { value: 1, done: false }
   console.log(gen.next()); // { value: 2, done: false }
   console.log(gen.next()); // { value: undefined, done: true }
   ```

   ---
   
   #### Generators-ի Առավելություններ
   
   1. **Արագ և պարզ սինտաքս:**
      - Ավելի հեշտ է ստեղծել և օգտագործել, քան սովորական iterator-ները։
   
   2. **Կատարումի դադարեցում և վերսկսում:**
      - Հնարավորություն է տալիս դադարեցնել և շարունակել հաշվարկները։
   
   3. **Օգտագործում մեծ տվյալների հոսքերի համար:**
      - Հարմար է բարդ և երկարատև գործողությունների համար։

   ---
   
   #### Եզրակացություն
   
   **Generators**-ը JavaScript-ում հատուկ ֆունկցիաներ են, որոնք տալիս են ճկունություն տվյալների ընթացքը կառավարելու համար։ Դրանք հեշտացնում են ասինխրոն գործողությունների կառավարումը, ստեղծում են պարզ iterators և օգտակար են մեծ տվյալների հոսքերի և բարդ հաջորդականությունների հետ աշխատելիս։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---


50. ### Ինչ է Iterables և Iterators-ը JavaScript-ում?
   
   **Iterables**-ը JavaScript-ում օբյեկտներ են, որոնք թույլ են տալիս իտերացիա (iteration)՝ այսինքն՝ տարր առ տարր անցնել իրենց պարունակությունը։ Iterable օբյեկտները պետք է պարունակեն հատուկ մեթոդ՝ **`Symbol.iterator`**, որը վերադարձնում է Iterator օբյեկտ։
   
   JavaScript-ում որոշ ներկառուցված տեսակներ, ինչպիսիք են **Arrays**, **Strings**, **Maps**, և **Sets**, արդեն համարվում են Iterables։
   
   #### Օրինակ
   ```javascript
   const array = [1, 2, 3];
   const iterator = array[Symbol.iterator]();
   
   console.log(iterator.next()); // { value: 1, done: false }
   console.log(iterator.next()); // { value: 2, done: false }
   console.log(iterator.next()); // { value: 3, done: false }
   console.log(iterator.next()); // { value: undefined, done: true }
   ```
   
   ---
   
   #### Iterators
   
   #### Նկարագրություն
   
   **Iterator**-ը օբյեկտ է, որն ապահովում է մեթոդ՝ **`next()`**, որը վերադարձնում է օբյեկտ՝ պարունակելով երկու հատկություն՝
   
   - **`value`**: Արտադրած արժեքը։
   - **`done`**: Ցույց է տալիս, թե արդյոք իտերացիան ավարտվել է (true կամ false)։
   
   #### Iterator-ի Օրինակ
   ```javascript
   const myIterator = {
     current: 0,
     last: 3,
     next() {
       if (this.current <= this.last) {
         return { value: this.current++, done: false };
       } else {
         return { value: undefined, done: true };
       }
     }
   };
   
   console.log(myIterator.next()); // { value: 0, done: false }
   console.log(myIterator.next()); // { value: 1, done: false }
   console.log(myIterator.next()); // { value: 2, done: false }
   console.log(myIterator.next()); // { value: 3, done: false }
   console.log(myIterator.next()); // { value: undefined, done: true }
   ```

   ---
   
   #### Iterables և Iterators-ի Հիմնական Հատկանիշները
   
   | **Հատկանիշ**              | **Iterables**                           | **Iterators**                         |
   |---------------------------|-----------------------------------------|---------------------------------------|
   | **Օբյեկտի տեսակ**         | Օբյեկտ, որն ունի `Symbol.iterator`։    | Օբյեկտ, որն ունի `next()` մեթոդ։     |
   | **Նպատակ**                | Տրամադրում է իտերացիայի մեխանիզմ։       | Իտերացիայի քայլերի կառավարում։        |
   | **Օգտագործում**            | Օգտագործվում է `for...of` ցիկլում։      | Օգտագործվում է ներքին գործարկման համար։ |

   ---
   
   #### Iterables-ի Օգտագործումը
   
   #### 1. **`for...of` Ցիկլ**
   
   ```javascript
   const array = [10, 20, 30];
   
   for (const value of array) {
     console.log(value);
   }
   // Output: 10, 20, 30
   ```
   
   #### 2. **`spread` օպերատոր**
   
   ```javascript
   const set = new Set([1, 2, 3]);
   
   const array = [...set];
   console.log(array); // [1, 2, 3]
   ```
   
   #### 3. **`destructuring`**
   
   ```javascript
   const [a, b, c] = 'ABC';
   console.log(a, b, c); // A B C
   ```

   ---
   
   #### Custom Iterable Օբյեկտ
   
   #### Ստեղծում սեփական Iterable
   ```javascript
   const myIterable = {
     values: [1, 2, 3],
     [Symbol.iterator]() {
       let index = 0;
       const values = this.values;
       return {
         next() {
           if (index < values.length) {
             return { value: values[index++], done: false };
           } else {
             return { value: undefined, done: true };
           }
         }
       };
     }
   };
   
   for (const value of myIterable) {
     console.log(value);
   }
   // Output: 1, 2, 3
   ```

   ---
   
   #### Iterables և Generators
   
   Generators-ը նույնպես ապահովում են Iterables-ի ֆունկցիոնալություն։
   
   #### Օրինակ՝ Generator-ի միջոցով Iterable
   ```javascript
   function* generator() {
     yield 1;
     yield 2;
     yield 3;
   }
   
   for (const value of generator()) {
     console.log(value);
   }
   // Output: 1, 2, 3
   ```

   ---
   
   #### Եզրակացություն
   
   - **Iterables**-ը JavaScript-ում հատուկ օբյեկտներ են, որոնք կարող են օգտագործվել `for...of` ցիկլի, `spread` օպերատորի և այլ մեխանիզմների հետ։
   - **Iterators**-ը հատուկ օբյեկտներ են, որոնք կառավարվում են `next()` մեթոդի միջոցով։
   - Ճկունություն ստանալու համար կարելի է ստեղծել սեփական Iterables և օգտագործել Generators՝ բարդ հոսքերի կառավարումը հեշտացնելու համար։
  
   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

51. ### Ինչ է Destructuring-ը JavaScript-ում?

   **Destructuring**-ը JavaScript-ի սինտաքս է, որը թույլ է տալիս հեշտությամբ բաժանել (extract) արժեքներ զանգվածներից կամ հատկություններ օբյեկտներից և վերագրել դրանք փոփոխականներին։
   
   Այն դարձնում է կոդը ավելի կարճ, պարզ և ընթեռնելի՝ հանելով բարդ հղումները։
   
   ---
   
   #### Զանգվածների (Array) Destructuring
   
   #### Օրինակներ
   
   #### Հիմնական Օրինակ
   ```javascript
   const numbers = [1, 2, 3];
   const [a, b, c] = numbers;
   
   console.log(a); // 1
   console.log(b); // 2
   console.log(c); // 3
   ```
   
   #### Արժեքների բաց թողում
   ```javascript
   const numbers = [1, 2, 3, 4];
   const [first, , third] = numbers;
   
   console.log(first); // 1
   console.log(third); // 3
   ```
   
   #### Մնացորդային արժեքներ (`rest` օպերատոր)
   ```javascript
   const numbers = [1, 2, 3, 4, 5];
   const [first, second, ...rest] = numbers;
   
   console.log(first); // 1
   console.log(second); // 2
   console.log(rest); // [3, 4, 5]
   ```

   ---
   
   #### Օբյեկտների (Object) Destructuring
   
   #### Օրինակներ
   
   #### Հիմնական Օրինակ
   ```javascript
   const person = {
     name: "Alice",
     age: 25
   };
   
   const { name, age } = person;
   
   console.log(name); // "Alice"
   console.log(age);  // 25
   ```
   
   #### Վերանվանում հատկություններ
   ```javascript
   const person = {
     name: "Alice",
     age: 25
   };
   
   const { name: fullName, age: years } = person;
   
   console.log(fullName); // "Alice"
   console.log(years);    // 25
   ```
   
   #### Արժեքների տեղադրվածություն (Default values)
   ```javascript
   const person = {
     name: "Alice"
   };
   
   const { name, age = 30 } = person;
   
   console.log(name); // "Alice"
   console.log(age);  // 30
   ```
   
   #### Մնացորդային հատկություններ (`rest` օպերատոր)
   ```javascript
   const person = {
     name: "Alice",
     age: 25,
     country: "Armenia"
   };
   
   const { name, ...rest } = person;
   
   console.log(name); // "Alice"
   console.log(rest); // { age: 25, country: "Armenia" }
   ```
   
   ---
   
   #### Կիրառում Ֆունկցիաներում
   
   #### Օրինակներ
   
   #### Զանգվածի Destructuring
   ```javascript
   function sum([a, b]) {
     return a + b;
   }
   
   console.log(sum([5, 10])); // 15
   ```
   
   #### Օբյեկտի Destructuring
   ```javascript
   function introduce({ name, age }) {
     return `My name is ${name} and I am ${age} years old.`;
   }
   
   const person = {
     name: "Alice",
     age: 25
   };
   
   console.log(introduce(person));
   // Output: My name is Alice and I am 25 years old.
   ```

   ---
   
   #### Nested Destructuring
   
   #### Օրինակ
   ```javascript
   const person = {
     name: "Alice",
     address: {
       city: "Yerevan",
       country: "Armenia"
     }
   };
   
   const {
     name,
     address: { city, country }
   } = person;
   
   console.log(name);    // "Alice"
   console.log(city);    // "Yerevan"
   console.log(country); // "Armenia"
   ```

   ---
   
   #### Խառնված Օրինակ
   
   ```javascript
   const data = {
     title: "Destructuring",
     tags: ["JavaScript", "ES6"],
     author: {
       name: "Alice",
       age: 25
     }
   };
   
   const {
     title,
     tags: [firstTag, secondTag],
     author: { name, age }
   } = data;
   
   console.log(title);     // "Destructuring"
   console.log(firstTag);  // "JavaScript"
   console.log(secondTag); // "ES6"
   console.log(name);      // "Alice"
   console.log(age);       // 25
   ```

   ---
   
   #### Destructuring-ի Առավելություններ
   
   1. **Կոդի ընթեռնելիություն:**
      - Կոդը դառնում է կարճ և ընթեռնելի։
   
   2. **Արժեքների արագ մուտք:**
      - Հեշտացնում է մուտքը տվյալների բարդ կառուցվածքներից։
   
   3. **Կոդի պարզեցում:**
      - Կրճատում է ավելորդ հղումները և փոփոխական հայտարարումները։


   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

52. ### Ինչ է Template Literals-ը և ինչպես կարող ենք այն օգտագործել?

   **Template Literals**-ը (կոչվում են նաև Template Strings) ES6-ում ներդրված սինտաքս է, որը թույլ է տալիս ստեղծել տողեր, որոնք ավելի ընթեռնելի և ճկուն են, քան ավանդական տողային սինտաքսը։ Template Literals-ը օգտագործում է backtick (\` \`) նշանները և ապահովում է տողի մեջ արտահայտություններ և բազմատող տեքստեր ներառելու հնարավորություն։

   ---
   
   ## Հիմնական Հատկանիշներ
   
   1. **Backtick (\` \`) Սինտաքս:**
      - Տողերը սահմանվում են backtick-ներով, ոչ թե մեկ կամ կրկնակի չակերտներով։
   
   2. **Ինտերպոլացիա (`${}`):**
      - Հնարավորություն է տալիս տեղադրել փոփոխականներ կամ արտահայտություններ տողի մեջ։
   
   3. **Բազմատող Տեքստեր:**
      - Կարելի է գրել բազմատող տեքստ առանց լրացուցիչ նշանների։
   
   4. **Tags (Tag Functions):**
      - Առաջարկում է օգտագործել ֆունկցիաներ՝ տողի մշակման համար։

   ---
   
   #### Սինտաքս
   ```javascript
   const string = `Your string here`;
   ```

   ---
   
   #### Օրինակներ
   
   #### 1. Տողի ինտերպոլացիա
   
   ```javascript
   const name = "Alice";
   const age = 25;
   
   const message = `My name is ${name} and I am ${age} years old.`;
   console.log(message);
   // Output: My name is Alice and I am 25 years old.
   ```
   
   - **`${}`** սինտաքսը թույլ է տալիս օգտագործել փոփոխականներ կամ արտահայտություններ։
   
   #### 2. Բազմատող տեքստեր
   
   ```javascript
   const multiline = `This is a
   multiline string.`;
   
   console.log(multiline);
   // Output:
   // This is a
   // multiline string.
   ```
   
   #### 3. Արտահայտություններ տողի մեջ
   
   ```javascript
   const a = 10;
   const b = 20;
   
   const result = `The sum of a and b is ${a + b}.`;
   console.log(result);
   // Output: The sum of a and b is 30.
   ```

   ---
   
   #### Tag Functions (Tagging Template Literals)
   
   Tagging-ը թույլ է տալիս Template Literal-ը մշակել ֆունկցիայի միջոցով։
   
   #### Օրինակ՝ Tag Function
   
   ```javascript
   function highlight(strings, ...values) {
     return strings.map((str, index) => {
       return `${str}<strong>${values[index] || ""}</strong>`;
     }).join("");
   }
   
   const name = "Alice";
   const age = 25;
   
   const message = highlight`My name is ${name} and I am ${age} years old.`;
   console.log(message);
   // Output: My name is <strong>Alice</strong> and I am <strong>25</strong> years old.
   ```
   
   #### Ինչպես է աշխատում
   1. `strings`-ը պահում է տողի մասերը՝ առանց փոփոխականների։
   2. `...values`-ը պահում է `${}`-ի արտահայտությունների արդյունքները։
   3. Ֆունկցիան վերադառնում է մշակված տողը։

   ---
   
   #### Template Literals-ի Օգտագործման Տարբեր Դեպքեր
   
   #### 1. HTML-ի ստեղծում
   
   ```javascript
   const title = "Welcome";
   const body = "This is a sample text.";
   
   const html = `
     <div>
       <h1>${title}</h1>
       <p>${body}</p>
     </div>
   `;
   
   console.log(html);
   ```
   
   #### 2. Տվյալների ձևաչափում
   
   ```javascript
   const items = ["Apple", "Banana", "Cherry"];
   
   const list = `
     <ul>
       ${items.map(item => `<li>${item}</li>`).join("")}
     </ul>
   `;
   
   console.log(list);
   ```
   
   #### 3. Դինամիկ տեքստերի ստեղծում
   
   ```javascript
   const user = {
     name: "Alice",
     age: 25,
     city: "Yerevan"
   };
   
   const userInfo = `
     Name: ${user.name}
     Age: ${user.age}
     City: ${user.city}
   `;
   
   console.log(userInfo);
   ```

   ---
   
   #### Template Literals-ի Առավելություններ
   
   1. **Կոդի ընթեռնելիություն:**
      - Հեշտացնում է բազմատող տեքստերի և դինամիկ տողերի ստեղծումը։
   
   2. **Ինտերպոլացիա:**
      - Թույլ է տալիս փոխել տեքստերը դինամիկ կերպով՝ օգտագործելով փոփոխականներ և արտահայտություններ։
   
   3. **Tag Functions-ի աջակցություն:**
      - Հնարավորություն է տալիս կատարել բարդ մշակումներ տողերի վրա։
   
   4. **HTML ձևաչափում:**
      - Հարմար է դինամիկ HTML կոդ գեներացնելու համար։

   ---
   
   #### Թերություններ
   
   1. **Ավելի մեծ ուշադրություն անվտանգությանը:**
      - Template Literals-ը, երբ օգտագործվում է HTML-ի համար, կարող է հանգեցնել **XSS (Cross-Site Scripting)** խոցելիությունների։
   
   2. **Հնարավոր բարձր ծախսեր Tag Functions-ի դեպքում:**
      - Եթե օգտագործվում են բարդ ֆունկցիաներ, կարող է բարձրանալ կատարման ժամանակը։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

53. ### Ինչ է Tagged Templates-ը JavaScript-ում?

   **Tagged Templates**-ը JavaScript-ի հզոր գործիք է, որը թույլ է տալիս Template Literals-ի (կամ Template Strings-ի) միջոցով կատարել բարդ մշակումներ տողի վրա՝ ֆունկցիայի միջոցով։ Այն թույլ է տալիս փոփոխել կամ վերահսկել տողի կառուցվածքը՝ մինչ դրա վերջնական օգտագործումը։

   ---
   
   #### Ինչպես է աշխատում Tagged Templates-ը
   
   Tagged Templates-ը օգտագործում է ֆունկցիա, որը գործարկվում է տողի մասերի և տեղադրված արժեքների վրա։
   
   #### Սինտաքս
   ```javascript
   function tagFunction(strings, ...values) {
     // strings: Տողի ստատիկ մասերը (առանց փոփոխականների)
     // values: `${}`-ի արտահայտությունների արդյունքները
   }
   
   tagFunction`Some text with ${value1} and ${value2}`;
   ```

   ---
   
   #### Օրինակներ
   
   #### Հիմնական Օրինակ
   ```javascript
   function tag(strings, ...values) {
     console.log(strings); // ['My name is ', ' and I am ', ' years old.']
     console.log(values);  // ['Alice', 25]
   }
   
   const name = "Alice";
   const age = 25;
   
   tag`My name is ${name} and I am ${age} years old.`;
   ```

   ---
   
   #### Տողերի փոփոխություն
   
   ```javascript
   function highlight(strings, ...values) {
     return strings.map((str, index) => {
       return `${str}<strong>${values[index] || ""}</strong>`;
     }).join("");
   }
   
   const name = "Alice";
   const age = 25;
   
   const result = highlight`My name is ${name} and I am ${age} years old.`;
   console.log(result);
   // Output: My name is <strong>Alice</strong> and I am <strong>25</strong> years old.
   ```

   ---
   
   #### Օգտագործման Տարբեր Դեպքեր
   
   #### 1. HTML-ի անվտանգ ստեղծում
   
   Tagged Templates-ը կարելի է օգտագործել XSS (Cross-Site Scripting) հարձակումներից պաշտպանվելու համար։
   
   ```javascript
   function escapeHTML(strings, ...values) {
     return strings.map((str, index) => {
       const escapedValue = String(values[index] || "").replace(/</g, "&lt;").replace(/>/g, "&gt;");
       return `${str}${escapedValue}`;
     }).join("");
   }
   
   const userInput = "<script>alert('Hacked!')</script>";
   
   const safeHTML = escapeHTML`<div>${userInput}</div>`;
   console.log(safeHTML);
   // Output: <div>&lt;script&gt;alert('Hacked!')&lt;/script&gt;</div>
   ```
   
   #### 2. Լոգերի ֆորմատավորում
   
   ```javascript
   function logFormat(strings, ...values) {
     const timestamp = new Date().toISOString();
     return `[${timestamp}] ${strings.map((str, i) => `${str}${values[i] || ""}`).join("")}`;
   }
   
   const level = "INFO";
   const message = "Server started";
   
   console.log(logFormat`[${level}] ${message}`);
   // Output: [2023-01-01T12:00:00.000Z] [INFO] Server started
   ```
   
   #### 3. Միջազգայինացում (I18n)
   
   Tagged Templates-ը կարող է օգտագործվել թարգմանություններ իրականացնելու համար։
   
   ```javascript
   function i18n(strings, ...values) {
     const translations = {
       "Hello": "Bonjour",
       "world": "monde"
     };
   
     return strings.map((str, index) => {
       return `${translations[str.trim()] || str}${values[index] || ""}`;
     }).join("");
   }
   
   const message = i18n`Hello, world!`;
   console.log(message);
   // Output: Bonjour, monde!
   ```

   ---
   
   #### Ինչպես է Tag Function-ը աշխատում
   
   1. **Strings մասերը**:
      - Պարունակում են տողի ստատիկ մասերը՝ առանց `${}` արտահայտությունների։
   
   2. **Values մասերը**:
      - Պարունակում են `${}` արտահայտությունների հաշվարկված արժեքները։
   
   3. **Մշակում**:
      - Ֆունկցիան ստանում է strings և values, մշակում է դրանք և վերադարձնում վերջնական տողը։
   
   ---
   
   #### Առավելություններ
   
   1. **Ճկունություն տողերի մշակման մեջ**:
      - Հնարավորություն է տալիս փոխել տողի կառուցվածքը և ավելացնել բարդ ֆորմատավորում։
   
   2. **Անվտանգություն**:
      - Հնարավորություն է տալիս կանխել XSS հարձակումները՝ հատուկ մշակման միջոցով։
   
   3. **Միջազգայինացում**:
      - Կառուցվածքային թարգմանությունների իրականացում։
   
   4. **Կոդի պարզեցում**:
      - Լոգերի, HTML-ի և այլ տեքստերի դինամիկ ձևաչափում։

   ---
   
   #### Թերություններ
   
   1. **Կատարման ժամանակի բարձր ծախսեր**:
      - Բարդ Tag Functions-ը կարող է բարձրացնել կատարման ժամանակը։
   
   2. **Կոդի բարդություն**:
      - Նորեկների համար Tag Function-ի սինտաքսը կարող է բարդ լինել։

   ---
   
   #### Եզրակացություն
   
   **Tagged Templates**-ը JavaScript-ում հզոր գործիք է, որը թույլ է տալիս կառուցել անվտանգ, ճկուն և դինամիկ տեքստեր։ Դրանք իդեալական են HTML-ի ձևաչափման, տվյալների անվտանգության ապահովման և բարդ տողի մշակման համար։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

54. ### Ինչ է Set-ը և Map-ը JavaScript-ում?

   
   **Set** և **Map**-ը JavaScript-ում ES6-ում ներդրված տվյալների կառուցվածքներ են, որոնք առաջարկում են արդյունավետ միջոց մեծ տվյալների հավաքածուները պահպանելու և դրանց վրա գործողություններ կատարելու համար։
   
   - **Set**-ը ներկայացնում է արժեքների հավաքածու, որտեղ չկա կրկնօրինակ։
   - **Map**-ը ներկայացնում է բանալի-արժեք զույգերի հավաքածու, որտեղ բանալիները եզակի են։

   ---
   
   #### 1. Set
   
   #### Նկարագրություն
   **Set**-ը տվյալների կառուցվածք է, որը պահպանում է միայն եզակի արժեքներ։ Այն կարող է պարունակել ցանկացած տիպի արժեք՝ primitive կամ object։
   
   #### Սինտաքս
   ```javascript
   const set = new Set([iterable]);
   ```
   - **`iterable`**: Ցանկալի տվյալների iterable օբյեկտ, օրինակ՝ զանգված։
   
   #### Հիմնական Մեթոդներ
   
   | **Մեթոդ**       | **Նկարագրություն**                                  |
   |------------------|----------------------------------------------------|
   | `add(value)`     | Ավելացնում է նոր արժեք։                            |
   | `delete(value)`  | Հեռացնում է արժեքը։                                |
   | `has(value)`     | Ստուգում է՝ արդյոք արժեքը առկա է Set-ում։          |
   | `clear()`        | Հեռացնում է բոլոր արժեքները։                        |
   | `size`           | Վերադարձնում է Set-ի տարրերի քանակը։              |
   
   #### Օրինակներ
   
   #### Հիմնական Օրինակ
   ```javascript
   const mySet = new Set();
   
   mySet.add(1);
   mySet.add(2);
   mySet.add(2); // Կրկնօրինակները անտեսվում են
   
   console.log(mySet.size); // 2
   console.log(mySet.has(1)); // true
   
   mySet.delete(2);
   console.log(mySet.has(2)); // false
   
   mySet.clear();
   console.log(mySet.size); // 0
   ```
   
   #### Զանգվածից եզակի արժեքներ
   ```javascript
   const array = [1, 2, 2, 3, 4, 4];
   const uniqueSet = new Set(array);
   
   console.log([...uniqueSet]); // [1, 2, 3, 4]
   ```
   
   ---
   
   #### 2. Map
   
   #### Նկարագրություն
   **Map**-ը բանալի-արժեք զույգերի հավաքածու է, որտեղ բանալիները կարող են լինել ցանկացած տիպի, ոչ միայն string (ինչպես օբյեկտների դեպքում)։
   
   #### Սինտաքս
   ```javascript
   const map = new Map([iterable]);
   ```
   - **`iterable`**: Բանալի-արժեք զույգերի iterable օբյեկտ։
   
   #### Հիմնական Մեթոդներ
   
   | **Մեթոդ**        | **Նկարագրություն**                                    |
   |-------------------|------------------------------------------------------|
   | `set(key, value)` | Ավելացնում է բանալի-արժեք զույգ։                      |
   | `get(key)`        | Վերադարձնում է բանալու արժեքը։                        |
   | `has(key)`        | Ստուգում է՝ արդյոք բանալին առկա է Map-ում։           |
   | `delete(key)`     | Հեռացնում է բանալու զույգը։                           |
   | `clear()`         | Հեռացնում է բոլոր բանալի-արժեք զույգերը։              |
   | `size`            | Վերադարձնում է Map-ի տարրերի քանակը։                 |
   
   #### Օրինակներ
   
   #### Հիմնական Օրինակ
   ```javascript
   const myMap = new Map();
   
   myMap.set('name', 'Alice');
   myMap.set('age', 25);
   
   console.log(myMap.get('name')); // "Alice"
   console.log(myMap.has('age')); // true
   
   myMap.delete('age');
   console.log(myMap.has('age')); // false
   
   myMap.clear();
   console.log(myMap.size); // 0
   ```
   
   #### Օբյեկտները որպես բանալի
   ```javascript
   const key = { id: 1 };
   const myMap = new Map();
   
   myMap.set(key, "Object Key");
   console.log(myMap.get(key)); // "Object Key"
   ```

   ---
   
   #### Տարբերություններ Set-ի և Map-ի միջև
   
   | **Հատկանիշ**          | **Set**                                  | **Map**                                  |
   |------------------------|------------------------------------------|------------------------------------------|
   | **Տվյալների կառուցվածք** | Արժեքների հավաքածու                    | Բանալի-արժեք զույգերի հավաքածու          |
   | **Կրկնօրինակներ**       | Չի թույլատրվում                         | Բանալիները եզակի են                      |
   | **Բանալիների տեսակ**    | Միայն արժեքներ (բանալի չկա)             | Ցանկացած տիպի բանալի                    |
   | **Կիրառման դեպքեր**     | Եզակի արժեքներ պահելու համար             | Բարդ բանալի-արժեք հարաբերություններ պահելու համար |

   ---
   
   #### Iteration (Իտերացիա)
   
   #### Set-ի Իտերացիա
   ```javascript
   const mySet = new Set([1, 2, 3]);
   
   for (const value of mySet) {
     console.log(value);
   }
   // Output: 1, 2, 3
   ```
   
   #### Map-ի Իտերացիա
   ```javascript
   const myMap = new Map([
     ['name', 'Alice'],
     ['age', 25]
   ]);
   
   for (const [key, value] of myMap) {
     console.log(`${key}: ${value}`);
   }
   // Output:
   // name: Alice
   // age: 25
   ```

   ---
   
   #### Երբ օգտագործել
   
   - **Set**:
      - Երբ անհրաժեշտ է պահել միայն եզակի արժեքներ։
      - Կրկնօրինակների հեռացում։
   
   - **Map**:
      - Երբ անհրաժեշտ է բանալի-արժեք զույգերի հարաբերություն։
      - Երբ բանալիները պետք է լինեն ոչ string տիպի։
   
   ---
   
   #### Եզրակացություն
   
   **Set** և **Map**-ը JavaScript-ում հզոր և ճկուն տվյալների կառուցվածքներ են։
   
   - **Set**-ը հարմար է եզակի արժեքների համար։
   - **Map**-ը հարմար է բանալի-արժեք զույգերի համար։
   
   Այս կառուցվածքները դարձնում են կոդը ավելի ընթեռնելի և արդյունավետ՝ առաջարկելով ֆունկցիոնալության լայն շրջանակ։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

55. ### Ինչ է JavaScript-ի Event Delegation-ը?
   
   
   **Event Delegation**-ը JavaScript-ում տեխնիկա է, որը թույլ է տալիս բաշխել իրադարձությունների մշակումը ծնողական տարրերին՝ զավակների փոխարեն։ Սա հնարավոր է, քանի որ իրադարձությունները "բարձրանում են" (bubble up) դեպի DOM-ի ծառի վերևը, ինչը թույլ է տալիս ծնող տարրին լսել իրադարձություններ, որոնք տեղի են ունենում նրա զավակների վրա։

   ---
   
   #### Ինչպես է աշխատում Event Delegation-ը
   
   JavaScript-ում իրադարձությունները ունեն **event bubbling** մեխանիզմ, որտեղ իրադարձությունը սկսում է իր ընթացքը սկզբնական տարրից (target) և "բարձրանում է" դեպի նրա ծնողները մինչև հասնում է `document`-ին։ Event Delegation-ը օգտագործում է այս մեխանիզմը՝ թույլ տալով ծնողական տարրին վերահսկել իր բոլոր զավակների իրադարձությունները։

   ---
   
   #### Օրինակներ
   
   #### Առանց Event Delegation-ի
   
   Եթե ձեզ անհրաժեշտ է click իրադարձություն մշակել բազմաթիվ կոճակների համար, առանց Event Delegation-ի կոդը կստացվի այսպես.
   
   ```javascript
   const buttons = document.querySelectorAll('.button');
   
   buttons.forEach(button => {
     button.addEventListener('click', event => {
       console.log(`Button ${event.target.textContent} clicked`);
     });
   });
   ```
   
   #### Event Delegation-ի Օգտագործմամբ
   
   Event Delegation-ի միջոցով մենք կարող ենք օգտագործել միայն մեկ event listener՝ կիրառված ծնողական տարրի վրա.
   
   ```javascript
   const parent = document.querySelector('.parent');
   
   parent.addEventListener('click', event => {
     if (event.target.classList.contains('button')) {
       console.log(`Button ${event.target.textContent} clicked`);
     }
   });
   ```
   
   #### Ինչպես է աշխատում
   1. **`event.target`**: Այն տարրը, որտեղ իրականում տեղի է ունեցել իրադարձությունը։
   2. **`classList.contains`**: Ստուգում է, թե արդյոք իրադարձությունը տեղի է ունեցել կոնկրետ տարրի վրա։

   ---
   
   #### Օգտագործման Տարբեր Դեպքեր
   
   #### 1. Դինամիկ տարրեր
   Event Delegation-ը օգտակար է, երբ դուք ստեղծում եք տարրեր դինամիկ կերպով։
   
   ```javascript
   const list = document.querySelector('.list');
   
   list.addEventListener('click', event => {
     if (event.target.tagName === 'LI') {
       console.log(`Clicked on item: ${event.target.textContent}`);
     }
   });
   
   // Դինամիկ տարր ավելացնել
   const newItem = document.createElement('li');
   newItem.textContent = 'New Item';
   list.appendChild(newItem);
   ```
   
   #### 2. Ավելի քիչ հիշողության օգտագործում
   Երբ ունեք բազմաթիվ տարրեր, Event Delegation-ը նվազեցնում է հիշողության օգտագործումը՝ փոխարենը կիրառելով միայն մեկ event listener։

   ---
   
   #### Առավելություններ
   
   1. **Արդյունավետություն:**
      - Նվազեցնում է event listeners-ի քանակը, ինչը բարելավում է կատարողականությունը։
   
   2. **Դինամիկ տարրերի աջակցություն:**
      - Ապահովում է դինամիկ ավելացված տարրերի իրադարձությունների կառավարումը։
   
   3. **Կոդի պարզեցում:**
      - Ավելի քիչ կոդ է անհրաժեշտ, քանի որ անհրաժեշտ է միայն մեկ listener։
   
   ---
   
   #### Թերություններ
   
   1. **Event bubbling-ի կախվածություն:**
      - Տեխնիկան հիմնված է իրադարձության "բարձրանալու" մեխանիզմի վրա, ինչը կարող է որոշ դեպքերում անցանկալի լինել։
   
   2. **Սահմանափակումներ իրադարձությունների տեսակների վրա:**
      - Որոշ իրադարձություններ, ինչպիսիք են `focus`-ը կամ `blur`-ը, չեն աջակցում bubbling։
   
   3. **Լրացուցիչ ստուգումներ:**
      - Անհրաժեշտ է ստուգել `event.target`-ը, որպեսզի համոզվեք, որ իրադարձությունը տեղի է ունեցել ճիշտ տարրի վրա։
   
   ---
   
   #### Եզրակացություն
   
   **Event Delegation**-ը հզոր տեխնիկա է JavaScript-ում, որը թույլ է տալիս պարզեցնել իրադարձությունների կառավարումը, բարելավել կատարողականությունը և աջակցել դինամիկ տարրերին։ Այս մոտեցումը հատկապես օգտակար է, երբ աշխատում եք մեծ թվով տարրերի կամ դինամիկ բովանդակության հետ։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

56. ### Ինչ է Factory Function-ը JavaScript-ում?
   
   **Factory Function**-ը JavaScript-ում ֆունկցիա է, որը վերադարձնում է նոր օբյեկտ։ Այն օգտագործվում է օբյեկտներ ստեղծելու համար՝ առանց նոր կոնստրուկտորների կամ դասերի անհրաժեշտության։ Factory Function-ը հնարավորություն է տալիս ստեղծել օբյեկտների բազմացում, որոնք կարող են կիսել ընդհանուր տրամաբանություն կամ տարբեր լինել ըստ փոխանցված պարամետրերի։

   ---
   
   #### Ինչու օգտագործել Factory Function
   
   1. **Դասերի (Class) այլընտրանք:**
      - Հեշտ և ընթեռնելի սինտաքս։
   
   2. **Անկախություն նոր օպերատորից:**
      - Չկա կարիք օգտագործելու `new` օպերատոր։
   
   3. **Կոդի վերսկսում (Reuse):**
      - Հնարավորություն է տալիս կրկին օգտագործել նույն տրամաբանությունը տարբեր օբյեկտների համար։
   
   4. **Ինկապսուլացիա:**
      - Օբյեկտի ներսի վիճակը և մեթոդները պաշտպանված են արտաքին մուտքից։

   ---
   
   #### Սինտաքս
   ```javascript
   function createObject(param1, param2) {
     return {
       property1: param1,
       property2: param2,
       method() {
         console.log(`${this.property1} and ${this.property2}`);
       }
     };
   }
   
   const obj = createObject('value1', 'value2');
   obj.method(); // Output: value1 and value2
   ```

   ---
   
   #### Օրինակներ
   
   #### Հիմնական Օրինակ
   
   ```javascript
   function createPerson(name, age) {
     return {
       name,
       age,
       greet() {
         console.log(`Hello, my name is ${this.name} and I am ${this.age} years old.`);
       }
     };
   }
   
   const person1 = createPerson('Alice', 30);
   const person2 = createPerson('Bob', 25);
   
   person1.greet(); // Output: Hello, my name is Alice and I am 30 years old.
   person2.greet(); // Output: Hello, my name is Bob and I am 25 years old.
   ```
   
   ---
   
   #### Factory Function-ով Մասնավոր Տվյալների Ապահովում
   
   ```javascript
   function createCounter() {
     let count = 0; // Մասնավոր փոփոխական
   
     return {
       increment() {
         count++;
         console.log(`Count: ${count}`);
       },
       decrement() {
         count--;
         console.log(`Count: ${count}`);
       },
       getCount() {
         return count;
       }
     };
   }
   
   const counter = createCounter();
   counter.increment(); // Count: 1
   counter.increment(); // Count: 2
   counter.decrement(); // Count: 1
   console.log(counter.getCount()); // 1
   ```
   
   ---
   
   #### Օբյեկտների Կոմպոզիցիա
   Factory Function-ները հարմար են օբյեկտների կոմպոզիցիայի համար՝ բազմակի հատկություններ և մեթոդներ ավելացնելու նպատակով։
   
   ```javascript
   function createMover() {
     return {
       move() {
         console.log('Moving...');
       }
     };
   }
   
   function createShouter() {
     return {
       shout() {
         console.log('Shouting!');
       }
     };
   }
   
   function createRobot(name) {
     return {
       name,
       ...createMover(),
       ...createShouter()
     };
   }
   
   const robot = createRobot('Robo');
   robot.move();  // Moving...
   robot.shout(); // Shouting!
   ```

   ---
   
   #### Factory Function vs Constructor Function
   
   | **Հատկանիշ**                | **Factory Function**                         | **Constructor Function**                   |
   |-----------------------------|---------------------------------------------|-------------------------------------------|
   | **Սինտաքս**                 | Սովորական ֆունկցիա                         | Պահանջում է `new` օպերատոր               |
   | **Մասնավոր փոփոխականներ**  | Հեշտորեն աջակցվում են փակ (closure) սինտաքսով | Պահանջում է լրացուցիչ մեթոդներ            |
   | **Վերադարձի տեսակ**         | Օբյեկտ                                     | Արտադրած օբյեկտ կամ `undefined`          |
   | **Օգտագործման պարզություն**  | Ավելի հեշտ                                  | Ավելի բարդ                                 |

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

57. ### Ինչ է Class-ը JavaScript-ում?
   
   **Class**-ը JavaScript-ում ES6-ում ներկայացված սինտաքս է, որը ապահովում է օբյեկտի վրա հիմնված ծրագրավորման (OOP) մոտեցում։ Class-ները օգտագործվում են օբյեկտներ ստեղծելու համար, որոնք կարող են պարունակել տվյալներ (հատկություններ) և ֆունկցիաներ (մեթոդներ)։ Class-ը JavaScript-ում հանդիսանում է `prototype`-ի վրա հիմնված ժառանգման պարզեցված սինտաքս։

   ---
   
   #### Սինտաքս
   
   ```javascript
   class ClassName {
     constructor(param1, param2) {
       this.property1 = param1;
       this.property2 = param2;
     }
   
     method1() {
       console.log('This is a method');
     }
   }
   
   const instance = new ClassName('value1', 'value2');
   instance.method1();
   ```
   
   ### Հիմնական բաղադրիչներ
   1. **Constructor:**
      - Սինտաքս, որը օգտագործվում է class-ի նոր օբյեկտների սկզբնականացման համար։
   
   2. **Methods (Մեթոդներ):**
      - Ֆունկցիաներ, որոնք սահմանվում են class-ի ներսում։
   
   3. **Instance:**
      - Class-ի օրինակ, որը ստեղծվում է `new` օպերատորով։
   
   ---
   
   #### Օրինակներ
   
   #### Հիմնական Օրինակ
   
   ```javascript
   class Person {
     constructor(name, age) {
       this.name = name;
       this.age = age;
     }
   
     greet() {
       console.log(`Hello, my name is ${this.name} and I am ${this.age} years old.`);
     }
   }
   
   const person1 = new Person('Alice', 30);
   const person2 = new Person('Bob', 25);
   
   person1.greet(); // Output: Hello, my name is Alice and I am 30 years old.
   person2.greet(); // Output: Hello, my name is Bob and I am 25 years old.
   ```

   ---
   
   #### Ժառանգում (Inheritance)
   
   JavaScript-ի Class-ները աջակցում են ժառանգումը `extends` բանալի բառի միջոցով։
   
   #### Օրինակ
   
   ```javascript
   class Animal {
     constructor(name) {
       this.name = name;
     }
   
     speak() {
       console.log(`${this.name} makes a noise.`);
     }
   }
   
   class Dog extends Animal {
     speak() {
       console.log(`${this.name} barks.`);
     }
   }
   
   const dog = new Dog('Buddy');
   dog.speak(); // Output: Buddy barks.
   ```

   ---
   
   #### Static Մեթոդներ
   
   **Static** մեթոդները կոչվում են հենց class-ից, այլ ոչ թե նրա օրինակներից։
   
   ### Օրինակ
   ```javascript
   class MathUtils {
     static add(a, b) {
       return a + b;
     }
   }
   
   console.log(MathUtils.add(5, 10)); // Output: 15
   ```


   ---
   
   #### Getters և Setters
   
   Getters և Setters ապահովում են հատկությունների հասանելիություն և կառավարում class-ի ներսում։
   
   ### Օրինակ
   ```javascript
   class Rectangle {
     constructor(width, height) {
       this.width = width;
       this.height = height;
     }
   
     get area() {
       return this.width * this.height;
     }
   
     set area(value) {
       this.width = Math.sqrt(value);
       this.height = Math.sqrt(value);
     }
   }
   
   const rect = new Rectangle(4, 5);
   console.log(rect.area); // Output: 20
   rect.area = 36;
   console.log(rect.width, rect.height); // Output: 6 6
   ```

   ---
   
   #### Class-ի Հատկանիշները
   
   | **Հատկանիշ**             | **Նկարագրություն**                                 |
   |---------------------------|--------------------------------------------------|
   | **Constructor**           | Սահմանում է class-ի սկզբնականացման տրամաբանությունը։|
   | **Methods**               | Ֆունկցիաներ, որոնք կապված են class-ի հետ։         |
   | **Static Methods**        | Մեթոդներ, որոնք կապված են class-ի հետ, ոչ թե օրինակների։|
   | **Inheritance**           | Թույլ է տալիս ստեղծել նոր class-ներ՝ ժառանգելով գոյություն ունեցող class-ից։|
   
   ---
   
   #### Class vs Constructor Function
   
   | **Հատկանիշ**             | **Class**                               | **Constructor Function**                |
   |---------------------------|-----------------------------------------|-----------------------------------------|
   | **Սինտաքսի պարզություն** | Ավելի ընթեռնելի և կառուցվածքային       | Ավելի բարդ և կոդային հին մոտեցում       |
   | **Inheritance**           | Աջակցում է `extends`-ի միջոցով          | Պահանջում է `Object.create` կամ `prototype`|
   | **Static Methods**        | Պարզորեն սահմանվում են `static` բանալիով | Պահանջում է լրացուցիչ կոդ                 |

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

58. ### Ինչ է object cloning-ի տարբեր եղանակներ JavaScript-ում?
   
   **Object Cloning**-ը JavaScript-ում տվյալ օբյեկտի կրկնօրինակ ստեղծելու գործընթացն է։ Cloning-ը կարևոր է, երբ ուզում ենք ստեղծել օբյեկտի նոր տարբերակ, որը անկախ կլինի սկզբնական օբյեկտից։
   
   JavaScript-ում օբյեկտները փոխանցվում են ըստ հղման (reference), ինչը նշանակում է, որ ուղղակի նշանակման դեպքում նոր փոփոխականը կկապվի սկզբնական օբյեկտի հետ։
   
   ```javascript
   const obj1 = { key: 'value' };
   const obj2 = obj1; // Reference
   obj2.key = 'new value';
   
   console.log(obj1.key); // "new value"
   ```
   
   Object Cloning-ի միջոցով հնարավոր է ստեղծել անկախ օբյեկտներ։


   ---
   
   #### Տարբեր Եղանակներ
   
   #### 1. **Shallow Copy**
   Shallow Copy-ը ստեղծում է օբյեկտի միայն առաջին մակարդակի հատկությունների կրկնօրինակ։ Nested օբյեկտները (deep properties) շարունակում են պահել իրենց հղումները։
   
   #### Օրինակներ
   
   ##### Օգտագործելով `Object.assign()`
   ```javascript
   const obj1 = { a: 1, b: { c: 2 } };
   const obj2 = Object.assign({}, obj1);
   
   obj2.b.c = 42;
   console.log(obj1.b.c); // 42
   ```
   
   ##### Օգտագործելով Spread Operator (`...`)
   ```javascript
   const obj1 = { a: 1, b: { c: 2 } };
   const obj2 = { ...obj1 };
   
   obj2.b.c = 42;
   console.log(obj1.b.c); // 42
   ```
   
   #### 2. **Deep Copy**
   Deep Copy-ը ստեղծում է օբյեկտի բոլոր մակարդակների անկախ կրկնօրինակ։ Nested օբյեկտները նույնպես կկրկնօրինակվեն։
   
   #### Օրինակներ
   
   ##### Օգտագործելով Recursion
   ```javascript
   function deepClone(obj) {
     if (obj === null || typeof obj !== 'object') {
       return obj;
     }
   
     const clone = Array.isArray(obj) ? [] : {};
   
     for (const key in obj) {
       if (obj.hasOwnProperty(key)) {
         clone[key] = deepClone(obj[key]);
       }
     }
   
     return clone;
   }
   
   const obj1 = { a: 1, b: { c: 2 } };
   const obj2 = deepClone(obj1);
   
   obj2.b.c = 42;
   console.log(obj1.b.c); // 2
   ```
   
   #### Օգտագործելով `JSON.parse` և `JSON.stringify`
   ```javascript
   const obj1 = { a: 1, b: { c: 2 } };
   const obj2 = JSON.parse(JSON.stringify(obj1));
   
   obj2.b.c = 42;
   console.log(obj1.b.c); // 2
   ```
   
   > **Նշում:** Այս մեթոդը չի աջակցում ֆունկցիաներին կամ `undefined` արժեքներին։
   
   #### Օգտագործելով Third-Party Գրադարաններ (Lodash)
   ```javascript
   const _ = require('lodash');
   const obj1 = { a: 1, b: { c: 2 } };
   const obj2 = _.cloneDeep(obj1);
   
   obj2.b.c = 42;
   console.log(obj1.b.c); // 2
   ```


   ---
   
   #### Համեմատություն Shallow և Deep Copy-ի միջև
   
   | **Հատկանիշ**         | **Shallow Copy**              | **Deep Copy**                 |
   |-----------------------|-------------------------------|-------------------------------|
   | **Կրկնօրինակ մակարդակ** | Միայն առաջին մակարդակը        | Բոլոր մակարդակները            |
   | **Կատարողականություն**  | Արագ և արդյունավետ            | Ավելի դանդաղ                  |
   | **Ներդրված օբյեկտներ**  | Պահպանում է հղումը            | Ստեղծում է նոր օբյեկտներ      |

   ---
   
   #### Երբ օգտագործել
   
   1. **Shallow Copy:**
      - Երբ օբյեկտը չունի ներդրված (nested) կառուցվածքներ կամ դրանք փոփոխության ենթակա չեն։
   
   2. **Deep Copy:**
      - Երբ աշխատում եք բարդ, բազմամակարդակ օբյեկտների հետ և ցանկանում եք ամբողջական անկախություն սկզբնական օբյեկտից։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---
59. ### Ինչ է JSON-ը և ինչու է այն կարևոր JavaScript-ում?

   
   **JSON (JavaScript Object Notation)**-ը թեթև, պարզ և ընթեռնելի տվյալների փոխանակման ձևաչափ է։ Այն ներկայացնում է տվյալների կառուցվածքը `key-value` զույգերի կամ զանգվածների միջոցով և հիմնականում օգտագործվում է վեբ հավելվածներում սերվերի և հաճախորդի միջև տվյալների փոխանակման համար։
   
   JSON-ը հիմնված է JavaScript-ի սինտաքսի վրա, սակայն լայնորեն կիրառվում է բազմաթիվ ծրագրավորման լեզուներում։

   ---
   
   #### JSON-ի Հիմնական Սինտաքս
   
   1. **Օբյեկտներ**
      - Տվյալները ներկայացվում են `key-value` զույգերով, որտեղ `key`-ը միշտ տողի տեսքով է, իսկ `value`-ը կարող է լինել տող, թիվ, boolean, null, զանգված կամ այլ օբյեկտ։
   
   2. **Զանգվածներ**
      - Տվյալների շարքը ներկայացվում է զանգվածներով՝ տողի կամ թվի տեսքով արժեքներով։
   
   #### Օրինակ
   ```json
   {
     "name": "Alice",
     "age": 25,
     "isStudent": false,
     "skills": ["JavaScript", "React", "Node.js"]
   }
   ```
   
   - **Key**-երը միշտ պետք է լինեն տողերի տեսքով։
     - Արժեքները կարող են լինել հետևյալ տեսակների՝
        - Տող (string): "Alice"
        - Թիվ (number): 25
        - Boolean: true կամ false
        - Null: null
        - Զանգված (array): ["JavaScript", "React"]
        - Օբյեկտ (object): { "key": "value" }

   ---
   
   #### Ինչպես է աշխատում JSON-ը JavaScript-ում
   
   JavaScript-ը առաջարկում է ներկառուցված մեթոդներ JSON-ի հետ աշխատելու համար՝ `JSON.parse` և `JSON.stringify`։
   
   #### 1. JSON.parse
   Այս մեթոդը օգտագործվում է JSON տողը JavaScript օբյեկտի վերածելու համար։
   
   #### Օրինակ
   ```javascript
   const jsonString = '{"name": "Alice", "age": 25}';
   const user = JSON.parse(jsonString);
   
   console.log(user.name); // Output: Alice
   console.log(user.age);  // Output: 25
   ```
   
   #### 2. JSON.stringify
   Այս մեթոդը օգտագործվում է JavaScript օբյեկտը JSON տողի վերածելու համար։
   
   #### Օրինակ
   ```javascript
   const user = { name: "Alice", age: 25 };
   const jsonString = JSON.stringify(user);
   
   console.log(jsonString); // Output: {"name":"Alice","age":25}
   ```

   ---
   
   #### JSON-ի Կարևորությունը JavaScript-ում
   
   1. **Տվյալների Փոխանակում**
      - JSON-ը հիմնական ձևաչափն է, որն օգտագործվում է սերվերի և հաճախորդի միջև տվյալների փոխանակման համար։ Օրինակ՝ API-ների միջոցով տվյալներ ստանալու և ուղարկելու համար։
   
   2. **API-ների Համատեղելիություն**
      - JSON-ը աջակցվում է REST և GraphQL API-ներում՝ որպես տվյալների փոխանցման ստանդարտ ձևաչափ։
   
   3. **Թեթևություն**
      - JSON-ը ավելի փոքր և արագ է, քան XML-ը, ինչը մեծացնում է վեբ հավելվածի կատարողականությունը։
   
   4. **Ընթեռնելիություն**
      - JSON-ը հեշտ է կարդալ և գրել, ինչը դարձնում է այն հարմար ծրագրավորողների և ոչ տեխնիկական մասնագետների համար։
   
   5. **Լայն աջակցություն**
      - JSON-ը աջակցվում է գրեթե բոլոր ժամանակակից ծրագրավորման լեզուներում, ինչը դարձնում է այն ունիվերսալ լուծում տվյալների փոխանակման համար։
   
   ---
   
   #### JSON-ի և JavaScript-ի միջև Կապը
   
   JSON-ը և JavaScript-ը սերտորեն կապված են միմյանց հետ։ JSON-ը հիմնված է JavaScript-ի օբյեկտի սինտաքսի վրա, և դրա հետ աշխատելու համար JavaScript-ը տրամադրում է հարմարավետ մեթոդներ։
   
   - **Օրինակ՝ Տվյալների Փոխանցում**
   ```javascript
   const apiResponse = '{"name": "Alice", "age": 25}';
   const user = JSON.parse(apiResponse);
   
   user.isStudent = true;
   
   const updatedData = JSON.stringify(user);
   console.log(updatedData); // Output: {"name":"Alice","age":25,"isStudent":true}
   ```

   ---
   
   #### JSON-ի Սահմանափակումներ
   
   1. **Կոշտ Սինտաքս**
      - Key-երը պետք է լինեն տողերի տեսքով։
      - Տվյալները չեն կարող պարունակել ֆունկցիաներ, `undefined` կամ `NaN` արժեքներ։
   
   2. **Անվտանգություն**
      - Եթե JSON տվյալները ստուգված չեն, դրանք կարող են պարունակել վնասակար բովանդակություն։
   
   3. **Կարդալ միայն Սինխրոն կերպով**
      - JSON-ը JavaScript-ում չի ապահովում streaming կամ մասային կարդալու մեթոդներ։
   
   4. **Կոմպլեքս տվյալների սինտաքս**
      - Nested (ներդրված) օբյեկտները կարող են ավելի բարդ լինել կարդալու կամ կառավարելու համար։

   ---
   
   #### JSON-ի Տարբերությունը XML-ի Համեմատ
   
   | **Հատկանիշ**       | **JSON**                             | **XML**                              |
   |---------------------|---------------------------------------|---------------------------------------|
   | **Սինտաքսի պարզություն** | Ավելի կարճ և ընթեռնելի                 | Ավելի բարդ և ծավալուն                 |
   | **Տվյալների տեսակներ**   | Աջակցում է primitive տեսակներին        | Աջակցում է միայն տեքստին             |
   | **Օգտագործման դյուրինություն** | Թեթև և հեշտ ինտեգրվող                | Ավելի ծանր և պահանջում է լրացուցիչ գրադարաններ |

   ---
   
   #### Երբ օգտագործել JSON
   
   1. **API-ներ**
      - Օգտագործեք JSON API-ների տվյալների փոխանակման համար։
   
   2. **Տվյալների պահպանում**
      - Հարմար է փոքր չափերի տվյալներ պահելու համար՝ localStorage-ում կամ sessionStorage-ում։
   
   3. **Կոմպլեքս օբյեկտների փոխանցում**
      - Հարմար է nested օբյեկտների և զանգվածների փոխանցման համար։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

60. ### Ինչ է AJAX-ը JavaScript-ում?

   **AJAX (Asynchronous JavaScript and XML)**-ը տեխնոլոգիաների համակցություն է, որը թույլ է տալիս վեբ հավելվածներին փոխանակել տվյալներ սերվերի հետ առանց էջը վերաբեռնելու։ Այն թույլ է տալիս իրականացնել դինամիկ և ինտերակտիվ վեբ հավելվածներ՝ տվյալները ստանալով կամ ուղարկելով ֆոնային ռեժիմում։
   
   Չնայած անվանման մեջ նշվում է XML-ը, այսօր AJAX-ը հաճախ օգտագործվում է JSON տվյալների փոխանակման համար՝ իր պարզության և թեթևության շնորհիվ։
   
   ---
   
   #### Ինչպես է աշխատում AJAX-ը
   
   AJAX-ը օգտագործում է **XMLHttpRequest (XHR)** օբյեկտը կամ **Fetch API**-ն՝ սերվերի հետ ֆոնային կապ հաստատելու համար։
   
   #### Հիմնական քայլեր
   1. Ստեղծվում է պահանջ (request) սերվերին։
   2. Սերվերը մշակում է պահանջը և վերադարձնում պատասխան (response)։
   3. Պատասխանը օգտագործվում է՝ էջը կամ տվյալները թարմացնելու համար՝ առանց ամբողջ էջը վերաբեռնելու։
   
   ---
   
   #### Օրինակ՝ Օգտագործելով XMLHttpRequest
   
   ```javascript
   const xhr = new XMLHttpRequest();
   
   xhr.open('GET', 'https://jsonplaceholder.typicode.com/posts', true);
   
   xhr.onload = function () {
     if (xhr.status === 200) {
       const data = JSON.parse(xhr.responseText);
       console.log(data);
     }
   };
   
   xhr.onerror = function () {
     console.error('Request failed');
   };
   
   xhr.send();
   ```
   
   - **`open(method, url, async)`**: Նախապատրաստում է պահանջը (GET կամ POST):
   - `method`: HTTP մեթոդ։
   - `url`: Պահանջի URL հասցեն։
   - `async`: Սինխրոն կամ ասինխրոն պահանջ (default՝ true):
   
   - **`send()`**: Ուղարկում է պահանջը սերվերին։
   
   ---
   
   #### Օրինակ՝ Օգտագործելով Fetch API
   
   Fetch API-ն համեմատաբար նոր և ավելի ընթեռնելի մեթոդ է AJAX գործողությունների համար։
   
   ```javascript
   fetch('https://jsonplaceholder.typicode.com/posts')
     .then(response => {
       if (!response.ok) {
         throw new Error('Network response was not ok');
       }
       return response.json();
     })
     .then(data => console.log(data))
     .catch(error => console.error('Fetch error:', error));
   ```
   
   - **`fetch(url)`**: Ուղարկում է պահանջը նշված URL հասցեին։
   - **`.then(response => response.json())`**: Վերածում է պատասխանը JSON օբյեկտի։
   - **`.catch()`**: Կառավարում է հնարավոր սխալները։

   ---
   
   #### AJAX-ի Առավելությունները
   
   1. **Անխափան օգտագործման փորձ**
      - Օգտագործողները չեն տեսնում էջի թարմացում կամ "loading" էֆեկտներ։
   
   2. **Արագ կատարողականություն**
      - Փոփոխվում են միայն անհրաժեշտ տվյալները, ոչ թե ամբողջ էջը։
   
   3. **Դինամիկ և ինտերակտիվ բովանդակություն**
      - Թույլ է տալիս իրականացնել որոնման դաշտեր, ավտոմատ լրացում, ֆիլտրներ և այլն։
   
   4. **Շերտավորված տվյալների կառավարում**
      - Թույլ է տալիս սերվերի տվյալները կառավարել առանձին ֆոնային գործընթացում։

   ---
   
   #### AJAX-ի Թերությունները
   
   1. **SEO Խնդիրներ**
      - Որոնման համակարգերը կարող են չսատարել դինամիկ բովանդակության "կարդալը"։
   
   2. **Անվտանգություն**
      - Եթե տվյալները չեն ստուգվում, դրանք կարող են ենթարկվել XSS (Cross-Site Scripting) հարձակումների։
   
   3. **Զննարկչի աջակցություն**
      - Հին զննարկիչները կարող են չաջակցել AJAX-ի որոշ հատկություններին։
   
   ---
   
   #### Երբ օգտագործել AJAX
   
   1. **Real-Time Տվյալների Թարմացում**
      - Օրինակ՝ վիճակագրական վահանակներ, չաթ հավելվածներ։
   
   2. **Որոնման դաշտեր և ֆիլտրեր**
      - Հնարավորություն է տալիս արդյունքները թարմացնել անմիջապես առանց էջի վերաբեռնելու։
   
   3. **Ֆորմաների Աջակցություն**
      - Ֆորմայի տվյալները սերվերին ուղարկելու համար՝ առանց էջը թարմացնելու։

   ---
   
   #### AJAX-ի և JSON-ի Կապը
   
   AJAX-ը հաճախ օգտագործվում է JSON տվյալների փոխանակման համար, քանի որ JSON-ը թեթև և հեշտ ինտեգրվող ձևաչափ է։ Օրինակ՝ API-ներից JSON տվյալներ ստանալու և դրանք վեբ հավելվածում ցուցադրելու համար։
   
   ```javascript
   fetch('https://jsonplaceholder.typicode.com/posts')
     .then(response => response.json())
     .then(data => {
       data.forEach(post => console.log(post.title));
     });
   ```

   ---
   
   #### Եզրակացություն
   
   **AJAX**-ը JavaScript-ում կարևոր տեխնոլոգիա է, որը թույլ է տալիս վեբ հավելվածներին դինամիկ կերպով փոխանակել տվյալներ սերվերի հետ՝ առանց էջը վերաբեռնելու։ Դրա միջոցով հնարավոր է ապահովել ավելի արագ, ինտերակտիվ և արդյունավետ օգտագործման փորձ։
   
   Օգտագործելով AJAX-ը՝ դուք կարող եք ստեղծել ժամանակակից վեբ հավելվածներ, որոնք հարմար են ինչպես օգտագործողների, այնպես էլ ծրագրավորողների համար։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

61. ### Ինչ է Fetch API-ը և ինչպես է այն աշխատում?

   
   **Fetch API**-ն JavaScript-ի ներկառուցված գործիք է, որը թույլ է տալիս իրականացնել HTTP հարցումներ։ Այն թույլ է տալիս ստանալ և ուղարկել տվյալներ սերվերին՝ օգտագործելով Promises։ Fetch API-ն ներկայացնում է ավելի ժամանակակից և պարզ մեթոդ, որը փոխարինում է հին `XMLHttpRequest`-ին։

   ---
   
   #### Հիմնական Հատկանիշներ
   
   1. **Promise-ների վրա հիմնված**:
      - Ապահովում է `.then` և `.catch` սինտաքս, ինչը պարզեցնում է ասինխրոն հարցումների կառավարումը։
   
   2. **Կառուցված JavaScript-ում**:
      - Fetch API-ն ներկառուցված է ժամանակակից զննարկիչներում, և դուք կարող եք այն օգտագործել առանց լրացուցիչ գրադարանների։
   
   3. **Հեշտ ինտեգրում JSON-ի հետ**:
      - Պատասխանները հեշտությամբ վերածվում են JSON օբյեկտների՝ օգտագործելով `.json()` մեթոդը։
   
   4. **Աջակցում է տարբեր HTTP մեթոդներին**:
      - Աջակցվում են `GET`, `POST`, `PUT`, `DELETE` և այլ HTTP մեթոդները։
   
   5. **Սինտաքսի պարզություն**:
      - Ընթերցվող և մաքուր կոդի գրելու համար։

   ---
   
   #### Ինչպես է աշխատում Fetch API-ը
   
   #### Սինտաքս
   ```javascript
   fetch(url, options)
     .then(response => responseHandler)
     .catch(error => errorHandler);
   ```
   - **`url`**: Պահանջի նպատակային հասցեն։
   - **`options`**: Պահանջի կարգավորումներ (օրինակ՝ HTTP մեթոդ, վերնագրեր և այլն)։
   
   ---
   
   #### Օրինակներ
   
   #### 1. Հիմնական Օրինակ (GET հարցում)
   ```javascript
   fetch('https://jsonplaceholder.typicode.com/posts')
     .then(response => {
       if (!response.ok) {
         throw new Error('Network response was not ok');
       }
       return response.json();
     })
     .then(data => console.log(data))
     .catch(error => console.error('Error:', error));
   ```
   
   - **`response.ok`**: Ստուգում է՝ արդյոք սերվերի պատասխանը հաջող էր։
   - **`.json()`**: Պատասխանը JSON օբյեկտի վերածելու մեթոդ։
   
   #### 2. POST հարցում (Տվյալների ուղարկում)
   ```javascript
   fetch('https://jsonplaceholder.typicode.com/posts', {
     method: 'POST',
     headers: {
       'Content-Type': 'application/json'
     },
     body: JSON.stringify({ title: 'New Post', body: 'This is the content', userId: 1 })
   })
     .then(response => response.json())
     .then(data => console.log(data))
     .catch(error => console.error('Error:', error));
   ```
   
   - **`method`**: Նշում է HTTP մեթոդը (օրինակ՝ `POST`)։
   - **`headers`**: Մասնաճյուղ, որը սահմանում է լրացուցիչ HTTP վերնագրեր։
   - **`body`**: Ուղարկվող տվյալները։
   
   #### 3. Հատուկ Վերնագրերով Պահանջ
   ```javascript
   fetch('https://jsonplaceholder.typicode.com/posts/1', {
     method: 'DELETE',
     headers: {
       'Authorization': 'Bearer token'
     }
   })
     .then(response => {
       if (response.ok) {
         console.log('Post deleted successfully');
       }
     })
     .catch(error => console.error('Error:', error));
   ```

   ---
   
   #### Fetch API-ի Առավելություններ
   
   1. **Կառուցված է JavaScript-ում**:
      - Չկա անհրաժեշտություն լրացուցիչ գրադարանների։
   
   2. **Promise-ների աջակցություն**:
      - Պարզացնում է ասինխրոն կոդի կառավարումը։
   
   3. **Աջակցություն բրաուզերներում**:
      - Աշխատում է ժամանակակից բրաուզերներում։
   
   4. **Հեշտ ինտեգրում JSON-ի հետ**:
      - Պատասխանների JSON վերամշակումը դյուրին է։
   
   ---
   
   #### Fetch API-ի Թերություններ
   
   1. **Timeout-ի բացակայություն**:
      - Fetch API-ն չունի ներկառուցված timeout կարգավորում։ Այն ավելացնելու համար պետք է օգտագործել լրացուցիչ տրամաբանություն։
   
   2. **Սխալների սահմանափակ կառավարում**:
      - Fetch-ը սխալ է վերադարձնում միայն ցանցային սխալների դեպքում։ HTTP սխալները (օրինակ՝ 404 կամ 500) պետք է կառավարել ձեռքով։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---
62. ### Ինչ է Axios-ը և ինչ է տարբերությունը Fetch API-ի հետ?

   **Axios**-ը JavaScript-ի գրադարան է, որը թույլ է տալիս հեշտությամբ կատարել HTTP հարցումներ։ Այն հիմնված է **Promise**-ների վրա և ապահովում է հեշտ օգտագործման ինտերֆեյս տվյալների բեռնելու և սերվերին ուղարկելու համար։ Axios-ը լայնորեն օգտագործվում է վեբ հավելվածներում՝ շնորհիվ իր ճկունության, հեշտ ինտեգրման և լրացուցիչ ֆունկցիոնալության։
   
   #### Հիմնական Հատկանիշներ
   
   1. **Promise-ների վրա հիմնված**:
      - Ապահովում է `.then` և `.catch` սինտաքս։
   
   2. **Աջակցում է բրաուզերին և Node.js-ին**:
      - Կարելի է օգտագործել ինչպես ֆրոնտենդում, այնպես էլ բեքենդում։
   
   3. **Ավտոմատ JSON վերամշակում**:
      - Պատասխանները ավտոմատ կերպով վերածվում են JSON օբյեկտի։
   
   4. **Խնդիրների կառավարում (Interceptors):**
      - Թույլ է տալիս վերամշակել պահանջներն ու պատասխանները։
   
   5. **HTTP մեթոդների աջակցություն:**
      - Աջակցում է GET, POST, PUT, DELETE և այլ մեթոդներին։
   
   6. **Timeout և սխալների կառավարում:**
      - Թույլ է տալիս սահմանել ժամանակի սահմանափակում և կառավարել սխալները։

   ---
   
   #### Օրինակ՝ Axios-ի Օգտագործում
   
   ```javascript
   import axios from 'axios';
   
   axios.get('https://jsonplaceholder.typicode.com/posts')
     .then(response => {
       console.log(response.data);
     })
     .catch(error => {
       console.error('Error:', error);
     });
   ```

   ---
   
   #### Fetch API
   
   **Fetch API**-ն ներկառուցված մեթոդ է, որը ապահովում է HTTP հարցումներ կատարելու հզոր և ճկուն միջոց։ Այն հիմնված է Promise-ների վրա և աշխատում է ինչպես ֆրոնտենդում, այնպես էլ Node.js-ում՝ որոշ լրացուցիչ գրադարանների միջոցով։
   
   #### Հիմնական Հատկանիշներ
   
   1. **Promise-ների վրա հիմնված**:
      - Ապահովում է `.then` և `.catch` սինտաքս։
   
   2. **Կառուցված JavaScript-ում**:
      - Չկա կարիք լրացուցիչ գրադարան ներբեռնելու։
   
   3. **Անհրաժեշտ է JSON վերամշակում**:
      - Պատասխանները JSON օբյեկտի վերածելու համար անհրաժեշտ է կիրառել `.json()` մեթոդը։
   
   4. **HTTP մեթոդների աջակցություն:**
      - Աջակցում է GET, POST, PUT, DELETE և այլ մեթոդներին։
   
   5. **Timeout-ի անմիջական աջակցություն չկա**:
      - Timeout սահմանելու համար անհրաժեշտ է լրացուցիչ տրամաբանություն։
   
   ---
   
   #### Օրինակ՝ Fetch API-ի Օգտագործում
   
   ```javascript
   fetch('https://jsonplaceholder.typicode.com/posts')
     .then(response => {
       if (!response.ok) {
         throw new Error('Network response was not ok');
       }
       return response.json();
     })
     .then(data => console.log(data))
     .catch(error => console.error('Error:', error));
   ```

   ---
   
   #### Axios vs Fetch API
   
   | **Հատկանիշ**                | **Axios**                                   | **Fetch API**                             |
   |-----------------------------|--------------------------------------------|-------------------------------------------|
   | **Աջակցություն**             | Պահանջում է գրադարանի ներբեռնում            | Կառուցված է JavaScript-ում                 |
   | **JSON վերամշակում**         | Ավտոմատ                                    | Պահանջում է `.json()`-ի կիրառություն       |
   | **Timeout աջակցություն**     | Ներկառուցված                               | Պահանջում է լրացուցիչ տրամաբանություն       |
   | **Խնդիրների կառավարում**     | Աջակցում է Interceptors-ի միջոցով           | Առկա չէ                                   |
   | **Խաչաձև-պլատֆորմայնություն**| Աջակցվում է բրաուզերում և Node.js-ում        | Աշխատում է միայն բրաուզերում               |
   | **Հեշտ օգտագործում**         | Ավելի պարզ և կառուցվածքային                | Ավելի քիչ ֆունկցիոնալ, բայց պարզ           |

   ---
   
   #### Եզրակացություն
   
   - Օգտագործեք **Axios**, երբ անհրաժեշտ է ավելի հզոր ֆունկցիոնալություն, ինչպիսին են Interceptors-ը, ավտոմատ JSON վերամշակումը, և timeout-ի կառավարումը։
   
   - Օգտագործեք **Fetch API**, երբ ցանկանում եք օգտագործել JavaScript-ի ներկառուցված գործիքակազմը կամ պետք է նվազեցնել հավելվածի կախվածությունը գրադարաններից։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

63. ### Ինչ է JavaScript-ում Modules-ը?
   
   **Modules**-ը JavaScript-ում կոդի կազմակերպման և վերահսկելիության մեխանիզմ է, որը թույլ է տալիս բաժանել կոդը ավելի փոքր, անկախ միավորների։ Դրանք ապահովում են կոդի վերօգտագործման, ընթեռնելիության և կառավարման հեշտություն, ինչը հատկապես կարևոր է մեծ նախագծերում։
   
   JavaScript-ի մոդուլները հաճախ օգտագործվում են ֆայլերի տեսքով, որտեղ յուրաքանչյուր ֆայլ կարող է պարունակել իր սեփական փոփոխականները, ֆունկցիաները և օբյեկտները։

   ---
   
   #### Ինչու օգտագործել Modules?
   
   1. **Կոդի բաժանում (Modularity):**
      - Կոդը բաժանվում է փոքր, կառավարելի հատվածների։
   
   2. **Կրկնօրինակման նվազեցում:**
      - Նվազեցնում է կրկնօրինակվող կոդը՝ հեշտացնելով վերօգտագործումը։
   
   3. **Սխալների կառավարում:**
      - Ավելի հեշտ է հայտնաբերել և շտկել սխալները։
   
   4. **Նախագծի մասշտաբայնացում:**
      - Հնարավորություն է տալիս աշխատել մեծ նախագծերի վրա՝ առանց կոդի խառնաշփոթ առաջացնելու։
   
   5. **Անվտանգություն:**
      - Փոփոխականներն ու ֆունկցիաները կարելի է սահմանափակել միայն մոդուլի սահմաններում։

   ---
   
   #### Մոդուլների Տիպերը
   
   #### 1. **ES Modules (ESM)**
   ES6-ում ներկայացված մոդուլային համակարգը։ Ֆայլերը դիտվում են որպես մոդուլներ, և դրանց օգտագործման համար կիրառվում են `import` և `export` բանալի բառերը։
   
   #### Օրինակներ
   
   #### Ֆունկցիայի Արտահանում և Ներմուծում
   
   **`math.js`** ֆայլ:
   ```javascript
   export function add(a, b) {
     return a + b;
   }
   
   export function subtract(a, b) {
     return a - b;
   }
   ```
   
   **`app.js`** ֆայլ:
   ```javascript
   import { add, subtract } from './math.js';
   
   console.log(add(5, 3));      // Output: 8
   console.log(subtract(5, 3)); // Output: 2
   ```
   
   #### Արտահանում Ընդհանուր
   
   **`utils.js`** ֆայլ:
   ```javascript
   function greet(name) {
     return `Hello, ${name}!`;
   }
   
   export default greet;
   ```
   
   **`app.js`** ֆայլ:
   ```javascript
   import greet from './utils.js';
   
   console.log(greet('Alice')); // Output: Hello, Alice!
   ```

   ---
   
   #### 2. **CommonJS (CJS)**
   CommonJS-ը մոդուլային համակարգ է, որը հիմնականում օգտագործվում է Node.js-ում։ Մոդուլները ներմուծվում են `require` մեթոդով և արտահանվում `module.exports` կամ `exports` օբյեկտի միջոցով։
   
   #### Օրինակ
   
   **`math.js`** ֆայլ:
   ```javascript
   function add(a, b) {
     return a + b;
   }
   
   function subtract(a, b) {
     return a - b;
   }
   
   module.exports = { add, subtract };
   ```
   
   **`app.js`** ֆայլ:
   ```javascript
   const { add, subtract } = require('./math');
   
   console.log(add(5, 3));      // Output: 8
   console.log(subtract(5, 3)); // Output: 2
   ```

   ---
   
   #### ES Modules vs CommonJS
   
   | **Հատկանիշ**        | **ES Modules**                       | **CommonJS**                        |
   |---------------------|-------------------------------------|-------------------------------------|
   | **Բանալի բառեր**    | `import`, `export`                  | `require`, `module.exports`        |
   | **Աջակցություն**     | Բրաուզեր և Node.js                 | Հիմնականում Node.js                |
   | **Dynamic Imports** | Աջակցվում է (`import()` սինտաքս)     | Մասամբ աջակցվում է                  |
   | **Performance**     | Ավելի արդյունավետ՝ բրաուզերներում    | Ավելի հարմար՝ սերվերային ծրագրերում |
   
   ---
   
   #### Մոդուլների Օգտագործման Բացառիկ Դեպքեր
   
   1. **Dynamic Imports**:
      - Մոդուլները կարելի է ներմուծել դինամիկ կերպով՝ անհրաժեշտ պահին։
   
    ```javascript
      if (condition) {
       import('./math.js').then(module => {
       console.log(module.add(5, 3));
       });
      }
      ```
   
   2. **Lazy Loading**:
      - Ներմուծեք մոդուլները միայն այն դեպքում, երբ դրանք անհրաժեշտ են, ինչը բարձրացնում է հավելվածի կատարողականությունը։
   
   3. **Tree Shaking**:
      - ES Modules-ը թույլ է տալիս հեռացնել չօգտագործվող կոդը (dead code elimination)։
   
   ---
   
   #### Երբ օգտագործել Modules
   
   - **Կոդի կառավարման համար**:
      - Երբ աշխատում եք մեծ նախագծի վրա և ցանկանում եք պահել կոդը կազմակերպված։
   
   - **Կրկնակի օգտագործվող կոմպոնենտներ ստեղծելու համար**:
      - Օրինակ՝ UI կոմպոնենտներ, օգտակար ֆունկցիաներ և այլն։
   
   - **Պատասխանատվությունների հստակ բաժանման համար**:
      - Տարբեր ֆայլերում պահեք բիզնես տրամաբանությունը, տվյալների մոդելը և UI կոմպոնենտները։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---
64. ### Ինչ է WebSockets-ը JavaScript-ում?
   
   **WebSockets**-ը հաղորդակցության պրոտոկոլ է, որը թույլ է տալիս երկկողմանի (bidirectional) և իրական ժամանակում տվյալների փոխանակում սերվերի և հաճախորդի միջև։ WebSockets-ը ապահովում է ավելի արդյունավետ տվյալների փոխանակում՝ համեմատած ավանդական HTTP հարցումների հետ, ինչը դարձնում է այն իդեալական իրական ժամանակում տվյալների վրա հիմնված հավելվածների համար։
   
   JavaScript-ում WebSockets-ը կարող է օգտագործվել `WebSocket` API-ի միջոցով։ Այն ապահովում է մշտական կապ, որտեղ սերվերն ու հաճախորդը կարող են տվյալներ ուղարկել և ստանալ ցանկացած պահի։
   
   ---
   
   ## Ինչպես է աշխատում WebSockets-ը
   
   1. Սկզբում հաստատվում է HTTP կապ, որը "զինվում" է WebSocket կապի։
   2. HTTP կապը թարմացվում է WebSocket կապի՝ օգտագործելով "Upgrade" HTTP վերնագիրը։
   3. Կապը հաստատելուց հետո երկու կողմերն էլ կարող են ուղարկել տվյալներ առանց հավելյալ HTTP հարցման։

   ---
   
   #### WebSocket API-ի Օգտագործումը JavaScript-ում
   
   #### Սինտաքս
   ```javascript
   const socket = new WebSocket(url);
   ```
   
   - **`url`**: WebSocket սերվերի URL-ը (օրինակ՝ `ws://example.com` կամ `wss://example.com` `wss`-ը նշանակում է անվտանգ կապ)։
   
   #### Օրինակ
   ```javascript
   // Ստեղծում ենք WebSocket կապ
   const socket = new WebSocket('wss://example.com/socket');
   
   // Կապի բացում
   socket.onopen = function(event) {
     console.log('Connection opened:', event);
     socket.send('Hello Server!');
   };
   
   // Տվյալների ստացում
   socket.onmessage = function(event) {
     console.log('Message from server:', event.data);
   };
   
   // Սխալների կառավարում
   socket.onerror = function(event) {
     console.error('WebSocket error:', event);
   };
   
   // Կապի փակման կառավարում
   socket.onclose = function(event) {
     console.log('Connection closed:', event);
   };
   ```

   ---
   
   #### WebSockets-ի Առավելությունները
   
   1. **Երկկողմանի հաղորդակցություն**:
      - Թույլ է տալիս ինչպես սերվերին, այնպես էլ հաճախորդին սկսել հաղորդակցություն։
   
   2. **Իրական ժամանակում տվյալների թարմացում**:
      - Հարմար է չաթ հավելվածների, խաղերի, վիճակագրական վահանակների և իրական ժամանակում գործարկվող հավելվածների համար։
   
   3. **Ավելի քիչ չափի փոխանցում**:
      - WebSocket կապը մշտական է, և յուրաքանչյուր հաղորդագրություն չի պահանջում HTTP վերնագրեր, ինչը խնայում է ռեսուրսները։
   
   4. **Արագություն**:
      - Մինչև 10x արագ է ավանդական HTTP հարցումների համեմատ՝ շնորհիվ մշտական կապի։
   
   ---
   
   #### WebSockets-ի Թերությունները
   
   1. **Աջակցություն զննարկիչներում**:
      - Չնայած ժամանակակից զննարկիչների մեծ մասը աջակցում է WebSockets-ին, հին զննարկիչները կարող են չունենալ աջակցություն։
   
   2. **Բարդություն**:
      - Արձանագրությունը ավելի բարդ է՝ համեմատած HTTP-ի հետ։
   
   3. **Հոսքային սխալների կառավարում**:
      - Եթե կապը ընդհատվում է, անհրաժեշտ է տրամադրել լրացուցիչ տրամաբանություն՝ կրկին կապ հաստատելու համար։
   
   ---
   
   #### WebSockets-ի Օգտագործման Տարբեր Դեպքեր
   
   1. **Չաթ հավելվածներ**
      - Օրինակ՝ WhatsApp-ի կամ Slack-ի իրական ժամանակում հաղորդագրությունների փոխանցում։
   
   2. **Վիճակագրական վահանակներ**
      - Իրական ժամանակում տվյալների թարմացում և վիզուալիզացիա։
   
   3. **Գործարքային համակարգեր**
      - Օրինակ՝ բորսայական գների կամ կրիպտոարժույթների իրական ժամանակում թարմացում։
   
   4. **Մուլտիպլեյեր խաղեր**
      - Տվյալների արագ և երկկողմանի փոխանակում խաղացողների միջև։
   
   ---
   
   #### WebSockets-ի և HTTP-ի Համեմատություն
   
   | **Հատկանիշ**               | **WebSockets**                      | **HTTP**                              |
   |-----------------------------|--------------------------------------|---------------------------------------|
   | **Կապի Տիպ**               | Մշտական                            | Պահանջ-պատասխան                     |
   | **Տվյալների Փոխանակում**    | Երկկողմանի                         | Միակողմանի (հաճախորդից սերվեր)      |
   | **Օգտագործման Դեպքեր**      | Իրական ժամանակում հաղորդակցություն  | Ավանդական վեբ հարցումներ            |
   | **Կատարողականություն**      | Ավելի արագ և արդյունավետ           | Ավելի դանդաղ                         |

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---
65. ### Ինչ է DOM Traversing-ը JavaScript-ում?
   
   **DOM Traversing**-ը JavaScript-ում գործընթաց է, որը թույլ է տալիս մուտք գործել և փոխազդել HTML փաստաթղթի տարբեր տարրերի հետ։ Այս գործընթացի ընթացքում մենք անցնում ենք DOM ծառի միջոցով՝ ընտրելով ծնողական, զավակային, հարևան և այլ տարրեր։
   
   DOM Traversing-ը կարևոր է, քանի որ այն թույլ է տալիս դինամիկ կերպով կառավարել էջի բովանդակությունը՝ հավելելով, հեռացնելով կամ փոփոխելով տարրերը։

   ---
   
   #### Ինչպես է աշխատում DOM Traversing-ը
   
   DOM Traversing-ը հիմնված է DOM ծառի վրա, որը կառուցվում է HTML փաստաթղթի հիման վրա։ Այս ծառը բաղկացած է տարրերից (nodes), և յուրաքանչյուր տարր կարող է ունենալ ծնողներ, զավակներ կամ հարևաններ։
   
   DOM Traversing-ը իրականացնում ենք DOM API-ի միջոցով՝ օգտագործելով տարբեր մեթոդներ և հատկություններ։
   
   ---
   
   #### Հիմնական Հատկություններ և Մեթոդներ
   
   #### 1. Ծնողական տարրերի հասանելիություն
   
   | **Մեթոդ/Հատկություն** | **Նկարագրություն**                     |
   |------------------------|----------------------------------------|
   | `parentNode`           | Վերադարձնում է ընթացիկ տարրի ծնողը։     |
   | `parentElement`        | Վերադարձնում է ընթացիկ տարրի ծնող տարրը։|
   
   #### Օրինակ
   ```javascript
   const child = document.querySelector('.child');
   console.log(child.parentNode);    // Վերադարձնում է ծնողը։
   console.log(child.parentElement); // Վերադարձնում է ծնող տարրը։
   ```
   
   ---
   
   #### 2. Զավակային տարրերի հասանելիություն
   
   | **Մեթոդ/Հատկություն** | **Նկարագրություն**                                   |
   |------------------------|----------------------------------------------------|
   | `childNodes`           | Վերադարձնում է ընթացիկ տարրի բոլոր զավակների NodeList։|
   | `children`             | Վերադարձնում է միայն զավակ տարրերի HTMLCollection։  |
   | `firstChild`           | Վերադարձնում է առաջին զավակ Node-ը։                |
   | `lastChild`            | Վերադարձնում է վերջին զավակ Node-ը։                |
   | `firstElementChild`    | Վերադարձնում է առաջին զավակ տարրը։                 |
   | `lastElementChild`     | Վերադարձնում է վերջին զավակ տարրը։                 |
   
   #### Օրինակ
   ```javascript
   const parent = document.querySelector('.parent');
   console.log(parent.children);            // Վերադարձնում է միայն տարրերը։
   console.log(parent.firstElementChild);  // Առաջին զավակ տարրը։
   console.log(parent.lastElementChild);   // Վերջին զավակ տարրը։
   ```
   
   ---
   
   #### 3. Հարևան տարրերի հասանելիություն
   
   | **Մեթոդ/Հատկություն** | **Նկարագրություն**                                |
   |------------------------|-------------------------------------------------|
   | `nextSibling`          | Վերադարձնում է հաջորդ Node-ը։                   |
   | `previousSibling`      | Վերադարձնում է նախորդ Node-ը։                   |
   | `nextElementSibling`   | Վերադարձնում է հաջորդ տարրը։                    |
   | `previousElementSibling` | Վերադարձնում է նախորդ տարրը։                   |
   
   #### Օրինակ
   ```javascript
   const item = document.querySelector('.item');
   console.log(item.nextElementSibling);  // Հաջորդ տարրը։
   console.log(item.previousElementSibling); // Նախորդ տարրը։
   ```
   
   ---
   
   #### 4. Տվյալ տարրի հետ աշխատելու մեթոդներ
   
   | **Մեթոդ**                 | **Նկարագրություն**                                     |
   |---------------------------|------------------------------------------------------|
   | `querySelector(selector)` | Ընտրում է առաջին հանդիպած տարրը՝ ըստ սելեկտորի։       |
   | `querySelectorAll(selector)` | Ընտրում է բոլոր տարրերը՝ ըստ սելեկտորի։              |
   | `getElementById(id)`      | Ընտրում է տարրը ըստ ID-ի։                             |
   | `getElementsByClassName(className)` | Ընտրում է բոլոր տարրերը ըստ դասի։                |
   | `getElementsByTagName(tagName)`    | Ընտրում է բոլոր տարրերը ըստ պիտակի։               |
   
   #### Օրինակ
   ```javascript
   const items = document.querySelectorAll('.list-item');
   items.forEach(item => console.log(item.textContent));
   ```

   ---
   
   #### Երբ օգտագործել DOM Traversing
   
   1. **Դինամիկ բովանդակություն ավելացնելու համար**
      - Օրինակ՝ ցուցակին նոր տարրեր ավելացնելու համար։
   
   2. **Տարրերի փոփոխություն**
      - Օրինակ՝ ստիլների փոփոխություն կամ տվյալների թարմացում։
   
   3. **Տարրերի հեռացում**
      - Օրինակ՝ թաքցնել կամ ջնջել կոնկրետ տարրը։
   
   ---
   
   #### Առավելություններ
   
   1. Թույլ է տալիս աշխատել ամբողջ DOM ծառի հետ։
   2. Հեշտացնում է բարդ HTML փաստաթղթերի կառավարումը։
   3. Աջակցում է տարբեր մեթոդների միջոցով տարրերի արագ հասանելիությանը։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---
66. ### Ինչ է Custom Events-ը JavaScript-ում?

   **Custom Events**-ը JavaScript-ում թույլ է տալիս ծրագրավորողներին ստեղծել և օգտագործել իրադարձություններ, որոնք նախատեսված չեն ըստ լռելյայն (built-in)։ Դրանք հարմար են վեբ հավելվածների համար, որտեղ անհրաժեշտ է հաղորդակցություն տարբեր տարրերի կամ մոդուլների միջև՝ օգտագործելով իրադարձություններ։
   
   Custom Events-ը ստեղծվում է `CustomEvent` դասի միջոցով և կարող է ներառել լրացուցիչ տվյալներ `detail` հատկության միջոցով։

   ---
   
   #### Ինչպես ստեղծել Custom Event
   
   Custom Event ստեղծելու համար օգտագործվում է `CustomEvent` կոնստրուկտորը։
   
   #### Սինտաքս
   ```javascript
   const event = new CustomEvent(eventName, options);
   ```
   - **`eventName`**: Իրադարձության անունը։
   - **`options`** (ոչ պարտադիր): Օբյեկտ, որը կարող է ներառել հետևյալ հատկությունները.
      - `detail`: Պահում է լրացուցիչ տվյալներ իրադարձության մասին։
      - `bubbles`: Boolean, որը ցույց է տալիս՝ իրադարձությունը "բարձրանում" է DOM ծառով (default՝ `false`)։
      - `cancelable`: Boolean, որը թույլ է տալիս իրադարձությունը չեղարկել (default՝ `false`)։

   ---
   
   #### Օրինակներ
   
   #### Հիմնական Օրինակ
   ```javascript
   // Ստեղծում ենք Custom Event
   const customEvent = new CustomEvent('myCustomEvent', {
     detail: { message: 'Hello, World!' },
     bubbles: true,
     cancelable: true
   });
   
   // Ավելացնում ենք իրադարձության լսող
   document.addEventListener('myCustomEvent', (event) => {
     console.log('Custom Event Triggered:', event.detail.message);
   });
   
   // Թողարկում ենք իրադարձությունը
   document.dispatchEvent(customEvent);
   ```
   **Output**: `Custom Event Triggered: Hello, World!`
   
   ---
   
   #### Իրադարձության չեղարկում
   
   ```javascript
   const customEvent = new CustomEvent('cancelableEvent', {
     cancelable: true
   });
   
   document.addEventListener('cancelableEvent', (event) => {
     console.log('Event received, canceling...');
     event.preventDefault();
   });
   
   const result = document.dispatchEvent(customEvent);
   
   if (!result) {
     console.log('The event was canceled.');
   }
   ```
   **Output**:
   - `Event received, canceling...`
   - `The event was canceled.`
   
   ---
   
   #### Լրացուցիչ տվյալների փոխանցում
   
   ```javascript
   const button = document.querySelector('button');
   
   button.addEventListener('customClick', (event) => {
     console.log('Button clicked with data:', event.detail);
   });
   
   const customClickEvent = new CustomEvent('customClick', {
     detail: { clickedAt: new Date() }
   });
   
   button.dispatchEvent(customClickEvent);
   ```
   
   **Output**:
   - `Button clicked with data: { clickedAt: '2024-12-22T12:00:00.000Z' }`

   ---
   
   #### Custom Events-ի Առավելությունները
   
   1. **Մոդուլների հաղորդակցություն**
      - Օգտակար է մեծ նախագծերում, որտեղ տարբեր մոդուլներ պետք է հաղորդակցվեն։
   
   2. **Դինամիկ հաղորդակցություն**
      - Հեշտացնում է տվյալների փոխանցումը տարբեր տարրերի միջև։
   
   3. **Լրացուցիչ տվյալների փոխանցում**
      - `detail` հատկության միջոցով կարող եք փոխանցել ցանկացած տվյալ։
   
   4. **Աջակցություն DOM-ի հետ**
      - Custom Events-ը ինտեգրվում է DOM-ի հետ, և դուք կարող եք օգտագործել այն նույն կերպ, ինչպես լռելյայն իրադարձությունները։
   
   ---
   
   #### Custom Events-ի Թերությունները
   
   1. **Բարդություն**
      - Ավելի բարդ է՝ համեմատած լռելյայն իրադարձությունների հետ։
   
   2. **Բրաուզերի աջակցություն**
      - Հին բրաուզերներում (օրինակ՝ IE 11) անհրաժեշտ է Polyfill։
   
   ---
   
   #### Երբ օգտագործել Custom Events
   
   1. **Հատուկ գործողություններ ավելացնելու համար**
      - Օրինակ՝ հավելվածի ներսում կոնկրետ իրադարձություն մոդելի վրա ազդելու համար։
   
   2. **Մոդուլների ինտեգրացիա**
      - Երբ ձեր հավելվածը բաղկացած է մոդուլներից, և դրանք պետք է համագործակցեն։
   
   3. **Դինամիկ ինտերֆեյսներ**
      - Երբ անհրաժեշտ է թարմացնել UI տարրերը հատուկ գործողությունների հիման վրա։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---
67. ### Ինչ է Shadow DOM-ը JavaScript-ում?
   
   **Shadow DOM**-ը JavaScript-ում տեխնոլոգիա է, որը թույլ է տալիս ստեղծել մեկուսացված DOM ծառ՝ զերծ մնալով գլոբալ ոճերի կամ սկրիպտերի ազդեցությունից։ Այն օգտագործվում է Web Components-ի (վեբ կոմպոնենտներ) հետ միասին՝ ինտերակտիվ և վերօգտագործվող UI բաղադրիչներ ստեղծելու համար։
   
   Shadow DOM-ը տալիս է **local scope**, ինչը նշանակում է, որ տարրի ներսում գտնվող ոճերը կամ կառուցվածքը չեն ազդում արտաքին տարրերի վրա և հակառակը։

   ---
   
   #### Ինչպես է աշխատում Shadow DOM-ը
   
   1. Ստեղծվում է **Shadow Root**, որը ծառայում է որպես տարրի մեկուսացված DOM ծառի հիմք։
   2. Այս ծառի ներսում կարող եք ավելացնել HTML և CSS, որոնք տեսանելի չեն գլխավոր (main) DOM-ին։
   
   ---
   
   #### Ինչու օգտագործել Shadow DOM
   
   1. **Մեկուսացում**
      - Ստեղծում է մեկուսացված միջավայր՝ կանխելով ոճերի և սկրիպտերի բախումները։
   
   2. **Վերօգտագործում**
      - Թույլ է տալիս ստեղծել վերօգտագործվող և անկախ կոմպոնենտներ։
   
   3. **Կատարողականություն**
      - Shadow DOM-ը կարող է բարելավել կատարողականությունը՝ նվազեցնելով DOM-ի չափը և ոճերի վերաշարադրումը (repaint)։
   
   4. **Կառավարման պարզություն**
      - Ապահովում է local scope, ինչը դարձնում է կոմպոնենտները ավելի հեշտ կառավարելի։
   
   ---
   
   #### Ինչպես ստեղծել Shadow DOM
   
   #### Օրինակ՝ Shadow Root ստեղծում
   ```javascript
   // Ստեղծում ենք տարր
   const host = document.createElement('div');
   document.body.appendChild(host);
   
   // Ստեղծում ենք Shadow Root
   const shadowRoot = host.attachShadow({ mode: 'open' });
   
   // Ավելացնում ենք պարունակություն Shadow DOM-ի մեջ
   shadowRoot.innerHTML = `
     <style>
       p {
         color: red;
       }
     </style>
     <p>This is inside Shadow DOM</p>
   `;
   ```
   
   - **`attachShadow` մեթոդը**:
   - Ստեղծում է Shadow Root։
   - Ընդունում է օբյեկտ, որը պարունակում է `mode` հատկությունը (`open` կամ `closed`)։
   
   ---
   
   #### Shadow DOM-ի Mode-երը
   
   1. **Open Mode**:
      - Shadow Root-ը հասանելի է JavaScript-ով `shadowRoot` հատկության միջոցով։
   
   2. **Closed Mode**:
      - Shadow Root-ը անհասանելի է JavaScript-ով։ Օրինակ՝
      ```javascript
      const shadowRoot = host.attachShadow({ mode: 'closed' });
      console.log(host.shadowRoot); // Output: null
      ```
   
   ---
   
   #### Օրինակ՝ Ստեղծում ենք Custom Element Shadow DOM-ով
   
   ```javascript
   class MyElement extends HTMLElement {
     constructor() {
       super();
       const shadow = this.attachShadow({ mode: 'open' });
   
       shadow.innerHTML = `
         <style>
           h1 {
             color: blue;
           }
         </style>
         <h1>Shadow DOM Example</h1>
       `;
     }
   }
   
   customElements.define('my-element', MyElement);
   
   // Օգտագործում ենք Custom Element-ը
   const element = document.createElement('my-element');
   document.body.appendChild(element);
   ```


---
   
   #### Shadow DOM-ի Առավելությունները
   
   1. **Մեկուսացված ոճեր**:
      - Թույլ է տալիս սահմանել կոմպոնենտի համար հատուկ ոճեր՝ առանց ազդեցության այլ տարրերի վրա։
   
   2. **Ոճերի բախման կանխում**:
      - Վերացնում է գլոբալ CSS-ի և կոմպոնենտի միջև ոճերի բախման խնդիրները։
   
   3. **Վերօգտագործելիություն**:
      - Shadow DOM-ը կատարյալ է վերօգտագործվող և դինամիկ UI կոմպոնենտների համար։

   ---
   
   #### Shadow DOM-ի Թերությունները
   
   1. **Բարդություն**:
      - Shadow DOM-ի ներդրումը կարող է ավելացնել հավելվածի բարդությունը։
   
   2. **Համատեղելիություն**:
      - Հին զննարկիչները (օրինակ՝ IE11) չեն աջակցում Shadow DOM-ին։
   
   3. **Դեբագինգի դժվարություն**:
      - Մեկուսացված կառուցվածքը կարող է բարդացնել սխալների հայտնաբերումը։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---
68. ### Ինչ է JavaScript-ում polyfill-ը?
   

   **Polyfill**-ը JavaScript-ում կոդ է (հաճախ՝ գրադարան կամ ֆունկցիա), որը ապահովում է հին զննարկիչների կամ պլատֆորմների աջակցությունը ժամանակակից ֆունկցիոնալությանը, որը նրանք ի սկզբանե չեն սատարում։ Այն "լրացնում" է բաց թողնված ֆունկցիոնալությունը՝ ապահովելով համատեղելիություն ժամանակակից JavaScript հնարավորությունների և հին միջավայրերի միջև։

---
   
   #### Ինչու է անհրաժեշտ Polyfill-ը?
   
   1. **Համատեղելիություն**:
      - Հին զննարկիչները (օրինակ՝ IE11) չեն աջակցում JavaScript-ի նոր ֆունկցիաներին, ինչպիսիք են `Promise`, `fetch`, կամ `Array.prototype.includes`։ Polyfill-ները լուծում են այս խնդիրը։
   
   2. **Ստանդարտների առաջընթաց**:
      - ECMAScript (JavaScript-ի ստանդարտ) նոր հնարավորությունները հաճախ ավելացվում են։ Polyfill-ները թույլ են տալիս օգտվել այդ հնարավորություններից, նույնիսկ եթե զննարկիչները դեռ չեն աջակցում դրանց։
   
   3. **Օգտագործողի փորձի բարելավում**:
      - Ապահովում է, որ ձեր վեբ հավելվածը ճիշտ աշխատի բոլոր օգտատերերի համար՝ անկախ նրանց օգտագործած զննարկիչից։
   
   ---
   
   #### Ինչպես է աշխատում Polyfill-ը?
   
   Polyfill-ը ստուգում է, արդյոք տվյալ ֆունկցիան կամ հատկությունը առկա է։ Եթե ոչ, այն ավելացնում է այդ ֆունկցիան կամ հատկությունը։
   
   #### Օրինակ՝ Polyfill `Array.prototype.includes`-ի Համար
   
   ```javascript
   if (!Array.prototype.includes) {
     Array.prototype.includes = function(element, start) {
       if (start === undefined) {
         start = 0;
       }
   
       for (let i = start; i < this.length; i++) {
         if (this[i] === element) {
           return true;
         }
       }
   
       return false;
     };
   }
   
   // Օգտագործում ենք polyfill-ը
   const array = [1, 2, 3];
   console.log(array.includes(2)); // true
   console.log(array.includes(5)); // false
   ```

   ---
   
   #### Տարբերություն Polyfill-ի և Shim-ի միջև
   
   | **Հատկանիշ**             | **Polyfill**                                  | **Shim**                                     |
   |---------------------------|-----------------------------------------------|---------------------------------------------|
   | **Նպատակ**               | Ապահովում է նոր API-ի կամ ֆունկցիայի աջակցություն։| Վերագրում է կամ ընդլայնում է առկա ֆունկցիոնալությունը։|
   | **Անվտանգություն**        | Չի փոխում JavaScript-ի լռելյայն վարքագիծը։   | Կարող է փոխել լռելյայն վարքագիծը։           |
   | **Օրինակ**                | `Array.prototype.includes`-ի polyfill։       | `bind` ֆունկցիայի shim։                     |

   ---
   
   #### Հաճախ Օգտագործվող Polyfill-ներ
   
   1. **`Promise`**
      - Աջակցություն ասինխրոն գործողությունների համար։
      ```javascript
      if (!window.Promise) {
        // Ձեր polyfill-ը...
      }
      ```
   
   2. **`fetch`**
      - HTTP հարցումներ կատարելու ժամանակակից API։
      ```javascript
      if (!window.fetch) {
        // Ավելացրեք fetch polyfill-ը։
      }
      ```
   
   3. **`Object.assign`**
      - Օբյեկտների հատկությունների պատճենում։
   
   4. **`Array.from`**
      - Պատրաստում է զանգված `array-like` օբյեկտից։
   
   5. **`Intl` (Internationalization API)**
      - Թույլ է տալիս թվերի, ամսաթվերի և լեզվական ձևաչափերի աջակցություն։
   
   ---
   
   #### Polyfill-ի Օգտագործման Մեթոդներ
   
   1. **CDN-ի Օգտագործում**:
      - Կարող եք ներբեռնել հայտնի polyfill-ներ, ինչպիսիք են `polyfill.io`-ն:
      ```html
      <script src="https://polyfill.io/v3/polyfill.min.js"></script>
      ```
   
   2. **Գրադարաններ**:
      - Օգտագործեք գրադարաններ, ինչպիսիք են Babel-ը կամ Core-JS-ը, որոնք ապահովում են polyfill-ներ։
      ```bash
      npm install core-js
      ```
   
   3. **Սեփական Polyfill-ներ Ստեղծել**:
      - Պահանջվող ֆունկցիոնալությունը կարող եք իրագործել ինքնուրույն՝ կիրառելով JavaScript։
   
   ---
   
   #### Երբ չօգտագործել Polyfill
   
   1. **Փոքր թիրախային լսարան**:
      - Եթե ձեր լսարանը հիմնականում օգտագործում է ժամանակակից զննարկիչներ։
   
   2. **Կատարողականության խնդիրներ**:
      - Polyfill-ները կարող են մեծացնել բեռի չափը և ազդել կատարողականության վրա։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---
69. ### Ինչ է Event Loop-ի և Call Stack-ի միջև կապը JavaScript-ում?
   
   JavaScript-ը միապրոցես (single-threaded) լեզու է, ինչը նշանակում է, որ այն կատարում է կոդը մեկ հոսքով՝ օգտագործելով **Call Stack**։ Սակայն JavaScript-ը կարող է նաև աշխատել ասինխրոն գործողությունների հետ՝ օգտագործելով **Event Loop**-ը։
   
   Event Loop-ը և Call Stack-ը JavaScript-ի հիմնական մեխանիզմներն են, որոնք ապահովում են կոդի ճիշտ կատարումը՝ հատկապես ասինխրոն գործողությունների դեպքում։

---
   
   #### Ինչ է Call Stack-ը?
   
   **Call Stack**-ը մեխանիզմ է, որը հետևում է ակտիվ ֆունկցիաների կանչերին։ Այն JavaScript-ի **լինեար** (linear) կառուցվածքն է, որտեղ ֆունկցիաները ավելացվում և հանվում են ֆունկցիաների կոդի կատարման ժամանակ։
   
   - **Push:** Ֆունկցիան ավելացվում է Call Stack-ի վրա, երբ այն կանչվում է։
   - **Pop:** Ֆունկցիան հանվում է Call Stack-ից, երբ այն ավարտում է իր կատարման գործընթացը։
   
   #### Օրինակ
   ```javascript
   function first() {
     second();
   }
   
   function second() {
     console.log('Hello, Event Loop!');
   }
   
   first();
   ```
   
   **Call Stack-ի քայլերը:**
   1. `first()` ֆունկցիան ավելացվում է Stack-ին։
   2. `second()` ֆունկցիան ավելացվում է Stack-ին։
   3. `console.log()`-ը կատարվում է և հանվում Stack-ից։
   4. `second()` հանվում է Stack-ից։
   5. `first()` հանվում է Stack-ից։

   ---
   
   #### Ինչ է Event Loop-ը?
   
   **Event Loop**-ը JavaScript-ի հիմնական մեխանիզմն է, որը կառավարում է ասինխրոն գործողությունների կատարման հերթականությունը։ Այն ապահովում է, որ Call Stack-ը մաքրվի, և կոդի մնացած ասինխրոն գործողությունները կատարվեն ճիշտ հերթականությամբ։
   
   #### Event Loop-ի քայլերը
   1. Ստուգում է՝ արդյոք Call Stack-ը դատարկ է։
   2. Եթե դատարկ է, Event Loop-ը հերթից (Queue) տեղափոխում է միկրոգործողությունները (Microtasks) և մակրոգործողությունները (Macrotasks) Call Stack։
   3. Կրկնում է գործընթացը։

   ---
   
   #### Call Stack-ի և Event Loop-ի Համագործակցությունը
   
   #### 1. Սինխրոն գործողություններ
   Սկզբնական կոդի կատարման ժամանակ բոլոր սինխրոն գործողությունները կատարում են Call Stack-ը։
   
   ```javascript
   console.log('First');
   console.log('Second');
   ```
   **Output:**
   ```
   First
   Second
   ```
   
   **Պարզապես Call Stack է օգտագործվում։**
   
   #### 2. Ասինխրոն գործողություններ
   
   Ասինխրոն գործողությունները (օրինակ՝ `setTimeout`, `fetch`) նախ ուղարկվում են Web API-ներին, և դրանց արդյունքը պահվում է Task Queue-ում կամ Microtask Queue-ում։ Event Loop-ը ստուգում է Call Stack-ը և դատարկության դեպքում ավելացնում դրանք Stack-ում։
   
   #### Օրինակ
   ```javascript
   console.log('Start');
   
   setTimeout(() => {
     console.log('Timeout');
   }, 0);
   
   console.log('End');
   ```
   
   **Output:**
   ```
   Start
   End
   Timeout
   ```
   
   **Քայլերի բացատրություն:**
   1. `console.log('Start')` կատարվում է անմիջապես։
   2. `setTimeout`-ը ուղարկվում է Web API-ին։
   3. `console.log('End')` կատարվում է անմիջապես։
   4. Event Loop-ը տեղադրում է `Timeout` callback-ը Call Stack-ում։

   ---
   
   #### Microtasks vs Macrotasks
   
   Event Loop-ը կառավարում է միկրոգործողություններն ու մակրոգործողությունները տարբեր հերթերում։
   
   - **Microtasks (Միկրոգործողություններ):**
      - Promise callbacks, `queueMicrotask()`
      - Ավելի բարձր առաջնահերթություն ունեն։
   
   - **Macrotasks (Մակրոգործողություններ):**
      - `setTimeout`, `setInterval`, `setImmediate` (Node.js)
   
   #### Օրինակ
   ```javascript
   console.log('Start');
   
   setTimeout(() => {
     console.log('Macrotask');
   }, 0);
   
   Promise.resolve().then(() => {
     console.log('Microtask');
   });
   
   console.log('End');
   ```
   
   **Output:**
   ```
   Start
   End
   Microtask
   Macrotask
   ```
   
   **Քայլերի բացատրություն:**
   1. `Start` և `End` սինխրոն գործողություններն անմիջապես կատարվում են։
   2. Promise-ը (Microtask) կատարվում է նախ, նույնիսկ եթե `setTimeout`-ը (Macrotask) ժամանակը 0 է։
   3. `setTimeout` callback-ը կատարվում է վերջում։
   
   ---
   
   #### Կապ Call Stack-ի և Event Loop-ի միջև
   
   - Call Stack-ը կառավարում է JavaScript-ի սինխրոն գործողությունները։
   - Event Loop-ը ապահովում է, որ ասինխրոն գործողությունները ճիշտ պահին ավելացվեն Stack-ում։
   
   Այս համագործակցությունը թույլ է տալիս JavaScript-ին իրականացնել սինխրոն և ասինխրոն գործողությունները մեկ հոսքով, դարձնելով այն հզոր գործիք վեբ հավելվածների համար։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---
70. ### Ինչ է Nullish Coalescing Operator-ը JavaScript-ում?

   
   **Nullish Coalescing Operator**-ը (??) JavaScript-ում տրամաբանային օպերատոր է, որը վերադարձնում է առաջին ոչ-null կամ ոչ-undefined արժեքը։ Այն ներկայացվել է ECMAScript 2020 (ES11)-ում և թույլ է տալիս անվտանգորեն սահմանել լռելյայն արժեքներ՝ առանց սխալ արդյունքների, որոնք կարող են առաջանալ "falsey" արժեքների (օրինակ՝ 0, "", false) օգտագործման դեպքում։

---
   
   #### Սինտաքս
   ```javascript
   let result = value1 ?? value2;
   ```
   - **`value1`**: Առաջին արժեքը։
   - **`value2`**: Երկրորդ արժեքը, որը վերադարձվում է, եթե `value1`-ը null կամ undefined է։

---
   
   #### Ինչպես է աշխատում
   
   Nullish Coalescing Operator-ը ստուգում է, թե արդյոք առաջին արժեքը (left-hand operand) **null** կամ **undefined** է։
   - Եթե այն **null** կամ **undefined** է, վերադարձնում է երկրորդ արժեքը։
     - Եթե ոչ, վերադարձնում է առաջին արժեքը։
   
   #### Օրինակներ
   #### Հիմնական Օրինակ
   ```javascript
   let value = null;
   let defaultValue = 'Default';
   
   let result = value ?? defaultValue;
   console.log(result); // Output: "Default"
   ```
   
   #### Երբ առաջին արժեքը "falsey", բայց ոչ null/undefined է
   ```javascript
   let value = 0;
   let defaultValue = 100;
   
   let result = value ?? defaultValue;
   console.log(result); // Output: 0
   ```
   
   > **Նշում**: `0`-ն "falsey" է, բայց այն չի համարվում null կամ undefined։
   
   #### Համեմատություն `||` Օպերատորի Հետ
   ```javascript
   let value = 0;
   let defaultValue = 100;
   
   let result1 = value || defaultValue; // `||` օգտագործումը
   let result2 = value ?? defaultValue; // `??` օգտագործումը
   
   console.log(result1); // Output: 100
   console.log(result2); // Output: 0
   ```
   - `||` օպերատորը ստուգում է "falsey" արժեքներ (օրինակ՝ 0, "", false):
   - `??` օպերատորը ստուգում է միայն null և undefined:
   
   ---
   
   #### Օգտագործման Դեպքեր
   
   #### 1. **Լռելյայն Արժեքների Սահմանում**
   Երբ ցանկանում եք սահմանել լռելյայն արժեք՝ խուսափելով null/undefined-ից։
   
   ```javascript
   function greet(name) {
     let userName = name ?? 'Guest';
     console.log(`Hello, ${userName}!`);
   }
   
   greet(); // Output: Hello, Guest!
   greet('Alice'); // Output: Hello, Alice!
   ```
   
   #### 2. **Կոնֆիգուրացիոն Օբյեկտների Համար**
   ```javascript
   const config = {
     timeout: undefined,
     retries: 3
   };
   
   const timeout = config.timeout ?? 5000;
   console.log(timeout); // Output: 5000
   ```
   
   #### 3. **Հեշտ Կարդացվող Կոդ**
   ```javascript
   const userInput = null;
   const processedInput = userInput ?? 'Default Input';
   console.log(processedInput); // Output: "Default Input"
   ```

   ---
   
   #### Նշումներ և Սահմանափակումներ
   
   1. **Խառը Օգտագործում `||` և `??` Օպերատորների Հետ**
      - `||`-ն և `??`-ը չեն կարող օգտագործվել առանց փակագծերի, քանի որ դա առաջացնում է սինտաքսային սխալ։
      ```javascript
      let result = null || undefined ?? 'Default'; // SyntaxError
      let result = (null || undefined) ?? 'Default'; // Correct
      ```
   
   2. **Համատեղելիություն**
      - Nullish Coalescing Operator-ը հասանելի է ECMAScript 2020-ից սկսած, ինչը նշանակում է, որ այն չի աշխատի հին բրաուզերներում։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

71. ### Ինչ է Optional Chaining-ը JavaScript-ում?
   
   **Optional Chaining (`?.`)**-ը JavaScript-ում օպերատոր է, որը թույլ է տալիս ապահով կերպով մուտք գործել օբյեկտների կամ զանգվածների հատկություններին՝ խուսափելով սխալներից, երբ հատկությունը կամ արժեքը գոյություն չունի։ Այն ներկայացվել է ECMAScript 2020 (ES11)-ում և դարձնում է կոդը ավելի պարզ և ընթեռնելի։

   ---
   
   #### Ինչպես է աշխատում
   
   Optional Chaining-ը ստուգում է, թե արդյոք մուտքագրված հատկությունը (property) կամ մեթոդը գոյություն ունի։
   - Եթե այն **null** կամ **undefined** է, օպերատորը կվերադարձնի **undefined** առանց որևէ սխալի։
   - Եթե այն գոյություն ունի, օպերատորը կվերադարձնի արժեքը։

   ---
   
   #### Սինտաքս
   ```javascript
   let result = object?.property;
   let result = object?.method?.();
   let result = array?.[index];
   ```
   - **`object?.property`**: Ստուգում է՝ արդյոք `object`-ը գոյություն ունի, ապա մուտք գործում է `property`։
   - **`object?.method?.()`**: Ստուգում է՝ արդյոք `method`-ը գոյություն ունի, ապա կանչում է այն։
   - **`array?.[index]`**: Ստուգում է՝ արդյոք զանգվածը գոյություն ունի, ապա մուտք գործում է նշված ինդեքսով տարրին։

   ---
   
   #### Օրինակներ
   
   #### 1. Հիմնական Օրինակ
   ```javascript
   const user = {
     name: 'Alice',
     address: {
       city: 'New York'
     }
   };
   
   console.log(user?.address?.city); // Output: "New York"
   console.log(user?.contact?.email); // Output: undefined
   ```
   
   - Առանց Optional Chaining-ի, կոդը կհանգեցներ սխալի՝ եթե `contact` հատկությունը գոյություն չունի։
   
   #### 2. Optional Chaining զանգվածների հետ
   ```javascript
   const users = [{ name: 'Alice' }, { name: 'Bob' }];
   
   console.log(users?.[1]?.name); // Output: "Bob"
   console.log(users?.[2]?.name); // Output: undefined
   ```
   
   #### 3. Optional Chaining մեթոդների հետ
   ```javascript
   const user = {
     greet() {
       return 'Hello!';
     }
   };
   
   console.log(user?.greet?.()); // Output: "Hello!"
   
   const noUser = null;
   console.log(noUser?.greet?.()); // Output: undefined
   ```
   
   #### 4. Միասնական Օգտագործում
   ```javascript
   const data = {
     user: {
       profile: {
         details: {
           age: 25
         }
       }
     }
   };
   
   console.log(data?.user?.profile?.details?.age); // Output: 25
   console.log(data?.user?.profile?.info?.name); // Output: undefined
   ```

   ---
   
   #### Առավելությունները
   
   1. **Սխալների կանխարգելում**:
      - Կանխում է "Cannot read property of undefined"-ի նման սխալները։
   
   2. **Կոդի պարզություն**:
      - Ավելի քիչ "if" ստուգումներ։
   
   3. **Ենթաբաժանությունների հետ անվտանգ աշխատանք**:
      - Կոմպլեքս օբյեկտներում ավելի հեշտ է մուտք գործել ենթաբաժանությունների արժեքներին։

   ---
   
   #### Համեմատություն Առանց Optional Chaining-ի
   
   Առանց Optional Chaining-ի, նմանատիպ կոդը պահանջում է բազմաթիվ ստուգումներ՝ խուսափելու սխալներից։
   
   ```javascript
   const city = user && user.address && user.address.city;
   console.log(city); // "New York"
   ```
   
   Optional Chaining-ի միջոցով նույն կոդը.
   ```javascript
   const city = user?.address?.city;
   console.log(city); // "New York"
   ```

   ---
   
   #### Երբ օգտագործել
   
   1. **Օբյեկտների հետ աշխատանք**:
      - Երբ գործ ունեք խորը ներդրված օբյեկտների կամ API պատասխանների հետ։
   
   2. **Մեթոդների կանչի ժամանակ**:
      - Երբ վստահ չեք՝ արդյոք մեթոդը գոյություն ունի։
   
   3. **Զանգվածների հետ աշխատանք**:
      - Երբ աշխատում եք հնարավոր չհամապատասխան ինդեքսների հետ։

   ---
   
   #### Նշումներ և Սահմանափակումներ
   
   1. **Լինել զուսպ**:
      - Խուսափեք Optional Chaining-ի ավելորդ օգտագործումից, եթե դուք վստահ եք, որ արժեքները միշտ գոյություն ունեն։
   
   2. **Միայն null/undefined-ի համար**:
      - Optional Chaining-ը վերադարձնում է `undefined` միայն null կամ undefined արժեքների դեպքում։ Այլ "falsey" արժեքներ (օրինակ՝ 0, "") չեն ազդում։
   
   3. **Համատեղելիություն**:
      - Աջակցվում է ECMAScript 2020-ից սկսած։ Հին զննարկիչների համար անհրաժեշտ է օգտագործել Polyfill։


   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---
72. ### Ինչ է ES5 և ES6 տարբերությունները JavaScript-ում?
   
   **ES5 (ECMAScript 5)** և **ES6 (ECMAScript 2015)** JavaScript-ի տարբերակներ են, որոնք ներկայացնում են լեզվի զարգացման տարբեր փուլերը։
   
   - **ES5**-ը թողարկվել է 2009 թվականին և հանդիսանում է JavaScript-ի հիմքում ընկած ստանդարտներից մեկը, որը լայնորեն աջակցվում է բոլոր ժամանակակից զննարկիչների կողմից։
   
   - **ES6**-ը (հայտնի նաև որպես ECMAScript 2015) թողարկվել է 2015 թվականին և ներառում է բազմաթիվ նոր հնարավորություններ, որոնք դյուրինացնում են կոդ գրելը, կարդալը և կառավարումը։
   
   ---
   
   #### Հիմնական Տարբերությունները
   
   | **Հատկանիշ**            | **ES5**                                         | **ES6**                                          |
   |--------------------------|------------------------------------------------|-------------------------------------------------|
   | **Փոփոխականների հայտարարում** | `var`                                          | `let`, `const`                                  |
   | **Ֆունկցիոնալ սինտաքս**  | Սովորական ֆունկցիաներ                          | Arrow Functions (`=>`)                          |
   | **Օբյեկտներ**            | Սովորական հատկություններ                       | Շարժական հատկություններ (Computed Properties)  |
   | **Կլասներ**              | Պրոտոտիպերի հիմքով                             | Դասի սինտաքս (Classes)                          |
   | **Մոդուլներ**            | Չկա ստանդարտ աջակցություն                      | `import` և `export`                             |
   | **Տողային տառադարձումներ**| Սովորական տողեր (`""`, `''`)                    | Template Literals (` `` `)                      |
   | **Սփրեդ և ռեսթ օպերատորներ**| Չկա                                             | `...`                                            |
   | **Պրոմիսներ**            | Չկա                                             | `Promise`                                       |
   | **Լռելյայն պարամետրեր**  | Չկա                                             | Աջակցվում է                                      |

   ---
   
   #### Հատկանիշների Համեմատություն
   
   #### 1. Փոփոխականների հայտարարում
   
   **ES5**:
   ```javascript
   var name = 'Alice';
   ```
   - `var`-ը ունի ֆունկցիոնալ սքոուփ և կարող է կրկին հայտարարվել։
   
   **ES6**:
   ```javascript
   let name = 'Alice';
   const age = 25;
   ```
   - `let`-ն ունի բլոկային սքոուփ։
   - `const`-ը օգտագործվում է հաստատուն արժեքների համար։
   
   ---
   
   #### 2. Ֆունկցիաներ
   
   **ES5**:
   ```javascript
   function add(a, b) {
     return a + b;
   }
   ```
   
   **ES6**:
   ```javascript
   const add = (a, b) => a + b;
   ```
   - Arrow Functions (`=>`) ապահովում են կարճ սինտաքս և պահպանում են "this" կոնտեքստը։

   ---
   
   #### 3. Տողային տառադարձումներ (Template Literals)
   
   **ES5**:
   ```javascript
   var greeting = 'Hello, ' + name + '!';
   ```
   
   **ES6**:
   ```javascript
   const greeting = `Hello, ${name}!`;
   ```
   - Template Literals-ն ապահովում են դինամիկ տեքստերի ներդրման ավելի պարզ մեթոդ։

   ---
   
   #### 4. Օբյեկտներ
   
   **ES5**:
   ```javascript
   var person = {
     name: 'Alice',
     age: 25
   };
   ```
   
   **ES6**:
   ```javascript
   const person = {
     name: 'Alice',
     age: 25,
     greet() {
       console.log('Hello!');
     }
   };
   ```
   - ES6-ում աջակցվում են ֆունկցիոնալ հատկություններ և շարժական հատկություններ։

   ---
   
   #### 5. Կլասներ
   
   **ES5**:
   ```javascript
   function Person(name, age) {
     this.name = name;
     this.age = age;
   }
   Person.prototype.greet = function() {
     console.log('Hello!');
   };
   ```
   
   **ES6**:
   ```javascript
   class Person {
     constructor(name, age) {
       this.name = name;
       this.age = age;
     }
   
     greet() {
       console.log('Hello!');
     }
   }
   ```
   - ES6-ը ներկայացնում է կլասների պարզ սինտաքս, որն ավելի ընթեռնելի է։
   
   ---
   
   #### 6. Մոդուլներ
   
   **ES5**:
   ```javascript
   // No native support, used libraries like RequireJS
   var module = require('module');
   ```
   
   **ES6**:
   ```javascript
   import { myFunction } from './myModule.js';
   export const myVariable = 42;
   ```
   - ES6-ը ներկայացնում է ներկառուցված մոդուլների աջակցություն `import` և `export` օպերատորներով։
   
   ---
   
   #### 7. Պրոմիսներ
   
   **ES5**:
   ```javascript
   // Ասինխրոն գործողությունների համար օգտագործվում էին callback-ներ։
   function fetchData(callback) {
     setTimeout(() => {
       callback('Data loaded');
     }, 1000);
   }
   ```
   
   **ES6**:
   ```javascript
   const fetchData = () => {
     return new Promise((resolve, reject) => {
       setTimeout(() => {
         resolve('Data loaded');
       }, 1000);
     });
   };
   
   fetchData().then(data => console.log(data));
   ```
   - `Promise`-ները թույլ են տալիս կառավարել ասինխրոն գործողությունները ավելի հեշտ և ընթեռնելի ձևով։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---
73. ### Ինչ է JavaScript Engine-ը և ինչ տարբերություն կա V8-ի և SpiderMonkey-ի միջև?
   
   **JavaScript Engine**-ը ծրագրային ապահովում է, որը իրականացնում է JavaScript կոդի կատարումը։ JavaScript Engine-ը փոխակերպում է JavaScript կոդը մեքենայական կոդի, որպեսզի այն կարողանա կատարվել սարքի պրոցեսորի կողմից։

   ---
   
   #### Ինչպես է աշխատում JavaScript Engine-ը
   
   JavaScript Engine-ը հետևյալ քայլերով իրականացնում է JavaScript կոդի կատարումը.
   
   1. **Պարսում (Parsing):**
      - JavaScript Engine-ը ստուգում է կոդի սինտաքսը և ստեղծում է `AST` (Abstract Syntax Tree)։
   
   2. **Բայթկոդի ստեղծում (Bytecode Generation):**
      - Ստեղծվում է միջանկյալ "բայթկոդ", որը ներկայացնում է կոդի հիմնական կառուցվածքը։
   
   3. **Օպտիմալացում (Optimization):**
      - Engine-ը օպտիմալացնում է կոդը՝ բարելավելով դրա կատարողականությունը։
   
   4. **Կատարում (Execution):**
      - Օպտիմալացված բայթկոդը կատարում է սարքի պրոցեսորի վրա։
   
   ---
   
   #### Հիմնական JavaScript Engine-ներ
   
   | **Engine**       | **Զննարկիչ**          | **Ծրագրավորող**      |
   |------------------|-----------------------|----------------------|
   | **V8**           | Google Chrome         | Google               |
   | **SpiderMonkey** | Mozilla Firefox       | Mozilla              |
   | **Chakra**       | Microsoft Edge (հին) | Microsoft            |
   | **JavaScriptCore (JSC)** | Safari               | Apple                |

---
   
   #### V8 Engine
   
   **V8**-ը Google-ի կողմից մշակված JavaScript Engine է, որը օգտագործվում է Google Chrome և Node.js-ում։
   
   #### Հիմնական հատկանիշներ
   
   1. **Բարձր կատարողականություն:**
      - Օգտագործում է JIT (Just-In-Time) կոմպիլյացիա, որն արագացնում է կոդի կատարման գործընթացը։
   
   2. **Node.js աջակցություն:**
      - Վազում է սերվերային միջավայրերում՝ շնորհիվ Node.js-ի։
   
   3. **Memory Management:**
      - Ավտոմատացնում է հիշողության կառավարումը՝ օգտագործելով Garbage Collector։
   
   4. **Երկու կոմպիլյատոր:**
      - **Ignition:** Ստեղծում է բայթկոդ։
      - **TurboFan:** Օպտիմալացնում է բայթկոդը մեքենայական կոդի վերածելու համար։
   
   #### Աշխատանքի ընթացքը V8-ում
   ```mermaid
   graph TD
       A[Source Code] --> B[Parser]
       B --> C[AST]
       C --> D[Ignition (Bytecode)]
       D --> E[TurboFan (Optimized Machine Code)]
       E --> F[Execution]
   ```

   ---
   
   #### SpiderMonkey Engine
   
   **SpiderMonkey**-ը Mozilla-ի կողմից մշակված JavaScript Engine է, որը օգտագործվում է Firefox զննարկչում։
   
   #### Հիմնական հատկանիշներ
   
   1. **Հիմնական JavaScript Engine:**
      - SpiderMonkey-ը առաջին JavaScript Engine-ն է, որը ստեղծվել է Netscape-ի կողմից։
   
   2. **Interpreter և JIT կոմպիլյատոր:**
      - Օգտագործում է Baseline JIT և IonMonkey JIT կոմպիլյատորներ՝ կոդի օպտիմալացման համար։
   
   3. **Memory Management:**
      - Ներդրված է Garbage Collector։
   
   4. **Համատեղելիություն ECMAScript-ի հետ:**
      - Աջակցում է ECMAScript-ի նոր հնարավորություններին։
   
   #### Աշխատանքի ընթացքը SpiderMonkey-ում
   ```mermaid
   graph TD
       A[Source Code] --> B[Parser]
       B --> C[AST]
       C --> D[Baseline JIT]
       D --> E[IonMonkey JIT]
       E --> F[Execution]
   ```

---
   
   #### V8-ի և SpiderMonkey-ի Տարբերությունները
   
   | **Հատկանիշ**         | **V8**                             | **SpiderMonkey**                     |
   |----------------------|-----------------------------------|-------------------------------------|
   | **Զննարկիչ**         | Google Chrome, Edge, Node.js       | Mozilla Firefox                     |
   | **Կոմպիլյացիա**      | Ignition + TurboFan               | Baseline JIT + IonMonkey JIT        |
   | **Կատարողականություն**| Շատ արագ                           | Բարձր, բայց ոչ V8-ի մակարդակով      |
   | **Օգտագործում**       | Client-Side, Server-Side          | Հիմնականում Client-Side             |
   | **API-ների Աջակցություն** | Node.js                           | Gecko Engine                         |

---
   
   ## Վիզուալ համեմատություն
   
   ```mermaid
   flowchart LR
       A[V8 Engine]
       A -->|Ignition| B(Bytecode)
       B -->|TurboFan| C(Machine Code)
       C --> D[Execution]
   
       X[SpiderMonkey Engine]
       X -->|Baseline JIT| Y(Bytecode)
       Y -->|IonMonkey JIT| Z(Machine Code)
       Z --> W[Execution]
   ```

   ---
   
   #### Եզրակացություն
   
   JavaScript Engines-ը կարևոր դեր է խաղում JavaScript-ի կատարման գործընթացում։
   - **V8**-ը հայտնի է իր բարձր կատարողականությամբ և Node.js աջակցությամբ, ինչը դարձնում է այն հզոր գործիք ինչպես հաճախորդային, այնպես էլ սերվերային ծրագրերի համար։
   - **SpiderMonkey**-ը առաջին JavaScript Engine-ն է, որը մեծապես աջակցում է Firefox-ին և ապահովում է ECMAScript ստանդարտների առաջատար աջակցությունը։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---
74. ### Ինչ է Node.js-ը և ինչու է այն կարևոր JavaScript-ի համար?

   **Node.js**-ը JavaScript-ի կատարողական միջավայր (runtime environment) է, որը թույլ է տալիս JavaScript-ը գործարկել սերվերի վրա։ Node.js-ը կառուցված է **V8 JavaScript Engine**-ի վրա, որը մշակվել է Google-ի կողմից և ապահովում է արագություն և արդյունավետություն։
   
   Node.js-ը ներկայացվել է 2009 թվականին, և այն հեղափոխական նշանակություն ունեցավ JavaScript-ի համար՝ տեղափոխելով այն միայն վեբ զննարկիչից դեպի սերվերային միջավայրեր։

   ---
   
   #### Ինչպես է աշխատում Node.js-ը
   
   1. **Single-Threaded Architecture:**
      - Node.js-ը օգտագործում է միայն մեկ թել (thread), բայց այն աջակցում է միաժամանակյա (asynchronous) գործողություններին `Event Loop` մեխանիզմի միջոցով։
   
   2. **Non-blocking I/O:**
      - Օգտագործում է ոչ-բլոկային I/O գործողություններ՝ ֆայլերի, ցանցային հարցումների և այլ ռեսուրսների արագ մուտք գործելու համար։
   
   3. **JavaScript Everywhere:**
      - Ծրագրավորողները կարող են գրել ինչպես սերվերային, այնպես էլ հաճախորդային կոդ JavaScript-ով։

   ---
   
   #### Node.js-ի Հիմնական Հատկանիշները
   
   #### 1. **Արագություն**
   - Օգտագործում է V8 Engine-ը, որը թարգմանում է JavaScript-ը մեքենայական կոդի, դարձնելով այն շատ արագ։
   
   #### 2. **Event-Driven Architecture**
   - Ապահովում է ասինխրոն գործողությունների կատարում՝ նվազեցնելով CPU-ի բեռը։
   
   #### 3. **Package Ecosystem (npm)**
   - Node.js-ը ունի ամենամեծ փաթեթների կառավարման համակարգը՝ **npm (Node Package Manager)**:
     ```bash
     npm install express
     ```
   
   #### 4. **Cross-Platform Support**
   - Աջակցում է տարբեր օպերացիոն համակարգերին, ինչպիսիք են Windows, macOS և Linux։

   ---
   
   #### Օրինակ Node.js-ում
   
   #### 1. Սկզբնական Օրինակ
   ```javascript
   const http = require('http');
   
   const server = http.createServer((req, res) => {
     res.statusCode = 200;
     res.setHeader('Content-Type', 'text/plain');
     res.end('Hello, World!\n');
   });
   
   server.listen(3000, () => {
     console.log('Server running at http://localhost:3000/');
   });
   ```
   
   #### 2. Օգտագործելով npm փաթեթ
   ```javascript
   const express = require('express');
   const app = express();
   
   app.get('/', (req, res) => {
     res.send('Hello, Express!');
   });
   
   app.listen(3000, () => {
     console.log('Server running on http://localhost:3000/');
   });
   ```

   ---
   
   #### Node.js-ի Օգտագործման Դեպքեր
   
   1. **Real-Time Applications**
      - Օրինակ՝ չաթ հավելվածներ, խաղեր։
   
   2. **RESTful API Development**
      - Կատարյալ է API-ներ կառուցելու համար։
   
   3. **Microservices**
      - Օգտագործվում է միկրոսերվիսային ճարտարապետությունների համար։
   
   4. **Streaming Applications**
      - Օրինակ՝ Netflix-ի կամ YouTube-ի նման հոսքային ծառայություններ։

   ---
   
   #### Ինչու է Node.js-ը Կարևոր JavaScript-ի Համար
   
   #### 1. **JavaScript-ի Սահմանափակումների Հեռացում**
   - Node.js-ը JavaScript-ին բերեց սերվերի վրա, ինչը թույլ տվեց գրել "full-stack" հավելվածներ JavaScript-ով։
   
   #### 2. **Արագ Արտադրողականություն**
   - Նվազեցնում է զարգացման ժամանակը, քանի որ նույն լեզուն օգտագործվում է թե՛ հաճախորդային, թե՛ սերվերային կողմում։
   
   #### 3. **Մեծ Համայնք**
   - Node.js-ը ունի հսկայական և ակտիվ համայնք, ինչը հեշտացնում է նոր լուծումներ գտնելը և խնդիրների լուծումը։
   
   #### 4. **Հիմք Բազմաթիվ Գործիքների Համար**
   - Node.js-ը հիմք է բազմաթիվ JavaScript գործիքների համար, ինչպիսիք են Webpack-ը, Babel-ը, և այլն։
   
   ---
   
   #### Node.js-ի Առավելությունները
   
   1. **Արագ Կատարողականություն**
      - V8 Engine-ի և ասինխրոն I/O-ի շնորհիվ։
   
   2. **Ընդարձակ Ecoysystem**
      - npm-ի միջոցով հեշտ է մուտք գործել բազմազան գրադարաններ։
   
   3. **Սկսնակների Համար Հեշտ**
      - Ծրագրավորողները, ովքեր արդեն ծանոթ են JavaScript-ին, հեշտությամբ կարող են սկսել աշխատել Node.js-ի հետ։
   
   4. **Microservices Friendly**
      - Կատարյալ է միկրոսերվիսային հավելվածների համար։
   
   ---
   
   #### Node.js-ի Թերությունները
   
   1. **Single-Threaded Limitation**
      - Սահմանափակված է մեկ թելով, ինչը կարող է խնդիր դառնալ CPU-ի բարձր բեռի դեպքում։
   
   2. **Callback Hell**
      - Ասինխրոն կոդը կարող է դառնալ բարդ և դժվար ընթեռնելի։
   
   3. **Not Suitable for CPU-Heavy Tasks**
      - Ավելի հարմար է I/O-heavy ծրագրերի համար։


   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---
75. ### Ինչ է JavaScript-ում streams-ը?
   
   
   **Streams**-ը JavaScript-ում տվյալների մշակումի մեխանիզմ է, որը թույլ է տալիս աշխատել տվյալների շարունակական հոսքերի հետ։ Այն օգտակար է, երբ տվյալները մեծ են կամ ստացվում են մաս-մաս (օրինակ՝ ֆայլից, ցանցից կամ օգտագործողի մուտքից)։
   
   Streams-ը թույլ է տալիս մշակել տվյալները առանց ամբողջ բեռնված տվյալը հիշողության մեջ պահելու, ինչը բարելավում է կատարողականությունն ու նվազեցնում է ռեսուրսների օգտագործումը։

   ---
   
   #### Ինչու օգտագործել Streams-ը?
   
   1. **Կատարողականություն**:
      - Փոխանակ բեռնելու և մշակելու տվյալների ամբողջական ֆայլը, Streams-ը թույլ է տալիս մշակել տվյալները մաս-մաս, ինչը արագացնում է գործընթացը։
   
   2. **Հիշողության արդյունավետություն**:
      - Հարմար է մեծ ֆայլերի կամ տվյալների հոսքերի հետ աշխատելու համար՝ խուսափելով ամբողջ ֆայլը RAM-ում պահելուց։
   
   3. **Ինտերակտիվություն**:
      - Streams-ը թույլ է տալիս մշակել տվյալները իրական ժամանակում, ինչը հարմար է ցանցային հարցումների և իրական ժամանակում տվյալների փոխանցման համար։

   ---
   
   #### Streams-ի Տիպերը
   
   JavaScript-ում Streams-ը բաժանվում է չորս հիմնական տեսակների.
   
   | **Տիպ**        | **Նկարագրություն**                                                         |
   |-----------------|-----------------------------------------------------------------------------|
   | **Readable**    | Հոսքեր, որոնցից տվյալներ կարելի է կարդալ։                                    |
   | **Writable**    | Հոսքեր, որոնց մեջ կարելի է տվյալներ գրել։                                    |
   | **Duplex**      | Հոսքեր, որոնք կարող են լինել և՛ կարդացող, և՛ գրող։                          |
   | **Transform**   | Հոսքեր, որոնք տվյալները վերափոխում են (կարդալ և վերափոխել նոր ձևով)։        |

   ---
   
   #### Ինչպես է աշխատում Stream-ը JavaScript-ում
   
   Streams-ը հիմնականում օգտագործվում է Node.js-ում և ինտերֆեյս է ապահովում մուտքագրման և ելքի տվյալների հետ աշխատելու համար։
   
   ```mermaid
   graph TD
       A[Source (e.g., File)] -->|Readable Stream| B[Processing]
       B -->|Writable Stream| C[Destination (e.g., File, Network)]
   ```

   ---
   
   #### Օրինակներ
   
   #### 1. **Readable Stream**
   Կարդալ տվյալներ ֆայլից.
   ```javascript
   const fs = require('fs');
   
   const readableStream = fs.createReadStream('example.txt', {
     encoding: 'utf8',
     highWaterMark: 16
   });
   
   readableStream.on('data', (chunk) => {
     console.log('New chunk:', chunk);
   });
   
   readableStream.on('end', () => {
     console.log('Stream ended.');
   });
   ```
   
   #### 2. **Writable Stream**
   Գրել տվյալներ ֆայլի մեջ.
   ```javascript
   const fs = require('fs');
   
   const writableStream = fs.createWriteStream('output.txt');
   
   writableStream.write('Hello, ');
   writableStream.write('Streams!\n');
   writableStream.end();
   
   writableStream.on('finish', () => {
     console.log('Data written to file.');
   });
   ```
   
   #### 3. **Duplex Stream**
   ```javascript
   const { Duplex } = require('stream');
   
   const duplexStream = new Duplex({
     read(size) {
       this.push('Hello, ');
       this.push('Duplex Stream!');
       this.push(null);
     },
     write(chunk, encoding, callback) {
       console.log('Writable part:', chunk.toString());
       callback();
     }
   });
   
   duplexStream.on('data', (chunk) => {
     console.log('Readable part:', chunk.toString());
   });
   
   duplexStream.write('Test Data');
   duplexStream.end();
   ```
   
   #### 4. **Transform Stream**
   ```javascript
   const { Transform } = require('stream');
   
   const transformStream = new Transform({
     transform(chunk, encoding, callback) {
       this.push(chunk.toString().toUpperCase());
       callback();
     }
   });
   
   process.stdin.pipe(transformStream).pipe(process.stdout);
   ```
   - Այս օրինակում, մուտքագրման տեքստը վերածվում է մեծատառերի։

   ---
   
   #### Հիմնական Մեթոդներ և Իրադարձություններ
   
   | **Մեթոդ/Իրադարձություն** | **Նկարագրություն**                                    |
   |--------------------------|----------------------------------------------------|
   | `.pipe(destination)`     | Հոսքի տվյալները ուղղորդում է դեպի "destination"։    |
   | `.on('data')`            | Կանչվում է, երբ տվյալների նոր հատված է հասանելի։    |
   | `.on('end')`             | Կանչվում է, երբ հոսքը ավարտվում է։                  |
   | `.write(data)`           | Տվյալներ է գրում Writable Stream-ի մեջ։            |
   | `.end()`                 | Փակում է Writable Stream-ը։                        |

   ---
   
   #### Երբ օգտագործել Streams-ը
   
   1. **Մեծ ֆայլերի մշակում**:
      - Երբ ֆայլը չափազանց մեծ է ամբողջությամբ հիշողության մեջ բեռնելու համար։
   
   2. **Real-Time Data Processing**:
      - Օրինակ՝ չաթ հավելվածներ, հոսքային ծառայություններ։
   
   3. **Նվազագույն Հիշողության Օգտագործում**:
      - Թույլ է տալիս մշակել տվյալները մաս-մաս՝ նվազեցնելով RAM-ի բեռը։

   ---
   
   #### Եզրակացություն
   
   Streams-ը JavaScript-ում հզոր մեխանիզմ է, որը թույլ է տալիս արդյունավետորեն մշակել տվյալների հոսքերը։
   - Այն կատարյալ է մեծ ֆայլերի հետ աշխատելու, իրական ժամանակում տվյալների հոսքերի մշակման և ցանցային տվյալների հետ աշխատելու համար։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---
76. ### Ինչ է JavaScript-ի տարբեր տվյալների կառուցվածքները (Data Structures)?

   **Տվյալների կառուցվածքները (Data Structures)** JavaScript-ում օգտագործվում են տվյալների կազմակերպման և մշակման համար։ Դրանք օգնում են պահպանել, կառավարել և կատարել գործողություններ տվյալների վրա։
   
   JavaScript-ը աջակցում է ինչպես պարզ, այնպես էլ բարդ տվյալների կառուցվածքների, որոնցից յուրաքանչյուրն ունի իր նպատակն ու առավելությունները։

   ---
   
   #### Տվյալների կառուցվածքների Տիպերը
   
   JavaScript-ում տվյալների կառուցվածքները բաժանվում են հետևյալ կատեգորիաների.
   
   #### 1. Պարզ Տվյալների Տիպեր (Primitive Data Types)
   
   Պարզ տվյալների տիպերը ֆիքսված չափի և պարզ արժեքներ են։ Դրանք պարունակում են.
   
   | **Տիպ**      | **Նկարագրություն**                                     | **Օրինակ**                  |
   |---------------|-------------------------------------------------------|-----------------------------|
   | **Number**    | Թվեր, ներառյալ ամբողջ թվերը և իրական թվերը             | `42`, `3.14`                |
   | **String**    | Տողեր                                                 | `'Hello'`, `"World"`       |
   | **Boolean**   | Ճշմարիտ կամ կեղծ արժեք                                | `true`, `false`             |
   | **Null**      | Դատարկ արժեք                                          | `null`                      |
   | **Undefined** | Արժեք, որը դեռ չի սահմանվել                          | `undefined`                 |
   | **Symbol**    | Հատուկ անփոփոխ և եզակի արժեք                          | `Symbol('unique')`          |
   | **BigInt**    | Շատ մեծ թվերի համար, որոնք դուրս են Number-ի տիրույթից | `123n`, `BigInt(456)`       |

   ---
   
   #### 2. Բարդ Տվյալների Տիպեր (Complex Data Types)
   
   Բարդ տվյալների տիպերը թույլ են տալիս պահպանել և կառավարել բազմաթիվ արժեքներ։ Դրանք ներառում են.
   
   #### **Object**
   
   Object-ը JavaScript-ի հիմնական տվյալների կառուցվածքն է, որը օգտագործվում է հիմնված "key-value" զույգերի վրա։
   
   ```javascript
   const person = {
     name: 'Alice',
     age: 25,
     isStudent: true
   };
   ```
   
   #### **Array**
   
   Array-ը օբյեկտ է, որը պահպանում է տվյալների հաջորդականություն։
   
   ```javascript
   const numbers = [1, 2, 3, 4, 5];
   ```
   
   #### **Set**
   
   Set-ը տվյալների կառուցվածք է, որը պահում է եզակի արժեքների հավաքածու։
   
   ```javascript
   const uniqueNumbers = new Set([1, 2, 2, 3]); // {1, 2, 3}
   ```
   
   #### **Map**
   
   Map-ը տվյալների կառուցվածք է, որը պահում է "key-value" զույգեր։ Այն աջակցում է ցանկացած տիպի բանալիների։
   
   ```javascript
   const userRoles = new Map();
   userRoles.set('Alice', 'Admin');
   userRoles.set('Bob', 'User');
   ```
   
   #### **WeakSet**
   
   WeakSet-ը նման է Set-ին, բայց թույլ է պահում միայն օբյեկտների հղումները։
   
   ```javascript
   const ws = new WeakSet();
   const obj = { name: 'Alice' };
   ws.add(obj);
   ```
   
   #### **WeakMap**
   
   WeakMap-ը նման է Map-ին, բայց թույլ է պահում միայն օբյեկտների բանալիների հղումները։
   
   ```javascript
   const wm = new WeakMap();
   const obj = { name: 'Bob' };
   wm.set(obj, 'Developer');
   ```


---
   
   ## Տվյալների Կառուցվածքներ ըստ Նպատակի
   
   1. **Դասակարգման և որոնման համար:**
      - **Array**: Հարմար է տվյալների հավաքածուն հաջորդականությամբ պահելու համար։
      - **Set**: Օգտագործվում է եզակի արժեքների համար։
      - **Map**: "key-value" զույգերի արդյունավետ կառավարման համար։
   
   2. **Օբյեկտային տվյալների համար:**
      - **Object**: Օգտագործվում է բարդ տվյալների կառավարման համար։
   
   3. **Կախվածությունների կառավարման համար:**
      - **WeakMap, WeakSet**: Օգտագործվում են օբյեկտների ժամանակավոր հղումները կառավարելու համար՝ թույլ տալով Garbage Collector-ին հեռացնել չօգտագործվող օբյեկտները։

   ---
   
   #### Տվյալների Կառուցվածքների Համեմատություն
   
   | **Կառուցվածք** | **Առավելություններ**                                     | **Թերություններ**                                    |
   |----------------|---------------------------------------------------------|-----------------------------------------------------|
   | **Array**      | Հեշտ մուտք և փոփոխություն, աջակցում է բազմազան մեթոդների | Դանդաղ որոնում մեծ տվյալների դեպքում                |
   | **Set**        | Ապահովում է եզակի արժեքներ                               | Չի աջակցում "key-value" զույգերին                 |
   | **Map**        | Ճկուն "key-value" զույգերի կառավարման համար              | Չի ապահովում ուղղակի ինդեքսային մուտք              |
   | **WeakMap**    | Ավտոմատ հղումների կառավարում                            | Չի աջակցում կրկնությանը (iteration)                 |

   ---
   
   #### Եզրակացություն
   
   JavaScript-ի տվյալների կառուցվածքները կարևոր դեր են խաղում հավելվածների արդյունավետության և ընթեռնելիության համար։
   
   - **Array**-ը և **Object**-ը հիմնական տվյալների կառուցվածքներն են, որոնք կիրառվում են տարբեր դեպքերում։
   - **Set** և **Map**-ը հարմար են եզակի արժեքների և "key-value" զույգերի կառավարման համար։
   - **WeakSet** և **WeakMap**-ը ապահովում են ժամանակավոր օբյեկտների հղումների կառավարում։
   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---

77. ### Ինչ է JavaScript-ում WeakRef-ը?

   
   **WeakRef**-ը JavaScript-ում թույլ հղում (weak reference) է դեպի օբյեկտ։ Այն թույլ է տալիս պահպանել օբյեկտի հղումը առանց խոչընդոտելու այն Garbage Collector-ի կողմից հեռացնելու գործընթացը։
   
   **WeakRef**-ը ներդրվել է ECMAScript 2021-ում և հիմնականում օգտագործվում է որոշակի հատուկ դեպքերում, երբ անհրաժեշտ է թույլ հղում դեպի օբյեկտ, բայց առանց ազդելու հիշողության կառավարման վրա։
   
---
   
   #### Ինչպես է աշխատում WeakRef-ը
   
   WeakRef-ը թույլ հղում է պահում օբյեկտի վրա՝ թույլ տալով Garbage Collector-ին այն հեռացնել, եթե այլ հղումներ չկան։ WeakRef-ի հիմնական նպատակն է ապահովել, որ օբյեկտը չպահպանվի հիշողության մեջ ավելի երկար, քան անհրաժեշտ է։
   
   #### Սինտաքս
   ```javascript
   const weakRef = new WeakRef(target);
   ```
   - **`target`**: Օբյեկտ, որի հղումը պետք է պահել որպես թույլ հղում։
   
   #### Նշումներ
   - WeakRef-ը չի պահպանում օբյեկտը "կենդանի" (reachable) վիճակում։
     - WeakRef-ից արժեքը ստանալու համար օգտագործվում է `.deref()` մեթոդը։

   ---
   
   #### Օրինակներ
   
   #### 1. Ստեղծում և Օգտագործում
   ```javascript
   let obj = { name: 'Alice' };
   
   // Ստեղծում ենք WeakRef
   const weakRef = new WeakRef(obj);
   
   // Օբյեկտից արժեք ստանալու համար օգտագործվում է deref()
   console.log(weakRef.deref()); // Output: { name: 'Alice' }
   
   // Հեռացնում ենք օբյեկտը
   obj = null;
   
   // WeakRef-ը կարող է վերադարձնել undefined, եթե օբյեկտը Garbage Collector-ի կողմից հեռացված է
   console.log(weakRef.deref()); // Output: undefined (կախված GC-ից)
   ```
   
   #### 2. WeakRef-ի Օգտագործում Կեշավորման Համար
   WeakRef-ը հաճախ օգտագործվում է կեշավորման ժամանակ, երբ անհրաժեշտ է կարճատև պահել տվյալներ, բայց չխոչընդոտել նրանց Garbage Collector-ին հեռացնելուց։
   
   ```javascript
   class Cache {
     constructor() {
       this.store = new Map();
     }
   
     set(key, value) {
       this.store.set(key, new WeakRef(value));
     }
   
     get(key) {
       const ref = this.store.get(key);
       return ref ? ref.deref() : undefined;
     }
   }
   
   const cache = new Cache();
   let user = { name: 'Bob' };
   
   cache.set('user1', user);
   
   console.log(cache.get('user1')); // Output: { name: 'Bob' }
   
   // Հեռացնում ենք օբյեկտի հղումը
   user = null;
   
   // Garbage Collector-ը կարող է հեռացնել օբյեկտը
   console.log(cache.get('user1')); // Output: undefined (կախված GC-ից)
   ```

   ---
   
   #### WeakRef-ի Հատկություններ
   
   1. **`deref()` մեթոդ:**
      - Վերադարձնում է թույլ հղված օբյեկտը, եթե այն դեռ "կենդանի" է։
      - Եթե օբյեկտը Garbage Collector-ի կողմից հեռացված է, վերադարձնում է `undefined`։
   
   ```javascript
   const weakRef = new WeakRef({ value: 42 });
   console.log(weakRef.deref()?.value); // Output: 42
   ```
   
   2. **Միայն Օբյեկտների Հետ Աշխատանք:**
      - WeakRef-ը կարող է պահել միայն օբյեկտների հղումներ, ոչ պարզ տիպերի (primitive types):
      ```javascript
      const weakRef = new WeakRef(42); // TypeError
      ```

   ---
   
   #### WeakRef-ի Առավելություններ
   
   1. **Հիշողության Արդյունավետություն:**
      - Օգտակար է այն դեպքերում, երբ անհրաժեշտ է թույլ հղում, բայց առանց օբյեկտի "կենդանի" պահելու։
   
   2. **Օգտագործում Կարճատև Տվյալների Հետ:**
      - Հարմար է կարճատև արժեքների կամ ժամանակավոր կեշերի համար։
   
   ---
   
   #### WeakRef-ի Թերություններ
   
   1. **Garbage Collector-ի Կախվածություն:**
      - WeakRef-ը կախված է Garbage Collector-ից, ինչը նշանակում է, որ դուք չեք կարող ճշգրիտ կառավարել, թե երբ օբյեկտը կհեռացվի։
   
   2. **Կիրառման Սահմանափակումներ:**
      - Հիմնականում կիրառվում է միայն հատուկ դեպքերում, օրինակ՝ կեշավորման և ռեսուրսների ժամանակավոր կառավարման համար։

   ---
   
   #### Երբ Օգտագործել WeakRef
   
   1. **Կեշավորման Համար:**
      - Երբ պետք է պահել տվյալներ, բայց թույլ տալ Garbage Collector-ին հեռացնել դրանք։
   
   2. **Ինտենսիվ Օբյեկտների Կառավարում:**
      - Երբ հավելվածը աշխատում է մեծ թվով օբյեկտների հետ, և պահանջվում է հիշողության արդյունավետ կառավարում։

---

**[⬆ Back to Top](#բովանդակություն)**

   ---

78. ### Ինչ է Web APIs-ը JavaScript-ում?

   
   **Web APIs**-ը JavaScript-ում գործիքների և ինտերֆեյսների հավաքածու է, որը թույլ է տալիս ծրագրավորողներին փոխազդել վեբ զննարկիչների և վեբ հավելվածների հետ։ Web APIs-ն ապահովում է ֆունկցիոնալություն, ինչպիսիք են տվյալների փոխանակումը, օգտագործողի ինտերֆեյսի կառավարումը, ցանցային հարցումների կատարումը և այլն։
   
   Web APIs-ը ստեղծվում են զննարկիչների մշակողների կողմից և ապահովում են ինտեգրված հնարավորություններ, որոնք օգնում են հեշտացնել վեբ հավելվածների ստեղծումը։

   ---
   
   #### Ինչպես են աշխատում Web APIs-ը
   
   1. **JavaScript-ի և APIs-ի կապ**:
      - JavaScript-ը փոխազդում է Web APIs-ի հետ՝ օգտագործելով համապատասխան մեթոդներ և հատկություններ։
   
   2. **Զննարկիչների կողմից աջակցություն**:
      - Web APIs-ը ներդրված են զննարկիչներում, ինչպիսիք են Chrome, Firefox, Safari և Edge։
   
   3. **Ներդրված ասինխրոնություն**:
      - Շատ Web APIs աջակցում են ասինխրոն կոդին, ինչը հնարավորություն է տալիս կատարել գործողություններ ֆոնում՝ չխանգարելով գլխավոր թելը (main thread):

   ---
   
   #### Web APIs-ի Տիպեր
   
   #### 1. **DOM (Document Object Model)**
   - Օգտագործվում է վեբ էջերի կառուցվածքը փոփոխելու և դրանց բովանդակությունը կառավարելու համար։
   
   **Օրինակ:**
   ```javascript
   const header = document.querySelector('h1');
   header.textContent = 'Hello, Web APIs!';
   ```
   
   #### 2. **Console API**
   - Օգտագործվում է զննարկչի կոնսոլում տվյալների մուտքագրման կամ դուրս բերման համար։
   
   **Օրինակ:**
   ```javascript
   console.log('This is a message in the console.');
   ```
   
   #### 3. **Fetch API**
   - Օգտագործվում է HTTP հարցումներ կատարելու համար։
   
   **Օրինակ:**
   ```javascript
   fetch('https://api.example.com/data')
     .then(response => response.json())
     .then(data => console.log(data))
     .catch(error => console.error('Error:', error));
   ```
   
   #### 4. **Geolocation API**
   - Օգտագործվում է օգտագործողի դիրքը ստանալու համար։
   
   **Օրինակ:**
   ```javascript
   navigator.geolocation.getCurrentPosition(
     position => {
       console.log('Latitude:', position.coords.latitude);
       console.log('Longitude:', position.coords.longitude);
     },
     error => console.error('Error:', error)
   );
   ```
   
   #### 5. **Canvas API**
   - Օգտագործվում է վեկտորային գրաֆիկաներ ստեղծելու համար։
   
   **Օրինակ:**
   ```javascript
   const canvas = document.getElementById('myCanvas');
   const ctx = canvas.getContext('2d');
   ctx.fillStyle = 'blue';
   ctx.fillRect(10, 10, 150, 100);
   ```
   
   #### 6. **Web Storage API**
   - Տեղական տվյալներ պահպանելու համար։
   
   **Օրինակ (localStorage):**
   ```javascript
   localStorage.setItem('username', 'JohnDoe');
   console.log(localStorage.getItem('username'));
   ```
   
   #### 7. **Notifications API**
   - Օգտագործվում է համակարգային ծանուցումներ ցուցադրելու համար։
   
   **Օրինակ:**
   ```javascript
   if (Notification.permission === 'granted') {
     new Notification('Hello, Web APIs!');
   } else {
     Notification.requestPermission();
   }
   ```
   
   #### 8. **WebSockets API**
   - Օգտագործվում է իրական ժամանակում երկկողմանի հաղորդակցության համար։
   
   **Օրինակ:**
   ```javascript
   const socket = new WebSocket('ws://example.com/socket');
   
   socket.onopen = () => console.log('Connection opened');
   socket.onmessage = event => console.log('Message:', event.data);
   ```

   ---
   
   #### Առավելություններ
   
   1. **Հեշտացում:**
      - Web APIs-ն ապահովում է գործիքներ, որոնք դյուրացնում են բարդ գործողությունների իրականացումը։
   
   2. **Ասինխրոն գործողություններ:**
      - Շատ APIs աջակցում են ասինխրոն գործողություններին՝ բարելավելով կատարողականությունը։
   
   3. **Զննարկչի ֆունկցիոնալության ինտեգրում:**
      - Թույլ է տալիս ծրագրավորողներին մուտք գործել զննարկչի հնարավորություններին։
   
   4. **Հասանելիություն և Համատեղելիություն:**
      - Շատ APIs աջակցվում են հիմնական զննարկիչների կողմից։

   ---
   
   #### Թերություններ
   
   1. **Աջակցության սահմանափակում:**
      - Ոչ բոլոր APIs են աջակցվում հին զննարկիչներում։
   
   2. **Ասինխրոնության բարդություն:**
      - Ասինխրոն գործողությունների կառավարումը կարող է լինել բարդ։
   
   3. **Անվտանգության խնդիրներ:**
      - Օրինակ՝ Geolocation API-ն պահանջում է օգտագործողի թույլտվություն։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---
79. ### Ինչ է JavaScript-ի Performance Optimization-ը?
   
   **Performance Optimization**-ը JavaScript-ում մեթոդների և տեխնիկայի շարք է, որը կիրառվում է հավելվածի արագությունը և արդյունավետությունը բարելավելու համար։ Դա ներառում է կոդի կատարողականության բարձրացում, բեռնումի ժամանակի կրճատում և ռեսուրսների օպտիմալ օգտագործում։
   
   JavaScript-ի օպտիմալացումը կարևոր է ինտերակտիվ վեբ հավելվածների համար, որտեղ կատարողականությունը մեծ ազդեցություն ունի օգտագործողի փորձի վրա։

   ---
   
   #### Ինչու է կարևոր Performance Optimization-ը?
   
   1. **Օգտագործողի Բավարարվածություն:**
      - Արագ բեռնվող և արձագանքող հավելվածները բարձրացնում են օգտագործողի գոհունակությունը։
   
   2. **SEO Արդյունավետություն:**
      - Բարձր կատարողականություն ունեցող կայքերը ավելի լավ են դասվում որոնողական համակարգերում։
   
   3. **Ռեսուրսների Կառավարում:**
      - Ապահովում է օպտիմալ հիշողության և հաշվարկային հզորությունների օգտագործումը։
   
   4. **Մոբիլ Բրաուզերների Աջակցություն:**
      - Օգտակար է դանդաղ ցանցերի և սահմանափակ ռեսուրսներով սարքերի համար։

   ---
   
   #### JavaScript Performance Optimization Տեխնիկաներ
   
   #### 1. **Կոդի Օպտիմալացում**
   
   #### Օգտագործեք ES6+ սինտաքս
   ES6-ի սինտաքսը թույլ է տալիս գրել ավելի արագ և կարդացվող կոդ։
   ```javascript
   // Avoid
   var arr = [1, 2, 3];
   
   // Prefer
   const arr = [1, 2, 3];
   ```
   
   #### Խուսափեք կրկնվող հաշվարկներից
   ```javascript
   // Avoid
   for (let i = 0; i < array.length; i++) {
     console.log(array[i]);
   }
   
   // Prefer
   const length = array.length;
   for (let i = 0; i < length; i++) {
     console.log(array[i]);
   }
   ```
   
   #### 2. **Դադարեցրեք Բլոկավորող Գործողությունները**
   
   #### Օգտագործեք ասինխրոն ֆունկցիաներ
   ```javascript
   // Avoid
   const data = fetchSync('https://api.example.com');
   
   // Prefer
   const data = await fetch('https://api.example.com');
   ```
   
   #### 3. **Հիշողության Օպտիմալացում**
   
   #### Օգտագործեք Garbage Collector-ի Օգուտները
   - Պահպանեք հղումները միայն անհրաժեշտ տվյալներին։
   
   #### Խուսափեք մեծ օբյեկտներ պահելուց
   ```javascript
   // Avoid
   const largeData = new Array(1000000).fill('data');
   
   // Prefer
   const processLargeData = () => {
     const chunk = new Array(1000).fill('data');
     return chunk;
   };
   ```
   
   #### 4. **Նվազեցրեք DOM-Ի Գործողությունները**
   
   DOM փոփոխությունները հաճախ թանկարժեք են։
   - Օգտագործեք `documentFragment` մեծ DOM թարմացումների համար։
   
   ```javascript
   const fragment = document.createDocumentFragment();
   for (let i = 0; i < 100; i++) {
     const div = document.createElement('div');
     fragment.appendChild(div);
   }
   document.body.appendChild(fragment);
   ```
   
   #### 5. **Բեռնումի Ժամանակի Կրճատում**
   
   #### Կոմպրեսիա և Մինիմալացում
   - Օգտագործեք գործիքներ, ինչպիսիք են Webpack կամ Parcel։
   
   ```bash
   npm install terser
   ```
   
   #### Lazy Loading
   Բեռնեք միայն անհրաժեշտ սկրիպտները։
   ```javascript
   if (condition) {
     import('./module.js').then(module => {
       module.default();
     });
   }
   ```
   
   #### 6. **Օգտագործեք Կեշավորում**
   
   #### Կեշավորեք AJAX հարցումները
   ```javascript
   const fetchData = async (url) => {
     const cache = localStorage.getItem(url);
     if (cache) return JSON.parse(cache);
   
     const response = await fetch(url);
     const data = await response.json();
     localStorage.setItem(url, JSON.stringify(data));
     return data;
   };
   ```
   
   #### Կիրառեք Service Workers
   ```javascript
   navigator.serviceWorker.register('/sw.js');
   ```

   ---
   
   #### Performance Մոնիտորինգ Գործիքներ
   
   1. **Google Lighthouse:**
      - Վերլուծում է կայքի արագությունը և տալիս է օպտիմալացման առաջարկներ։
   
   2. **Chrome DevTools Performance Tab:**
      - Օգտագործվում է JavaScript-ի, CSS-ի և DOM-ի կատարողականության մոնիտորինգի համար։
   
   3. **WebPageTest:**
      - Ամբողջական վերլուծություն կայքի բեռնումի վերաբերյալ։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---
80. ### Ինչ է JavaScript-ում Event Listeners-ը?

   **Event Listeners**-ը JavaScript-ում ֆունկցիաներ են, որոնք հետևում են DOM-ի տարրերում առաջացող իրադարձություններին (events) և կատարում են որոշակի գործողություններ, երբ այդ իրադարձությունները տեղի են ունենում։
   
   Այս մեխանիզմը թույլ է տալիս ստեղծել ինտերակտիվ վեբ հավելվածներ՝ պատասխանելով օգտագործողի գործողություններին, ինչպիսիք են `click`, `keydown`, `mouseover`, և այլն։

   ---
   
   #### Ինչպես է աշխատում Event Listener-ը
   
   1. Event Listener-ը "լսում" է կոնկրետ իրադարձություն որոշակի տարրում։
   2. Երբ այդ իրադարձությունը տեղի է ունենում, համապատասխան ֆունկցիան (callback) ակտիվանում է։
   
   #### Սինտաքս
   ```javascript
   element.addEventListener(event, callback, options);
   ```
   - **`element`**: DOM տարրը, որի վրա կցվում է listener-ը։
   - **`event`**: Իրադարձության տիպը (օր.`"click"`, "mouseover")։
   - **`callback`**: Ֆունկցիան, որը կկատարվի, երբ իրադարձությունը տեղի ունենա։
   - **`options`** (ըստ ցանկության): Պարամետրեր, որոնք կարգավորում են իրադարձության վարքագիծը։

   ---
   
   #### Event Listener-ի Օրինակներ
   
   #### 1. `click` Իրադարձություն
   ```javascript
   const button = document.querySelector('button');
   
   button.addEventListener('click', () => {
     console.log('Button clicked!');
   });
   ```
   
   #### 2. `keydown` Իրադարձություն
   ```javascript
   document.addEventListener('keydown', (event) => {
     console.log(`Key pressed: ${event.key}`);
   });
   ```
   
   #### 3. `mouseover` Իրադարձություն
   ```javascript
   const box = document.querySelector('.box');
   
   box.addEventListener('mouseover', () => {
     console.log('Mouse is over the box!');
   });
   ```

   ---
   
   #### Event Listener-ի Կարգավորումներ
   
   #### 1. **`once` Պարամետր**
   - Իրադարձությունը լսելուց հետո listener-ը ավտոմատ կհեռացվի։
   
   ```javascript
   button.addEventListener('click', () => {
     console.log('This will run only once!');
   }, { once: true });
   ```
   
   #### 2. **`capture` Պարամետր**
   - Կարգավորում է, թե իրադարձությունը պետք է լսվի "capturing" կամ "bubbling" փուլում։
   
   ```javascript
   button.addEventListener('click', () => {
     console.log('Capturing phase');
   }, { capture: true });
   ```
   
   #### 3. **`passive` Պարամետր**
   - Կարգավորում է, որ listener-ը երբեք չկանգնեցնի իրադարձության լռելյայն վարքը։
   
   ```javascript
   document.addEventListener('scroll', () => {
     console.log('Scrolling...');
   }, { passive: true });
   ```

   ---
   
   #### Իրադարձությունների Հեռացում
   
   Event Listener-ը կարելի է հեռացնել `removeEventListener` մեթոդի միջոցով։
   
   #### Օրինակ
   ```javascript
   const logClick = () => {
     console.log('Button clicked!');
   };
   
   button.addEventListener('click', logClick);
   
   // Later in the code
   button.removeEventListener('click', logClick);
   ```
   > **Նշում:** `removeEventListener`-ը չի գործում, եթե callback ֆունկցիան հայտարարաված չէ որպես անունով ֆունկցիա։

   ---
   
   #### Event Propagation (Իրադարձության Տարածում)
   
   JavaScript-ում իրադարձությունները տարածվում են երկու հիմնական փուլով՝ **Capturing** և **Bubbling**:
   
   1. **Capturing (Իրադարձության բռնում):**
      - Իրադարձությունը տարածվում է տարրի արմատից դեպի ներս։
   
   2. **Bubbling (Իրադարձության պղպջակում):**
      - Իրադարձությունը տարածվում է ներսի տարրից դեպի արմատ։
   
   ```javascript
   const parent = document.querySelector('.parent');
   const child = document.querySelector('.child');
   
   parent.addEventListener('click', () => {
     console.log('Parent clicked!');
   }, true); // Capturing phase
   
   child.addEventListener('click', () => {
     console.log('Child clicked!');
   }); // Bubbling phase
   ```

   ---
   
   #### Event Delegation (Իրադարձությունների Պատվիրակում)
   
   **Event Delegation**-ը տեխնիկա է, որը թույլ է տալիս լսել իրադարձությունները ընդհանուր տարրի վրա և կառավարել ներսի տարրերի վրա տեղի ունեցող իրադարձությունները։
   
   #### Օրինակ
   ```javascript
   const list = document.querySelector('ul');
   
   list.addEventListener('click', (event) => {
     if (event.target.tagName === 'LI') {
       console.log(`List item clicked: ${event.target.textContent}`);
     }
   });
   ```
   > Այս մեթոդը նվազեցնում է Event Listener-ների քանակը և բարելավում է կատարողականությունը։

   ---
   
   #### Եզրակացություն
   
   **Event Listeners**-ը JavaScript-ում կարևոր գործիք է ինտերակտիվ վեբ հավելվածներ կառուցելու համար։
   - Նրանք թույլ են տալիս կառավարել օգտագործողի գործողությունները և արձագանքել դրանց իրական ժամանակում։
   - Event Delegation, Capturing և Bubbling մեխանիզմների օգտագործումը ապահովում է ավելի ճկուն և արդյունավետ կոդ։

   ---

**[⬆ Back to Top](#բովանդակություն)**

   ---
