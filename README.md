# 🌟 Beginner-Friendly JavaScript Libraries

A curated list of useful JavaScript libraries for beginners. These libraries help you learn faster, make your projects interactive, and improve your web development skills.

---

## 📦 Utility Libraries

| Library | Description | Example |
|---------|-------------|---------|
| [Lodash](https://lodash.com) | Utilities for arrays, objects, strings, and more | `_.map([1,2,3], n => n*2)` |
| [Axios](https://axios-http.com/) | Promise-based HTTP client | `axios.get("https://jsonplaceholder.typicode.com/todos/1")` |
| [Day.js](https://day.js.org/) | Lightweight date & time manipulation | `dayjs().format("YYYY-MM-DD HH:mm:ss")` |
| [uuid](https://www.uuidgenerator.net/) | Generate unique IDs | `uuidv4()` |

---

## 🎨 Animation & UI Libraries

| Library | Description | Example |
|---------|-------------|---------|
| [GSAP](https://gsap.com/resources/) | Smooth animations | `gsap.to(".box", {x:100, duration:2})` |
| [Framer Motion](https://motion.dev/) | React animations | `<motion.div animate={{x:100}} />` |
| [Anime.js](https://animejs.com/) | Lightweight DOM & SVG animations | `anime({targets: '.box', translateX: 250})` |
| [AOS](https://michalsnik.github.io/aos/) | Scroll animations | `<div data-aos="fade-up"></div>` |
| [ScrollReveal](https://scrollrevealjs.org/) | Scroll animations | `ScrollReveal().reveal('.box', {duration:2000})` |

---

## 📊 Charts & Data Visualization

| Library | Description | Example |
|---------|-------------|---------|
| [Chart.js](https://www.chartjs.org/) | Charts & graphs | `new Chart(ctx, {type:"bar", data:{labels:["A","B"], datasets:[{data:[5,10]}]}})` |
| [D3.js](https://d3js.org/) | Interactive data visualizations | `d3.select('svg').selectAll('rect').data(data).enter().append('rect')` |

---

## ⚛️ React & Frontend Libraries

| Library | Description | Example |
|---------|-------------|---------|
| [React](https://react.dev/) | UI components | `<h1>Hello, React!</h1>` |
| [React Router](https://reactrouter.com/) | Routing in React apps | `<Route path="/about" element={<About />} />` |

---

## 🎵 Audio & Multimedia

| Library | Description | Example |
|---------|-------------|---------|
| [Howler.js](https://howlerjs.com/) | Play audio in browser | `new Howl({src:['sound.mp3']}).play()` |
| [Clipboard.js](https://clipboardjs.com/) | Copy text to clipboard | `new ClipboardJS('.btn')` |
| [Notyf](https://carlosroso.com/notyf/) | Toast notifications | `notyf.success('Success!')` |

---

## 🖼️ Graphics & 3D

| Library | Description | Example |
|---------|-------------|---------|
| [Three.js](https://threejs.org/) | 3D graphics & animations | `new THREE.Mesh(geometry, material)` |
| [Vivus.js](https://maxwellito.github.io/vivus/) | SVG drawing animations | `new Vivus('my-svg', {duration:200})` |

---

## 🛠️ Miscellaneous Libraries

| Library | Description | Example |
|---------|-------------|---------|
| [Owl Carousel 2](https://owlcarousel2.github.io/OwlCarousel2/) | Responsive carousels | `$('.owl-carousel').owlCarousel({loop:true})` |
| [Sortable.js](https://sortablejs.github.io/Sortable/) | Drag-and-drop sorting | `Sortable.create(document.getElementById('items'))` |
| [Jarallax](https://github.com/nk-o/jarallax) | Parallax backgrounds | `jarallax(document.querySelectorAll('.jarallax'), {speed:0.5})` |

---
