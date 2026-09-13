# Moonverse

An interactive 3D moon visualization experience built with Three.js. A stunning visual journey through a procedurally generated lunar landscape with dynamic aurora effects, realistic water simulation, and ambient celestial phenomena.

## Features

- **Interactive 3D Environment**: Drag to explore, scroll to zoom with smooth orbit controls
- **Procedural Terrain**: Algorithmically generated mountain landscape using Perlin noise-like functions
- **Aurora Borealis Effects**: Realistic animated northern lights with dynamic color gradients and wave patterns
- **Water Simulation**: Real-time water surface with dynamic normal maps and reflections
- **Celestial Elements**:
  - Animated moon with realistic lighting
  - 18,000+ procedurally placed stars with twinkling effect
  - Shooting stars with particle trails
  - Ambient birds and fish animations
- **Post-Processing**: Bloom and tone mapping for cinematic visuals
- **Responsive Design**: Adapts to any screen size and device

## Technology Stack

- **Three.js** - 3D graphics library
- **GLSL Shaders** - Custom vertex and fragment shaders for effects
- **WebGL** - Hardware-accelerated rendering
- **Canvas API** - Procedural texture generation

## Performance

- Optimized for 60 FPS with high-performance WebGL settings
- Adaptive pixel ratio scaling
- Efficient particle and geometry management
- Bloom post-processing with proper tone mapping

## Getting Started

### Installation

Clone the repository:
```bash
git clone https://github.com/saklincodes/MoonVerse.git
cd MoonVerse
```

### Running Locally

Since this is a static web project, simply open `index.html` in your browser:

```bash
# Using Python 3
python -m http.server 8000

# Using Python 2
python -m SimpleHTTPServer 8000

# Using Node.js
npx http-server
```

Then navigate to `http://localhost:8000` in your browser.

## Controls

- **Mouse Drag**: Rotate and explore the scene
- **Mouse Scroll**: Zoom in/out
- **Auto Animation**: Aurora, stars, and creatures animate automatically

## Browser Support

- Chrome/Chromium 90+
- Firefox 88+
- Safari 14+
- Edge 90+

Requires a modern browser with WebGL 2.0 support.

## Project Structure

```
MoonVerse/
├── index.html          # Main HTML file with all styles and scripts
├── README.md          # This file
└── assets/           # (Optional) Any additional assets
```

## How It Works

### Terrain Generation
Mountains are generated using a combination of sine and cosine functions with multiple frequency layers to create natural-looking elevation maps.

### Aurora Effects
The aurora uses a custom shader with animated Perlin noise, creating flowing curtains of color that respond to time-based uniforms.

### Stars and Particles
An optimized point-cloud system renders thousands of stars with individual flickering animations. Shooting stars are generated as line segments with fade effects.

### Water Simulation
The water uses Three.js's built-in Water shader with procedurally generated normal maps for realistic surface movement.

## Performance Considerations

- Uses `antialias: false` for better performance on lower-end devices
- Employs `powerPreference: "high-performance"` to utilize dedicated GPUs
- Efficiently manages particle lifecycles to prevent memory leaks
- Uses additive blending for light effects

## Future Enhancements

- Add multiple viewing locations (space, underwater perspectives)
- Interactive UI elements for customization
- Mobile touch controls optimization
- VR/WebXR support

## License

This project is open source and available under the MIT License.

## Author

Created as an interactive artistic experience. A stunning blend of procedural generation, shader programming, and creative visualization.

---

**Explore the Moonverse** - Where moonlight meets imagination ✨
