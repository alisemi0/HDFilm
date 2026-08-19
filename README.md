<div align="center">

# 🍿 HDFilm - Premium Cinema Platform Interface
**Modern, Fast and Customizable Movie Showcase**

[![Live Preview](https://img.shields.io/badge/🔴_Click_For_Live_Preview-E50914?style=for-the-badge&logo=netflix&logoColor=white)](https://proje1-dizi.blogspot.com/)

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)](#)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)](#)
[![ES6 JavaScript](https://img.shields.io/badge/ES6_Vanilla_JS-F7DF1E?style=flat-square&logo=javascript&logoColor=black)](#)
[![CodEX Town](https://img.shields.io/badge/Developer-CodEX_Town-00a8ff?style=flat-square)](#)

*A preview project for a user experience-focused, SEO-friendly, and fully flexible movie/series platform.*

</div>

---

## 📸 Screenshots

| Homepage (Grid Structure) | Movie Details Page | Mobile View |
| :---: | :---: | :---: |
| ![Homepage](https://iili.io/qKeTBYN.png) | ![Details](https://iili.io/qKeAihX.png) | ![Mobile](https://iili.io/qKe7hp2.png) |

---

## ✨ Featured Advanced Features

### 🎨 UI/UX Design Architecture
* **Flawless Grid & Flexbox Architecture:** An intelligent grid system that automatically scales movie posters to the screen width of the device (Responsive).
* **Cinematic Hover Effects:** Summary information, IMDB ratings, and play buttons appear with a smooth "Glassmorphism" effect when hovering over the posters.
* **Dynamic Category Filtering:** A smart menu that works without refreshing the page, allowing users to instantly switch between genres such as action, comedy, and science fiction.
* **Built-in Dark Mode Infrastructure:** A color palette designed using CSS Variables, allowing one-click switching between day and night modes.

### ⚡ Performance and Integration
* **Fast Loading (Lazy Loading):** A browser-based lazy loading strategy that ensures high-resolution movie posters only load when they are displayed on the screen.
* **Full CodeX Player Compatibility:** 100% integrated with our sister project `CodEX Player`, offering zero latency and HLS support on movie detail pages.
* **Blogger & CMS Compatible:** Thanks to its pure (vanilla) structure without complex frameworks, it can be easily integrated into Blogger theme XMLs or systems like WordPress.

---

## 💻 Core Code Architecture

HDFilm is developed in accordance with clean code standards. Here are some examples of the architecture working in the background:

### 1. Dynamic Filtering Logic (`app.js`)
A lightweight JS engine that uses `data-category` attributes, allowing users to filter movies by genre in seconds.

---

## ☕ Support Us

If you found this project useful and would like to support me in continuing its development:

* [Sponsor on GitHub](https://github.com/sponsors/alisemi0)
* [Become a Supporter](https://www.alisemi.dev/p/destek.html)

---

```javascript
const filterButtons = document.querySelectorAll('.filter-btn');
const movieCards = document.querySelectorAll('.movie-card');

filterButtons.forEach(button => { 
button.addEventListener('click', () => { 
// Update active button style 
document.querySelector('.filter-btn.active').classList.remove('active'); 
button.classList.add('active'); 

const filterValue = button.getAttribute('data-filter'); 

movieCards.forEach(card => { 
if (filterValue === 'all' || card.getAttribute('data-category').includes(filterValue)) { 
card.style.display = 'block'; // or an animated class can be added 
setTimeout(() => card.style.opacity = '1', 50); 
} else { 
card.style.opacity = '0'; 
setTimeout(() => card.style.display = 'none', 300);
}
});
});
});
```

<div align="center">

<p><b>Coded with creativity and passion by Ali Semi</b>.</p>
</div>
