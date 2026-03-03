# Beginner-Friendly JavaScript Open Source Libraries

This is a curated list of **useful JavaScript open-source libraries** for beginners. These libraries help you learn faster and make your projects more interactive and professional.

---

## 1. [Lodash](https://lodash.com)

A utility library for **working with arrays, objects, strings, and more**.  
**Example:**
```javascript
import _ from "lodash";

const numbers = [1, 2, 3, 4, 5];
const doubled = _.map(numbers, n => n * 2);
console.log(doubled); // [2, 4, 6, 8, 10]
```

## 2. [Axios](https://axios-http.com/)

A promise-based HTTP client for fetching data from APIs easily.
Example:
```javascript

import axios from "axios";

axios.get("https://jsonplaceholder.typicode.com/todos/1")
  .then(response => console.log(response.data))
  .catch(error => console.error(error));
```

## 3. [Day.js](https://day.js.org/)

A lightweight library for date and time manipulation, alternative to Moment.js.
Example:
``` javascript
import dayjs from "dayjs";

const now = dayjs();
console.log(now.format("YYYY-MM-DD HH:mm:ss"));
```

## 4. [GSAP](https://gsap.com/resources/) (GreenSock Animation Platform)

A powerful animation library for creating smooth web animations.
Example:
```javascript
import gsap from "gsap";

gsap.to(".box", { x: 100, duration: 2 });

```

## 5. [SweetAlert2](https://sweetalert2.github.io/)

A beautiful, customizable alert library for modern web projects.
Example:
``` javascript
import Swal from "sweetalert2";

Swal.fire({
  title: 'Hello!',
  text: 'This is a fancy alert!',
  icon: 'success',
});
```
## 6. [Three.js](https://threejs.org/)

A powerful 3D JavaScript library for creating interactive 3D graphics and animations in the browser.

Example:

``` javascript
import * as THREE from 'three';

// Create scene, camera, renderer
const scene = new THREE.Scene();
const camera = new THREE.PerspectiveCamera(75, window.innerWidth/window.innerHeight, 0.1, 1000);
const renderer = new THREE.WebGLRenderer();
renderer.setSize(window.innerWidth, window.innerHeight);
document.body.appendChild(renderer.domElement);

// Create a cube
const geometry = new THREE.BoxGeometry();
const material = new THREE.MeshBasicMaterial({ color: 0x00ff00 });
const cube = new THREE.Mesh(geometry, material);
scene.add(cube);

camera.position.z = 5;

// Animation loop
function animate() {
    requestAnimationFrame(animate);
    cube.rotation.x += 0.01;
    cube.rotation.y += 0.01;
    renderer.render(scene, camera);
}

animate();
```

## 7 . [D3.js](https://d3js.org/)

A powerful JavaScript library for data visualization — perfect for creating charts, graphs, and interactive visuals in the browser.

Example:
``` html
<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>D3.js Simple Bar Chart</title>
  <script src="https://d3js.org/d3.v7.min.js"></script>
</head>
<body>
  <svg width="500" height="200"></svg>

  <script>
    // Sample data
    const data = [30, 80, 45, 60, 20, 90, 50];

    // Select SVG
    const svg = d3.select('svg');

    // Set scale
    const xScale = d3.scaleBand()
                     .domain(d3.range(data.length))
                     .range([0, 500])
                     .padding(0.1);

    const yScale = d3.scaleLinear()
                     .domain([0, d3.max(data)])
                     .range([0, 200]);

    // Draw bars
    svg.selectAll('rect')
       .data(data)
       .enter()
       .append('rect')
       .attr('x', (d, i) => xScale(i))
       .attr('y', d => 200 - yScale(d))
       .attr('width', xScale.bandwidth())
       .attr('height', d => yScale(d))
       .attr('fill', 'teal');
  </script>
</body>
</html>
```

 ## 8. [React](https://react.dev/)

A JavaScript library for building user interfaces with components.

```javascript
// Import React (if using modules)
import React from "react";
import { createRoot } from "react-dom/client";

function App() {
  return <h1>Hello, React!</h1>;
}

const root = createRoot(document.getElementById("root"));
root.render(<App />);
```

## 9. [Chart.js](https://www.chartjs.org/)

Create graphs and charts.

Best for: Dashboard projects 📊
```javascript
new Chart(ctx, {
  type: "bar",
  data: { labels: ["A","B"], datasets: [{ data: [5,10] }] }
});
```

## 10. [uuid](https://www.uuidgenerator.net/)
Generate unique IDs.

Very useful for:

To-do app

Multi-vendor project
``` javascript
import { v4 as uuidv4 } from "uuid";
uuidv4();
```

## 11. [AOS](https://michalsnik.github.io/aos/)

Animate elements on scroll.

Used for:

Modern landing pages

Portfolio websites

Just add attributes:
```html
<div data-aos="fade-up"></div>
```
## 12. [React Router](https://reactrouter.com/)

For routing in React apps (moving between pages).
```javascript
import { BrowserRouter, Routes, Route } from "react-router-dom";

function App() {
  return (
    <BrowserRouter>
      <Routes>
        <Route path="/" element={<Home />} />
        <Route path="/about" element={<About />} />
      </Routes>
    </BrowserRouter>
  );
}
```

## 13. [Framer Motion](https://motion.dev/)

For animations in React. Very beginner-friendly.
```javascript
import { motion } from "framer-motion";

function App() {
  return (
    <motion.div animate={{ x: 100 }} transition={{ duration: 2 }}>
      Slide me!
    </motion.div>
  );
}
```
 ## 14. [Anime.js](https://animejs.com/)

Lightweight JavaScript animation library for DOM, SVG, and CSS.
```javascript
anime({
  targets: '.box',
  translateX: 250,
  duration: 2000
});
```

## 15. [Howler.js](https://howlerjs.com/)

For audio in the browser.
```javascript
var sound = new Howl({ src: ['sound.mp3'] });
sound.play();
```

## 16. [Clipboard.js](https://clipboardjs.com/)

For copying text to clipboard easily.
```javascript
new ClipboardJS('.btn'); // <button class="btn" data-clipboard-text="Hello!">Copy</button>
```

## 17. [ScrollReveal](https://scrollrevealjs.org/)

For scroll animations.
```javascript
ScrollReveal().reveal('.box', { duration: 2000, origin: 'left', distance: '100px' });
```

## 18. [Notyf](https://carlosroso.com/notyf/)

For beautiful toast notifications.
```javascript
const notyf = new Notyf();
notyf.success('You did it!');
notyf.error('Oops, something went wrong.');
```
## 19. [Owl Carousel 2](https://owlcarousel2.github.io/OwlCarousel2/)

For responsive carousels/sliders.
```javascript
$('.owl-carousel').owlCarousel({ loop:true, margin:10, nav:true });
```


## 20. [Vivus.js](https://maxwellito.github.io/vivus/)

For SVG animations (drawing effect).
```javascript
new Vivus('my-svg', { type: 'delayed', duration: 200 });
```
