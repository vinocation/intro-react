## Babel

transpilation tool 

One of its core uses to transform futuristic JavaScript (like ES2021) to an older version of JavaScript (like ES5 i.e. JavaScript before 2015) so that older browsers can use your newer JavaScript.

```
npm install -D @babel/core@7.12.16 @babel/preset-react@7.12.13
```

.babelrc

```
{
  "presets": [
    [
      "@babel/preset-react",
      {
        "runtime": "automatic"
      }
    ]
  ]
}



```

### Browsers list

```
//package.json
{
  …
  "browserslist": [
    "last 2 Chrome versions"
  ]
}

```