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
## 6. Three.js

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
