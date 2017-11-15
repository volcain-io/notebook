# Code

A collection of useful & clever code snippets

Index of contents:

1. [JavaScript](#javascript)

## JavaScript

* Defaults (parameters) and destructing arrays
    ```javascript
    function createGrid([width = 5, height = 5] = []) {
        return `Generates a ${width} x ${height} grid`;
    }
    createGrid(); // Generates a 5 x 5 grid
    createGrid([]); // Generates a 5 x 5 grid
    createGrid([2]); // Generates a 2 x 5 grid
    createGrid([2,3]); // Generates a 2 x 3 grid
    createGrid([undefined,3]); // Generates a 5 x 3 grid
    ```

* Defaults (parameters) and destructing objects
    Just like array destructing with array defaults, a function can have an object
    be a default parameter and use object destructing.
    ```javascript
    function createSundae({scoops=1, toppings = ['Hot Fudge']} = {}) {
        const scoopText = scoops === 1 ? 'scoop' : 'scoops';
        return `Your sundae has ${scoops} ${scoopText} with ${toppings.join(' and ')} toppings.`;
    }
    createSundae(); // Your sundae has 1 scoop with Hot Fudge toppings.
    createSundae({}); // Your sundae has 1 scoop with Hot Fudge toppings.
    createSundae({scoops: 2}); // Your sundae has 2 scoops with Hot Fudge toppings.
    createSundae({scoops: 2, toppings: ['Sprinkle']}); // Your sundae has 2 scoops with Sprinkle toppings.
    createSundae({toppings: ['Cookie Dough']}); // Your sundae has 1 scoop with Cookie Dough toppings.
    ```

* Create & fill a two dimensional array (e.g. 3x2)
    ```javascript
    const ROWS = 3;
    const COLS = 2;
    Array(ROWS).fill().map(_ => Array(COLS).fill(false));
    // 0: [false, false]
    // 1: [false, false]
    // 2: [false, false]
    ```
