# BlackBox Development Team - Website

Modern, interactive landing page for BlackBox Development Team, a nearshore software development company offering elite engineering talent from Latin America.

![BlackBox Website](https://img.shields.io/badge/version-1.0.0-blue.svg)
![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=flat&logo=javascript&logoColor=%23F7DF1E)

## 🌟 Features

### Visual & UX
- **Custom Cursor with Trail Effect** - Elegant gradient trail that follows mouse movement (desktop only)
- **Smooth Scroll Animations** - Reveal animations on scroll with intersection observer
- **Interactive 3D Cube** - Rotating CSS 3D element in hero section
- **Scroll-to-Top Button** - Appears after scrolling 300px with smooth animation
- **Mobile-First Responsive Design** - Optimized for all devices and screen sizes
- **Dark Theme** - Professional dark mode with cyan accent colors

### Sections
1. **Hero** - Eye-catching introduction with animated badge and call-to-action
2. **Stats Bar** - Animated counters showing company achievements (19+ years, 200+ projects, 50+ engineers, 98% retention)
3. **Who We Are** - Company introduction with animated code window
4. **What We Do** - Three service cards with hover effects (Dedicated Teams, Staff Augmentation, Web Development)
5. **Testimonials** - Interactive carousel with client reviews featuring:
   - Overlapping card design
   - Click, keyboard, and dot navigation
   - Auto-play functionality (5s interval)
   - Pause on hover
6. **Contact** - Functional form with Web3Forms integration
7. **Footer** - Company info and links

### Interactive Elements
- **Hamburger Menu** - Mobile navigation with smooth animations
- **Testimonials Carousel**:
  - Click on any visible card to navigate
  - Arrow buttons for prev/next
  - Dot indicators
  - Keyboard navigation (←/→)
  - Auto-play with pause on hover
- **Contact Form** - Integrated with Web3Forms API
- **Hover Effects** - Cards, buttons, and interactive elements with smooth transitions

## 🎨 Design System

### Color Palette
```css
Primary: #1eabca (Cyan)
Primary Dark: #178fa8
Primary Light: #4fc3dc
Accent: #00ff88 (Neon Green)
Dark: #020202
Dark Soft: #0a0a0a
Dark Card: #111111
Secondary: #c3c3c3
```

### Typography
- **Primary Font**: Outfit (Google Fonts)
- **Monospace Font**: Space Mono (Google Fonts)

### Gradients
- Primary gradient for buttons and accents
- Mesh gradient for backgrounds
- Radial gradients for glows and depth

## 🚀 Technologies

- **HTML5** - Semantic markup
- **CSS3** - Custom properties, Grid, Flexbox, Animations
- **Vanilla JavaScript** - No dependencies
- **Web3Forms** - Form submission handling
- **Google Fonts** - Outfit & Space Mono

## 📱 Responsive Breakpoints

- **Desktop**: > 1200px
- **Tablet**: 768px - 1199px
- **Mobile**: < 768px
- **Small Mobile**: < 480px

## 🛠️ Setup & Usage

### Basic Setup
1. Clone the repository:
```bash
git clone https://github.com/mdeiriondo/BBXDevs.git
cd BBXDevs
```

2. Open `index.html` in your browser or use a local server:
```bash
# Using Python
python -m http.server 8000

# Using Node.js (http-server)
npx http-server

# Using PHP
php -S localhost:8000
```

3. Visit `http://localhost:8000`

### Configuration

#### Update Contact Form
Replace the Web3Forms access key in `index.html`:
```html
<input type="hidden" name="access_key" value="YOUR_ACCESS_KEY_HERE">
```
Get your free access key at [Web3Forms](https://web3forms.com)

#### Update Content
- **Company Info**: Edit text in HTML sections
- **Testimonials**: Modify the testimonial cards in the testimonials section
- **Stats**: Update numbers in the stats bar
- **Services**: Edit service cards content

#### Styling
All styles are in the `<style>` tag in the HTML file. Key CSS variables are at the top:
```css
:root {
    --primary: #1eabca;
    --dark: #020202;
    /* ... */
}
```

## 📂 File Structure

```
BBXDevs/
├── index.html              # Main HTML file (includes CSS & JS)
├── favicon.png             # Favicon (not included, add your own)
├── README.md               # This file
└── .git/                   # Git repository
```

## 🎯 Key Components

### Custom Cursor
Desktop-only feature with 8 trailing elements creating a smooth gradient effect:
- Main cursor: 20px circle with primary border
- Trail elements: Decreasing opacity and scale
- Hover state: Expands to 40px on interactive elements

### Testimonials Carousel
Sophisticated overlapping card design:
- 3 cards: active (center), prev (left), next (right)
- Smooth transitions with cubic-bezier easing
- Multiple navigation methods
- Responsive: Shows only active card on mobile

### Scroll Animations
Elements with `.reveal` class animate into view:
- Initial state: `opacity: 0, translateY(50px)`
- Active state: `opacity: 1, translateY(0)`
- Triggered when element is 150px into viewport

## 🌐 Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

**Note**: Custom cursor is disabled on touch devices for better UX.

## 📈 Performance

- **Single File** - No external dependencies
- **Optimized CSS** - CSS Grid and Flexbox
- **Vanilla JS** - No framework overhead
- **Lazy Loading** - Animations trigger on scroll
- **Mobile Optimized** - Reduced effects on mobile

## 🔧 Customization Tips

### Change Colors
Edit CSS variables in `:root`:
```css
--primary: #YOUR_COLOR;
--dark: #YOUR_DARK_COLOR;
```

### Add/Remove Testimonials
1. Duplicate a testimonial card
2. Update `data-index` attribute
3. Add corresponding dot indicator
4. Update `totalTestimonials` in JS (auto-detected)

### Modify Animations
Adjust timing in CSS:
```css
transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
```

### Disable Custom Cursor
Remove or comment out:
```css
body { cursor: none; }
```

## 📝 License

This project is private and proprietary to BlackBox Development Team.

## 👥 Contact

- **Website**: [Visit Site](#)
- **Email**: info@bbxdevs.com
- **GitHub**: [@mdeiriondo](https://github.com/mdeiriondo)

## 🙏 Acknowledgments

- Fonts: [Google Fonts](https://fonts.google.com)
- Form Service: [Web3Forms](https://web3forms.com)
- Icons: SVG inline graphics

---

**Built with ❤️ by BlackBox Development Team**
