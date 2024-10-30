# DAY_029 | Minimalist Portfolio Landing Page with GSAP Animations

## Project Overview

For **DAY_029** of my daily code challenge series, I created a **minimalist portfolio landing page** using **HTML**, **CSS**, **JavaScript**, and **GSAP**. This landing page features a clean, modern design with smooth scale animations, elegant typography, and a dynamic layout. The project demonstrates sophisticated use of flexbox layouts, GSAP animations, and minimalist design principles to create a striking, professional portfolio introduction.

---

## Preview

![DAY_029_1](./assets/DAY_029_1.gif)

## Inspiration

This project was inspired by my desire to create a portfolio landing page that combines minimalist design with dynamic animations. I wanted to create a strong first impression by using bold typography, clean layouts, and smooth transitions while maintaining a professional aesthetic.

---

## Key Features

- **Minimalist Design**: Clean black and white color scheme with bold typography.
- **Smooth Scale Animations**: GSAP-powered animations for seamless page loading and transitions.
- **Dynamic Content Sections**: Well-organized content areas with clear visual hierarchy.
- **Interactive Elements**: Hover states and clickable components for enhanced user engagement.
- **Social Media Integration**: Seamlessly integrated social media links with hover animations.

---

## JavaScript and Animation Details

### JavaScript Libraries Used

1. **GSAP (GreenSock Animation Platform)**:
   - Manages initial page load animations and content transitions.
2. **Ion Icons**:
   - Provides scalable icons for social media links and navigation elements.

### Animation Implementation

The page utilizes GSAP for smooth, professional animations that enhance the user experience without overwhelming the content.

#### Key Code for Initial Animation

```javascript
gsap.from("nav > div, .col", 2, {
  delay: 1,
  scale: 0,
  ease: "power3.inOut",
  stagger: {
    amount: 0.3
  },
  onComplete: () => {
    gsap.from(".social-links", {
      opacity: 0,
      y: 30,
      duration: 1,
      ease: "power3.out"
    });
  }
});
```

### Layout Structure

The layout uses a sophisticated flexbox structure to create a balanced, visually appealing design.

#### Code for Main Layout Structure

```css
.container {
  width: 100%;
  height: 100vh;
  display: flex;
  flex-direction: column;
  gap: 0.25em;
}

.content-wrapper {
  flex: 12;
  width: 100%;
  height: 100%;
  display: flex;
  padding: 0 0 0.5em 0;
  gap: 0.25em;
  background: #000;
}
```

---

## How to Run

1. **Clone the repository**:
   ```bash
   git clone https://github.com/thounny/DAY_029.git
   ```

2. **Navigate to the project directory**:
   ```bash
   cd DAY_029
   ```

3. **Open the `index.html` file** in your browser, or use a local development server like **Live Server** in VSCode.

---

## Project Structure

```bash
DAY_029/
│
├── assets/
├── fonts/
│   └── helveticaneue.woff2
├── index.html
└── styles.css
```

---

## Technologies Used

- **HTML5**: Provides the structural foundation for the landing page.
- **CSS3**: Handles styling, flexbox layout, and visual effects.
- **JavaScript (ES6)**: Manages animations and interactive elements.
- **GSAP (GreenSock Animation Platform)**: Powers the smooth animations and transitions.
- **Ion Icons**: Provides scalable vector icons for UI elements.

---

## Author

![Logo](./assets/index_dwn.gif)

**Thounny Keo**  
Creative Developer & Designer  
Frontend Development Student | Year Up United

---

![moon](./assets/miku.gif)
