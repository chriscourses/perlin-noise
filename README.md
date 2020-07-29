# perlin-noise
Library-free Perlin noise derived from p5.js

Installation
-----
    # Using Yarn
    yarn add @chriscourses/perlin-noise
    
    # Using npm
    npm install @chriscourses/perlin-noise

    
Usage
-----
Return a one dimensional Perlin noise value:

    const { noise } = require('@chriscourses/perlin-noise')
    const x = noise(10) // returns value 0-1
    
You can also call noise in sequence to access all of its pre-generated values:

    const { noise } = require('@chriscourses/perlin-noise')
    
    for (let i = 0; i < 100; i += 0.01;) {
      const x = noise(i) // returns value 0-1, but different and related to the previous return value on each loop cycle
    }
    
API
-----

### noise(x, [y], [z])

Returns the Perlin noise value at specified coordinates.

| Parameter       | Type            | Description
|-----------------|-----------------|---------------
| x               | *number*        | x value for one dimensional noise 
| y               | *number*        | y value for two dimensional noise (optional)
| z               | *number*        | z value for three dimensional noise (optional)
