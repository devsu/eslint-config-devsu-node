# eslint-config-node
Devsu's ESLint shareable configs for node applications.

## Usage

Add `eslint` and `eslint-config-devsu-node` to `devDependencies` in your `package.json`:

```
npm install --save-dev eslint eslint-config-devsu-node
```

In your project root, create/edit `.eslintrc`:

```
{
  "extends": "devsu-node"
}
```

Change in `package.json` your run script to add a lint property:

```
...
"scripts": {
  "lint": "eslint ."
},
...
```

Try our rules by running:

```
npm run lint
```

## Overriding rules

To override a particular rule, use the `rules` key:

```
{
  "extends": "devsu-node",
  "rules": {
    "comma-dangle": "off"
  }
}
```
