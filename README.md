# Vivek Rajendra Patil - Portfolio Website

[![GitHub Pages](https://img.shields.io/badge/Hosted%20on-GitHub%20Pages-orange)](https://github.com/vivek-patil/portfolio)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

A modern, bilingual (English/German) portfolio website showcasing expertise in CAD design, vehicle technology, and metal forming simulations.

## Features

- **Bilingual Support**: Seamlessly switch between English and German
- **Responsive Design**: Optimized for desktop, tablet, and mobile devices
- **Modern UI/UX**: Clean, professional design with smooth animations and orange/amber color theme
- **Fast Loading**: Lightweight and optimized for performance
- **GitHub Pages Ready**: Easy deployment on GitHub Pages

## Sections

1. **Hero/Home**: Professional introduction and quick links
2. **About**: Academic and professional background with key achievements
3. **Skills**: Technical skills organized by category:
   - CAD & 3D Modeling (Siemens NX, CATIA V5, Solidworks, Blender)
   - Simulation & Analysis (DEFORM, Q-Form, Star CCM+)
   - Vehicle Engineering
   - Manufacturing & Materials
4. **Projects**: 6 featured projects including:
   - Mercedes Benz Luxury Concept Vehicle
   - Hybrid Metal-Plastic Forming Research
   - Metal Forming Simulation & Optimization (75% time reduction)
   - Formula Student E-Racing Car
   - Advanced CAD Techniques
   - Large Heat Pump Analysis (Bachelor Thesis)
5. **Experience**: Professional timeline with detailed work history from Institute for Metal Forming Technology, Mercedes Benz, and Formula Student
6. **Contact**: Multiple ways to get in touch

## Technologies Used

- **HTML5**: Semantic markup with bilingual support
- **CSS3**: Modern styling with CSS Grid, Flexbox, and animations
- **JavaScript**: Interactive features and language switching
- **Font Awesome**: Professional icons
- **Git**: Version control
- **GitHub Pages**: Hosting platform

## Setup Instructions

### Local Development

1. **Clone the repository**
   ```bash
   git clone https://github.com/YOUR_USERNAME/vivek-portfolio.git
   cd vivek-portfolio
   ```

2. **Open in browser**
   Simply open `index.html` in your web browser:
   - **Windows**: Double-click `index.html` or right-click > Open with > Browser
   - **Mac/Linux**: `open index.html` or drag to browser

3. **Local Server (Optional)**
   For better development experience, use a local server:

   Using Python:
   ```bash
   # Python 3
   python -m http.server 8000

   # Python 2
   python -m SimpleHTTPServer 8000
   ```

   Then open: `http://localhost:8000`

   Using Node.js (with `http-server`):
   ```bash
   npx http-server
   ```

   Using VS Code:
   - Install "Live Server" extension
   - Right-click `index.html` > "Open with Live Server"

## Deployment to GitHub Pages

### Method 1: GitHub Repository Settings (Recommended)

1. **Create a GitHub repository**
   - Go to GitHub and create a new repository named 'vivek-portfolio'

2. **Push your code**
   ```bash
   git remote add origin https://github.com/YOUR_USERNAME/vivek-portfolio.git
   git add .
   git commit -m "Initial commit: CAD Designer Portfolio"
   git branch -M main
   git push -u origin main
   ```

3. **Enable GitHub Pages**
   - Go to your repository on GitHub
   - Click "Settings" > "Pages"
   - Under "Source", select "main" branch
   - Click "Save"
   - Your site will be published at: `https://YOUR_USERNAME.github.io/vivek-portfolio/`

### Method 2: Using as User/Organization Site

1. **Create a repository named**: `YOUR_USERNAME.github.io`

2. **Push your code**
   ```bash
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_USERNAME.github.io.git
   git add .
   git commit -m "Initial commit"
   git push -u origin main
   ```

3. **Access your site** at: `https://YOUR_USERNAME.github.io`

## Customization

### Update Personal Information

1. **Contact Details** ([index.html](index.html)):
   - Email: Update `vvrpatil41@gmail.com`
   - Phone: Update `+49 176 34698220`
   - LinkedIn: Add your profile URL
   - GitHub: Add your GitHub username
   - Location: Update as needed

2. **Projects**:
   - Edit project cards in the "Projects Section" of `index.html`
   - Add/remove projects as needed
   - Update project descriptions, features, and tags
   - Customize the featured project

3. **Experience**:
   - Update timeline items in the "Experience Section"
   - Add new positions or remove old ones
   - Adjust dates and responsibilities

4. **Skills**:
   - Edit skill categories and tags in the "Skills Section"
   - Add or remove technical skills based on your expertise

### Styling Customization

Edit [css/styles.css](css/styles.css) to customize:

- **Colors**: Modify CSS variables in `:root`
  ```css
  :root {
      --primary-color: #f97316;     /* Orange */
      --secondary-color: #ea580c;   /* Darker orange */
      --accent-color: #fb923c;      /* Light orange */
      /* ... other colors */
  }
  ```

- **Fonts**: Change font families
- **Animations**: Adjust animation speeds and effects
- **Layout**: Modify grid layouts and spacing

### Adding New Language

To add a third language (e.g., Hindi):

1. Add language button in HTML:
   ```html
   <button onclick="switchLanguage('hi')" class="lang-btn" id="lang-hi">HI</button>
   ```

2. Add `data-hi` attributes to translatable elements:
   ```html
   <h1 data-en="About" data-de="Über mich" data-hi="के बारे में">About</h1>
   ```

3. Update [js/script.js](js/script.js) if needed

## Project Structure

```
vivek-portfolio/
│
├── index.html              # Main HTML file with bilingual content
├── README.md              # This file
├── LICENSE                # MIT License
├── .gitignore             # Git ignore file
│
├── css/
│   └── styles.css         # All styles with orange theme
│
├── js/
│   └── script.js          # JavaScript functionality
│
├── images/                # Images folder (add your images here)
│   └── (your project images)
│
└── assets/                # Additional assets
    └── (other files)
```

## Features in Detail

### Language Switching
- Toggle between English and German with a single click
- Language preference saved in localStorage
- Keyboard shortcut: Press 'L' to switch languages
- All content seamlessly translated

### Responsive Design
- Mobile-first approach
- Hamburger menu on mobile devices
- Optimized layouts for all screen sizes
- Touch-friendly interactions

### Performance
- Minimal dependencies (only Font Awesome for icons)
- Optimized CSS with efficient selectors
- Lazy loading for animations
- Debounced scroll events for smooth performance

### Accessibility
- Semantic HTML5 markup
- ARIA labels for screen readers
- Keyboard navigation support
- High contrast text for readability

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Opera (latest)

## Customization Tips

### Adding Your Own Projects

To add a new project, copy this template in the Projects section:

```html
<div class="project-card">
    <div class="project-icon">
        <i class="fas fa-icon-name"></i>
    </div>
    <h3 data-en="Project Name English" data-de="Projektname Deutsch">Project Name</h3>
    <p data-en="English description" data-de="Deutsche Beschreibung">Description</p>
    <div class="project-tags">
        <span>Tag1</span>
        <span>Tag2</span>
    </div>
</div>
```

### Adding Images

1. Place your images in the `images/` folder
2. Reference them in HTML:
   ```html
   <img src="images/project-screenshot.jpg" alt="Project Screenshot">
   ```

## License

This project is open source and available under the [MIT License](LICENSE).

## Contact

**Vivek Rajendra Patil**
- Email: vvrpatil41@gmail.com
- Phone: +49 176 34698220
- Location: Stuttgart, Germany
- University: Universität Stuttgart
- Program: M.Sc. Fahrzeugtechnik (Vehicle Technology)

---

**Note**: Remember to replace `YOUR_USERNAME` with your actual GitHub username in all URLs and commands.

## Troubleshooting

### Site not loading on GitHub Pages
- Ensure the repository is public
- Check that GitHub Pages is enabled in Settings
- Wait a few minutes after enabling (initial deployment takes time)
- Clear browser cache and try again

### Language switching not working
- Check browser console for JavaScript errors
- Ensure `js/script.js` is properly linked in HTML
- Verify `data-en` and `data-de` attributes are present on elements

### Styles not applying
- Check that `css/styles.css` path is correct
- Verify file structure matches expected layout
- Clear browser cache and hard reload (Ctrl+Shift+R)

### Mobile menu not working
- Ensure JavaScript is enabled in browser
- Check that Font Awesome is loading correctly
- Verify hamburger menu code is intact

## Future Enhancements

- [ ] Add dark mode toggle
- [ ] Include CAD model viewer (e.g., three.js for 3D models)
- [ ] Add project detail pages with more screenshots
- [ ] Include downloadable resume/CV PDF
- [ ] Add contact form with backend
- [ ] Integrate Google Analytics for visitor tracking
- [ ] Add more interactive 3D visualizations
- [ ] SEO optimization
- [ ] Blog section for design insights

---

Built with ❤️ for showcasing CAD design and vehicle engineering expertise.
