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

    **[⬆ Back to Top](#բովանդակություն)**

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

    **[⬆ Back to Top](#բովանդակություն)**

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
   
    **[⬆ Back to Top](#բովանդակություն)**

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
      

    **[⬆ Back to Top](#բովանդակություն)**

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


   **[⬆ Back to Top](#բովանդակություն)**

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
         

    **[⬆ Back to Top](#բովանդակություն)**

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


    **[⬆ Back to Top](#բովանդակություն)**

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


   **[⬆ Back to Top](#բովանդակություն)**

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

**[⬆ Back to Top](#բովանդակություն)**

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

**[⬆ Back to Top](#բովանդակություն)**

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


**[⬆ Back to Top](#բովանդակություն)**
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
   

**[⬆ Back to Top](#բովանդակություն)**

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
   

**[⬆ Back to Top](#բովանդակություն)**
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

**[⬆ Back to Top](#բովանդակություն)**

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

**[⬆ Back to Top](#բովանդակություն)**
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
   
   const user1 = { name: "Alice" };
   const user2 = { name: "Bob" };
   
   introduce.call(user1); // "My name is Alice"
   introduce.call(user2); // "My name is Bob"
   ```
   
   3. **Մաթեմատիկական հաշվարկներ (apply):**
   
   ```javascript
   const numbers = [5, 6, 2, 3, 7];
   
   console.log(Math.max.apply(null, numbers)); // 7
   console.log(Math.min.apply(null, numbers)); // 2
   ```

**[⬆ Back to Top](#բովանդակություն)**

