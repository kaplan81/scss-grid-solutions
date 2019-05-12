# Scss Grid Solutions

> Sample project on how to create your own CSS layout framework and theming with Sass by using the CSS Grid specification.

## Up and running

This project is deliciously simple.

It only contains Sass files and an `index.html`.

```
npm i
npm start
```

## Scss Structure

The `scss` folder is compiled to the `css` one.

`reset.scss` is based on [Eric Meyer's reset](https://meyerweb.com/eric/tools/css/reset).

`app.scss` is a Sass barrel that contains all partials:

- functions
- mixins
- \*rules
- variables

\*"rules" are utility classes to be declared on our templates.

## Grid Framework

There is a separation of concerns split into the differnt partials.

The grid framework has its corresponding mixin, rule and variable and they are interconnected: variables are used in mixins and mixins in rules.

The result is a Grid System. Pretty much Bootstrap-like but rows are now grid displayed divs.

The main benefit we obtain is:

- Apart from the classical 12 column system we have the alternative of using a 10 column based one.
- We do not need to install any library.

Mobile first is the default approach but if we use the hidden rule we can use `hidden-xx-down` classes to think the opposite just for things that we do not intend to display on ocassions.

## Theming

`_blue-theme.variable.scss` provides a good example on how to theme your applications.

The logic of that variable follows the principles of [Material Design](https://material.io/design/color/#tools-for-picking-colors).
