# Interactive Card Grid

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)

A modern, responsive card grid system with advanced features like quick-access drawers, real-time search, and dynamic pagination. Built with HTML5, JavaScript, and Tailwind CSS.

## ✨ Features

- 🎯 **Responsive Grid Layout**: Adapts seamlessly from mobile to desktop (1-5 columns)
- 🔍 **Real-time Search**: Filter cards by title, description, author, or skill
- 📑 **Smart Pagination**: Dynamic page navigation with smooth scrolling
- 🎨 **Modern UI**: Clean, accessible design with Tailwind CSS
- 📱 **Mobile-First**: Fully responsive on all devices
- 🚀 **Quick Links Drawer**: Slide-in panel for quick access to relevant resources
- ⌨️ **Keyboard Accessible**: Full keyboard navigation support
- 🔄 **Dynamic Data Loading**: JSON-based data management

## 🚀 Quick Start

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/interactive-card-grid.git
   ```

2. Open `index.html` in your browser:
   ```bash
   start index.html   # Windows
   open index.html    # macOS
   xdg-open index.html # Linux
   ```

3. No build steps required! The project uses CDN-loaded Tailwind CSS.

## 💻 Tech Stack

- **HTML5** - Semantic markup
- **JavaScript** - Vanilla JS for interactivity
- **Tailwind CSS** - Utility-first CSS framework
- **JSON** - Data storage and management

## 🏗 Project Structure

```
interactive-card-grid/
├── index.html        # Main application file
├── data.json        # Card data and resources
├── README.md        # Documentation
└── frd_drawer.md    # Drawer feature requirements
```

## Data Structure
The card data is currently hardcoded within the <script> tag in the HTML file as a JavaScript array of objects. Each card object follows this structure:

| Field         | Description                                            |
| ------------- | ------------------------------------------------------ |
| id            | Unique identifier (currently unused but good practice) |
| title         | Main title of the card                                 |
| publishedDate | Date string (e.g., "March 1, 2025")                    |
| description   | Descriptive text content                               |
| linkUrl       | URL the card links to                                  |
| author        | Name of the author/creator                             |
| skill         | Skill category/tag (e.g., "Python", "CSS")             |


## 🔍 Browser Support

- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ✅ Opera (latest)

## 🛠 Future Enhancements

1. 🌐 API Integration
   - Backend API connectivity
   - Real-time data updates
   - Caching layer

2. 🎨 UI/UX Improvements
   - Dark mode support
   - Custom color themes
   - Animation preferences

3. 🔄 Advanced Features
   - Card sorting options
   - Filter combinations
   - Save favorites
   - Share functionality

4. Line Clamp Plugin: Officially include the @tailwindcss/line-clamp plugin (requires a build step or alternative CDN) for more robust description truncation.
5. State Management: For more complex versions, consider a simple state management approach.
6. Accessibility Improvements: Further review and enhance accessibility features (e.g., more descriptive aria-labels, keyboard navigation testing).
7. Loading State: Add a visual indicator while data might be loading (more relevant if fetching from an API).
8. Error Handling: Implement more robust error handling, especially if fetching data externally.

## 📄 License

This project is released under the MIT License.