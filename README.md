# perlin-noise

Simple Perlin noise derived from p5.js

## Installation

    # Using npm
    npm install @chriscourses/perlin-noise

    # Using Yarn
    yarn add @chriscourses/perlin-noise

## Usage

Return a one dimensional Perlin noise value:

```js
const { noise } = require('@chriscourses/perlin-noise')
const x = noise(10) // returns value 0-1
```

You can also call noise in sequence to access all of its pre-generated values:

```js
const { noise } = require('@chriscourses/perlin-noise')

for (let i = 0; i < 100; i += 0.01;) {
  const x = noise(i) // returns value 0-1, but different and related to the previous return value on each loop cycle
}
```

## API

### noise(x, [y], [z])

Returns a Perlin noise generated value 0 - 1

| Parameter    | Type     | Description                         |
| ------------ | -------- | ----------------------------------- |
| x            | _number_ | x value for one dimensional noise   |
| y (optional) | _number_ | y value for two dimensional noise   |
| z (optional) | _number_ | z value for three dimensional noise |
