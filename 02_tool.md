## npm

npm allows you to bring in code from the npm registry which is a bunch of open source modules that people have written so you can use them in your project

## Prettier

#### code quality

```
npm install --global prettier
```

## npm/Yarn scripts

```
'scripts': {
    'format': "prettier --write \"src/**/*.{js,jsx}\""
}
```

## ESLint

```
npm install -D eslint eslint-config-prettier
```

> [Airbnb config](https://github.com/airbnb/javascript)

```
// .eslintrc.json
{
  "extends": ["eslint:recommended", "prettier"],
  "plugins": [],
  "parserOptions": {
    "ecmaVersion": 2021,
    "sourceType": "module",
    "ecmaFeatures": {
      "jsx": true
    }
  },
  "env": {
    "es6": true,
    "browser": true,
    "node": true
  }
}

```

```
"lint": "eslint \"src/**/*.{js,jsx}\" --quiet"


npm run eslint -- --fix
```
