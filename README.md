# eslint-tutorial

## Init
```
eslint --init
```

## Configure
```
{
  "rules": {
    "semi": ["error", "always"],
    "quotes": ["error", "double"]
  }
}
// rule: ["level", "option for rule"]
```
[rules](http://eslint.org/docs/rules/)

## Error Level
- "off" or 0: turn the rule off
- "warn" or 1: turn the rule on as a warning (doesn’t affect exit code)
- "error" or 2: turn the rule on as an error (exit code will be 1)

## pieces
- Environments: which environments your script is designed
- Globals: global vars
- Rules: which rules are enabled

## Parser Options
- default: es5
- es6, es7, JSX
- eslint-plugin-react

```
{
  "parserOptions": {
    "ecmaVersion": 6,
	"sourceType": "module",
	"ecmaFeatures": {
	  "jsx": true
	}
  },
  "rules": { ... }
}
```

## Parser
- default: Espree
- esprima, babel-eslint

