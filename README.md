*This repository is a mirror of the [component](http://component.io) module [damonoehlman/stylar](http://github.com/damonoehlman/stylar). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/damonoehlman-stylar`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
# Stylar

Badass CSS Styling Helpers

## Usage

Get the current transform on an element

```js
console.log(stylar(targetElement, 'transform'));
```

Update the transform of an element:

```js
stylar(targetElement, 'transform', 'translate(50px, 100px)');
```

Get the current transform of an element using the `get` helper:

```js
stylar(targetElement).get('transform');
```

Set the current transform of the element using the `set` helper (chainable):

```js
stylar(targetElement)
    .set('transform', 'translate(50px, 100px)')
    .set('background-color', 'red');
```

__NOTE:__ You can also use the set forms to update multiple elements at once:

```js
stylar([element1, element2], 'transform', 'translate(50px, 100px)');
```