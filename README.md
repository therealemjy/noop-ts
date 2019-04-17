# noop

A very simple "do nothing" JavaScript function, compatible with TypeScript.
Since the noop accepts any arguments (and does nothing in return), it can be used as a replacement of any function passed as a parameter of another function or a property of a web/React/Angular/(...) component.

That can be particularly useful for unit tests, for example to test a React component:

```javascript
import noop from 'noop-ts';

describe('MyComponent', () => {
  it('does what I want it to do', () => {
    const component = shallow(<MyComponent onChange={noop} />);
    expect(component).toMatchSnapshot();
  });
});
```

## Installation

### npm

```
npm install noop --save-dev
```

### yarn

```
yarn add noop --dev
```

