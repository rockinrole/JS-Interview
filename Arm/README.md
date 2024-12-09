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
   

    **[⬆ Back to Top](#բովանդակություն)**

9. ### Ինչ է boxing-ը


    **[⬆ Back to Top](#բովանդակություն)**

10. ### Ինչ են double equal (==) և triple equal (===) օպերատորները


    **[⬆ Back to Top](#բովանդակություն)**



