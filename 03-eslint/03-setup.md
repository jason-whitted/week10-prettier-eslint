# ESLint: Setup

## VS Code Setup

1. Install the **ESLint** extension

## Project Setup

Configuration can be done via:

- `.eslintrc` file (JSON)
- `.eslintrc.yml` file (YAML)
- `eslintConfig` section in your `package.json`

## Install eslint-config-react-app

Follow the installation instructions from [https://github.com/facebook/create-react-app/tree/master/packages/eslint-config-react-app](https://github.com/facebook/create-react-app/tree/master/packages/eslint-config-react-app)

```bash
npm install --save-dev eslint-config-react-app @typescript-eslint/eslint-plugin@^4.0.0 @typescript-eslint/parser@^4.0.0 babel-eslint@^10.0.0 eslint@^7.5.0 eslint-plugin-flowtype@^5.2.0 eslint-plugin-import@^2.22.0 eslint-plugin-jsx-a11y@^6.3.1 eslint-plugin-react@^7.20.3 eslint-plugin-react-hooks@^4.0.8
```

## Install prettier-eslint

```bash
npm install --save-dev prettier-eslint
```

## Enable ESLint in VS Code

By default, VS Code prevents many extensions from accessing your filesystem. When initially configuring ESLint in VS Code you may receive the warning:

> ESLint is disabled since its execution has not been approved or denied yet. Use the light bulb menu to open the approval dialog.

Enable ESLint. I usually specify "Allow Everywhere".

## Configuration
```json
{
    "extends": "react-app",
    "rules": {
      "eqeqeq": "error",
      "no-console": "warning",
      "no-debugger": "warning",
      "no-var": "error",
      "prefer-const": "error"
    }
  }
```

More rules can be enabled/disabled/configured. Check out the documentation on the [eslint.org](https://eslint.org) website.