<div align="center">

  <h1>💠 NEXUS Admin Dashboard</h1>
  
  <p>
    A modern, fully responsive <strong>Admin Dashboard</strong> interface designed to master <strong>CSS Grid</strong> architecture.
    <br>
    This project moves away from basic layouts, implementing a "Hybrid Architecture" that combines the structural power of Grid 
    with the flexibility of Flexbox, all wrapped in a professional <strong>Dark Mode</strong> aesthetic.
  </p>

  <p>
    <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" />
    <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" />
    <img src="https://img.shields.io/badge/Layout-Grid_%2B_Flexbox-8A2BE2?style=for-the-badge" alt="Grid + Flexbox" />
  </p>

  <h3>
    <a href="https://andrewtechtips.github.io/admin-dashboard/">📊 VIEW LIVE DEMO</a>
  </h3>
</div>

<br />

---

## ✨ Key Features

* **📐 Hybrid Layout Architecture:** I utilized **CSS Grid** (`grid-template-areas`) to map out the macro-structure (Sidebar vs. Main Content) and **Flexbox** to perfectly align internal components.
* **🌑 Professional Dark Mode:** Built with a sophisticated color palette using CSS Variables (`--bg-body`, `--bg-sidebar`) to reduce eye strain and look premium.
* **📱 Fluid Responsiveness:** Instead of relying solely on media queries, I used modern CSS functions like `clamp()` and `minmax()` to make the sidebar and card grid adapt smoothly to any screen width.
* **💎 Glassmorphism Header:** The top navigation features a sticky positioning with `backdrop-filter: blur(16px)`, creating a sleek frosted-glass effect over scrolling content.
* **🎨 High-Quality Icons:** Integrated **Material Design Icons (MDI)** via CDN instead of basic emojis, ensuring a consistent and professional look throughout the UI.

---

## 🛠️ Technical Highlights

The core strength of this project is the layout logic. Here is how the main grid is orchestrated:

### 1. Grid Template Areas
This approach makes the layout semantic and incredibly easy to manage:
```css
.container {
    display: grid;
    /* Sidebar cleverly resizes between 240px and 280px based on viewport */
    grid-template-columns: clamp(240px, 20vh, 280px) 1fr;
    grid-template-rows: auto 1fr;
    grid-template-areas: 
        "sidebar header"
        "sidebar main";
    min-height: 100vh;
}
```

### 2. Status Badge System
I implemented a modular CSS class system for project statuses, allowing for easy scalability:
```css
.status-live { 
    background: rgba(34, 197, 94, 0.15); 
    color: #4ade80; 
    border: 1px solid rgba(34, 197, 94, 0.3); 
}
```

## 🎨 Resources Used

* **Icons:** [Material Design Icons (MDI)](https://materialdesignicons.com/) - Accessed via CDN to replace standard emojis with professional vector icons.
* **Fonts:** [Outfit](https://fonts.google.com/specimen/Outfit) - Hosted on Google Fonts, selected for its modern and clean geometric look.
* **Avatars:** [DiceBear API](https://www.dicebear.com/) - Used to generate consistent and dynamic SVG profile pictures for the user interface.

## 🚀 Getting Started

To explore the dashboard layout locally on your machine:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/AndrewTechTips/admin-dashboard.git]
    ```

2.  **Run the project:**
    Navigate to the project folder and simply open the `index.html` file in your preferred web browser. No installation or build steps are required!

---

## 📬 Contact

If you want to contact me, you can reach me at:

* **LinkedIn:** www.linkedin.com/in/andrei-condrea-b32148346
* **Email:** condrea.andrey777@gmail.com


<p align="center">
 <i>Built with focus and grid-gap. 💠</i>
</p>