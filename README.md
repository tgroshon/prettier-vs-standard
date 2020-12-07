Prettier vs. Standard
=====================

A formatting comparison.

How will the two tools format the following input code:

```javascript
export const f = function(a) { if (a === 0) { return []; } return [1,2,3,4,a].map(int => int * 2); }
```

Standard via `standard --fix`:

```javascript
export const f = function (a) { if (a === 0) { return [] } return [1, 2, 3, 4, a].map(int => int * 2) }
```

Prettier via `prettier`:

```javascript
export const f = function (a) {
  if (a === 0) {
    return [];
  }
  return [1, 2, 3, 4, a].map((int) => int * 2);
};
```

## Try Yourself

Clone and run either: `npm run standard` or `npm run prettier`

