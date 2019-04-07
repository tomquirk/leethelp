# leethelp
JS helpers for Leetcode and friends

* Big O order -> https://en.wikipedia.org/wiki/Big_O_notation#Orders_of_common_functions

## sortObjects

```js
const sortObjects = (arr, key, asc = true) => {
  return arr.sort((a, b) => {
    if (a[key] < b[key]) return asc ? -1 : 1;
    if (a[key] > b[key]) return asc ? 1 : -1;
    return 0;
  });
};
```

## sort
```js
/**
 * Time complexity: O(nlog(n))
 */
const sort = (arr, asc = true) => {
  return arr.sort((a, b) => {
    if (a < b) return asc ? -1 : 1;
    if (a > b) return asc ? 1 : -1;
    return 0;
  });
};
```
