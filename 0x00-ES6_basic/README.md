0x00. ES6 Basics
================

  };
}

```

Execution:

```
bob@dylan:~$ cat 2-main.js
import getNeighborhoodsList from './2-arrow.js';

const neighborhoodsList = new getNeighborhoodsList();
const res = neighborhoodsList.addNeighborhood('Noe Valley');
console.log(res);
bob@dylan:~$
bob@dylan:~$ npm run dev 2-main.js
[ 'SOMA', 'Union Square', 'Noe Valley' ]
bob@dylan:~$

```

**Repo:**

-   GitHub repository: `alx-backend-javascript`
-   Directory: `0x00-ES6_basic`
-   File: `2-arrow.js`

 Done? Help Check your code Ask for a new correction Get a sandbox QA Review

### 3\. Parameter defaults

mandatory

Score: 0.00% (Checks completed: 0.00%)

Condense the internals of the following function to 1 line - without changing the name of each function/variable.

*Hint:* The key here to define default parameter values for the function parameters.

```
export default function getSumOfHoods(initialNumber, expansion1989, expansion2019) {
  if (expansion1989 === undefined) {
    expansion1989 = 89;
  }

  if (expansion2019 === undefined) {
    expansion2019 = 19;
  }
  return initialNumber + expansion1989 + expansion2019;
}

```

Execution:

```
bob@dylan:~$ cat 3-main.js
import getSumOfHoods from './3-default-parameter.js';

console.log(getSumOfHoods(34));
console.log(getSumOfHoods(34, 3));
console.log(getSumOfHoods(34, 3, 4));
bob@dylan:~$
bob@dylan:~$ npm run dev 3-main.js
142
56
41
bob@dylan:~$

```

**Repo:**

-   GitHub repository: `alx-backend-javascript`
-   Directory: `0x00-ES6_basic`
-   File: `3-default-parameter.js`

 Done? Help Check your code Ask for a new correction Get a sandbox QA Review

### 4\. Rest parameter syntax for functions

mandatory

Score: 0.00% (Checks completed: 0.00%)

Modify the following function to return the number of arguments passed to it using the rest parameter syntax

```
export default function returnHowManyArguments() {

}

```

Example:

```
> returnHowManyArguments("Hello", "Holberton", 2020);
3
>

```

Execution:

```
bob@dylan:~$ cat 4-main.js
import returnHowManyArguments from './4-rest-parameter.js';

console.log(returnHowManyArguments("one"));
console.log(returnHowManyArguments("one", "two", 3, "4th"));
bob@dylan:~$
bob@dylan:~$ npm run dev 4-main.js
1
4
bob@dylan:~$

```

**Repo:**

