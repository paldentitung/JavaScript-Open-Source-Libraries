# Beginner-Friendly JavaScript Open Source Libraries

This is a curated list of **useful JavaScript open-source libraries** for beginners. These libraries help you learn faster and make your projects more interactive and professional.

---

## 1. [Lodash](https://lodash.com)

A utility library for **working with arrays, objects, strings, and more**.  
**Example:**
```javascript
import _ from "lodash";

const numbers = [1, 2, 3, 4, 5];
const doubled = _.map(numbers, n => n * 2);
console.log(doubled); // [2, 4, 6, 8, 10]
```

## 2. [Axios](https://axios-http.com/)

A promise-based HTTP client for fetching data from APIs easily.
Example:
```javascript

import axios from "axios";

axios.get("https://jsonplaceholder.typicode.com/todos/1")
  .then(response => console.log(response.data))
  .catch(error => console.error(error));
```

## 3. [Day.js](https://day.js.org/)

A lightweight library for date and time manipulation, alternative to Moment.js.
Example:
``` javascript
import dayjs from "dayjs";

const now = dayjs();
console.log(now.format("YYYY-MM-DD HH:mm:ss"));
```
