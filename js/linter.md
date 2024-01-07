# Linter

# Set up

[Resource](https://www.youtube.com/watch?v=3BHXuZvI4FI)

Install `eslint`

```sh
bun add -D eslint
```

Install `prettier`

```sh
bun add -D prettier
```

Install `eslint-config-prettier` to avoid conflicts

```sh
bun add -D eslint-config-prettier
```

Define `.eslintrc.json`

**Basic example**

```json
{
  "env": {
    "browser": true,
    "es2021": true
  },
  "extends": ["standard-with-typescript", "eslint-config-prettier"],
  "parserOptions": {
    "ecmaVersion": "latest",
    "sourceType": "module"
  },
  "plugins": [],
  "rules": {}
}
```

Define `.eslintignore` to avoid actions over built files if it is necessary

Define `.prettierrc`

```json
{
  "useTabs": true,
  "singleQuote": true,
  "arrowParens": "avoid"
}
```

Define `.prettierignore` to avoid actions over built files if it is necessary

## Set up VS Code

Install `eslint` plugin

Install `prettier code formatter` plugin

Configure `Format auto save`

Select default formatter performing a manual formatter over a file.
