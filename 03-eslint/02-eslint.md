# ESLint

ESLint is a linting tool specifically for EcmaScript.

> **Find Problems**<br>
> ESLint statically analyzes your code to quickly find problems.
>
> **Fix Automatically**<br>
> Many problems ESLint finds can be automatically fixed.
>
> **Customize**<br>
> You can customize ESLint to work exactly the way you need it for your project.

## Aside: Usage with Prettier

The `prettier` code formatter and the `ESLint` linter rules often times contradict each other.

Typically we will want `prettier` to run first, and then we will allow `eslint` to fix the document.

In a NodeJS project we would normally need to install the npm packages for `prettier` and `eslint` in addition to configuring them. Since these two libraries are used frequently together a `prettier-eslint` library was created to help prevent some of the infighting that these two libraries may have.

## Aside: Rules

ESLint does nothing by default. You need to configure rules. There are libraries that provide a default ruleset we can use to make our lives easier. You can then extend from those rulesets and override rules to your liking.

The `eslint:recommended` ruleset comes with eslint by default, which can be used as a starting point.

The [eslint-config-react-app](https://github.com/facebook/create-react-app/tree/master/packages/eslint-config-react-app) package provides the base ruleset that React apps use.

The [eslint-config-airbnb](https://www.npmjs.com/package/eslint-config-airbnb) package is extremely popular and provides a very specifc, well documented ruleset based on best practices in the industry. It is a bit more involved to set up and will require a fair bit of fiddling with individual rules to get to work exactly how you want.

In the end, the **airbnb** ruleset is a more valuable linting experience; however, to keep things simple we'll be sticking with the **react-app** ruleset.
