# Eslint, stylelint and Prettier config files

Just to make things easy, if you think this is what you want just follow the readme.

## Overview

Here will be most common config files.

Includes:

- `eslint`
- `babel-eslint`
- `eslint-plugin-react`
- `eslint-plugin-react-hooks`
- `editorconfig`
- `stylelint`
- `prettier`

## Usage

Install the plugin

```sh
pnpm i @calgns/eslint-config
```

Create an `.eslintrc` file in your project root and add:

```json
{
  "extends": ["@calgns/eslint-config"]
}
```

Create a `.prettierrc.js` file in your project root and add:

```js
module.exports = require('@calgns/prettier-config');
```

Add an `.editorconfig` file in the project root:

```
root = true

[*]
indent_style = space
quote_type = auto # single or double
indent_size = 2
end_of_line = lf
charset = utf-8
semicolons = true
linebreak_style = "unix"
trim_trailing_whitespace = true
insert_final_newline = true
```

## Customize

If needed you can add your own preferences.
```json
{
	"extends": ["fast-lint-prettify"],
	"rules": {
		// your own rules here
	}
}
```