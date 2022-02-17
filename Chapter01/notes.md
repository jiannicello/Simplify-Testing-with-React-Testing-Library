# Ch 1 - Exploring React Testing Library

# DOM testing library

## @testing-library/dom

The module `@testing-library/dom` for **DOM testing library** was not in the package.json because as shown in package-lock.json, it's a dependency of `@testing-library/react` which is in the package.json. 

```js
import { fireEvent, screen } from '@testing-library/dom';
```

## `screen` functions
- `screen.getByPlaceholderText(/first name/i)`
- `screen.getByRole('textbox', {
    name: /first name:/i
})` // when label is used and when input name attribute is used
- `screen.queryByRole('button', {
    name: /hide details/i,
  });` // when button is not on page and you don't want an error. You want to check that it's not there.
- `screen.getByText('/email address/i)` // text of an element

# jest

- JavaScript testing framework, testrunner, created by Facebook.
- provides the `describe`, `it`, `test` and `expect` functions





