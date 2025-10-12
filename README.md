# 📁 Folder Hover Animation

- A smooth and visually appealing **folder hover animation** built using **HTML**, **Tailwind CSS**, and **GSAP (GreenSock Animation Platform)**. <br>  
- When you hover over a folder, it gracefully lifts upward and reveals a stack of images that fan out and rotate — just like opening a digital folder on your desktop!

---

## 🪄 Live Demo
> [🔗 View Demo](https://folder-hover-animation.netlify.app/)

---

## ✨ Features

- 🎨 **Clean UI** inspired by :- https://www.wildyriftian.com/works  
- ⚡ **GSAP-powered animations** for buttery-smooth motion  
- 📱 **Responsive design** — animations only trigger on desktop view (auto-disabled on mobile)  
- 💫 **Dynamic effects** with randomized rotation for natural variation  
- 🧠 **Efficient and reusable code** that handles multiple folders dynamically  
- 🧩 **Built using modern tools**: Tailwind CSS + GSAP  

---

## 🧰 Tech Stack

| Technology | Purpose |
|-------------|----------|
| **HTML5** | Page structure |
| **Tailwind CSS** | Styling & responsiveness |
| **JavaScript (ES6)** | Interactivity |
| **GSAP (GreenSock)** | Animation engine |

---

## 📂 Folder Structure
folder-hover-animation <br>
│<br>
├── index.html # Main HTML structure <br>
├── main.js # GSAP animation logic <br>
└── style.css 


---

## ⚙️ How It Works

### 🖱️ 1. Hover Detection
Each `.folder` listens for `mouseenter` and `mouseleave` events.  
When hovered:
- The folder slightly **lifts upward**.
- Sibling folders become dimmed (`disabled` class applied).

### 🎞️ 2. GSAP Animations
The `.folder-wrapper` animates vertically (`y: 0 → 25px`) using a smooth **back-out** easing.  
Each folder’s preview images:
- Move upward (`y: -100%`)
- Rotate slightly using random angles (`gsap.utils.random()`)
- Animate with small **delays** to create a natural stagger effect.

### 📱 3. Responsive Logic
On mobile (`<1024px`):
- Animations are disabled for performance and UX.
- Preview images remain hidden (`hidden lg:inline-block` in Tailwind).

### 🔄 4. Resize Handling
When the browser is resized:
- The script checks if the screen crosses the mobile/desktop breakpoint.
- Resets folder positions and clears any leftover animation states.

---

> ⭐ Don’t forget to star this repo if you found it helpful!
