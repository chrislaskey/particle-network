# Particle Network

> HTML canvas-based rendering of a network of particles in motion

Based on [VincentGarreau/particles.js](https://github.com/VincentGarreau/particles.js/).

## Usage

### Basic HTML

Copy the `src/es5/particle-network.js` file into your project.

In the HTML `head` include the library:

```html
<script src="particle-network.js"></script>
```

Then create a new container right before the closing `</body>` tag:

```html
<script>
  var particleContainer = document.querySelector('#hero')
  var particleOptions = {
    density: 10000,
    velocity: 0.5
  }

  new ParticleNetwork(particleContainer, particleOptions)
</script>
```

### React

Copy `src/react` into your project directory. Then import and define the
component inside a containing element:

```javascript
import React from 'react'
import ParticleNetwork from './ParticleNetwork'

const Page = () => (
  <header>
    <ParticleNetwork id='header-particles' />
    <h1>Hello World</h1>
  </header>
)
```

To style the component pass an `id` attribute.
