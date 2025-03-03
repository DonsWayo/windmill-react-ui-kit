# Windmill React UI

The component library for fast and accessible development of gorgeous interfaces.

Projects using it: [Windmill Dashboard React](https://github.com/estevanmaito/windmill-dashboard-react)

## Mission

Be the most accessible it can be out of the box and the fastest way to production.

[Go to docs to see complete, live examples](https://windmillui.com/react-ui)

## 🚀 Usage

Install

```sh
npm i windmill-react-ui-kit
```

Inside `tailwind.config.js`

```js
const windmill = require('windmill-react-ui-kit/config')
module.exports = windmill({
  purge: [],
  theme: {
    extend: {},
  },
  variants: {},
  plugins: [],
})
```

Then place `Windmill` at the root of your project (the order doesn't matter, as long as your application is inside).

```js
// index.js
import React from 'react'
import ReactDOM from 'react-dom'
import App from './App'
import { Windmill } from 'windmill-react-ui-kit'

ReactDOM.render(
  <Windmill>
    <App />
  </Windmill>,
  document.getElementById('root')
)
```

Use components inside your project

```js
import { Button } from 'windmill-react-ui-kit'

function App() {
  return <Button>Hi there!</Button>
}

export default App
```

## 🔌 Contributing

- Fork
- Clone
- `npm install`
- `npm run storybook`

It will start a local server at `localhost:6006` with all components rendered.

⚠ Use `npm run cz` instead of `git commit`! It will guide you through some short questions and guarantee that you commit message is standardized.

Commit will also trigger linting and test coverage.
