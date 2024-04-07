# Javascript ծրագրավորման լեզվի հարցազրույցի հարցեր և պատասխաններ

> Սեղմեք :star: եթե ձեզ դուր է գալիս. 
> Եթե ունեք ձեր հարցերը, կխնդրենք բացել Pull Request այդ հարցերը ծրագրում ավելացնելու համար.

## Բովանդակություն

| No. | Հարցեր                                                                                |
|-----|---------------------------------------------------------------------------------------|
| 1   | [Որոնք են JavaScript լեզվում Primitive տիպերը](#որոնք-են-javaScript-լեզվում-primitive-տիպերը) |
| 2   | [Ինչ է undefined և undeclared](#ինչ-է-undefined-և-undeclared)                         |

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

3. ### 
