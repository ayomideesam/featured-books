# Featured Books

> **Fat Bee-Hive Technical Assessment** - Implementation of a responsive featured books UI component using HTML, CSS/SCSS, and BEM methodology.

## 🎯 Project Overview

This project recreates a Figma design specification for a featured books showcase, implementing a clean and modern card-based layout. The component displays books in a 2x2 grid on desktop devices and adapts to a single-column layout on mobile devices, with smooth hover animations and accessible interactions.

**Live Demo**: [View Project](https://ayomideesam.github.io/featured-books)

## ✨ Features Implemented

### 🎨 Visual Design
- **Responsive Grid Layout**: 2 columns on desktop/tablet, 1 column on mobile, 3 columns on TV/large displays
- **Card-Based Interface**: Horizontal layout with image placeholder, content area, and call-to-action button
- **Consistent Card Heights**: Equal-height cards across all grid layouts with proper content distribution
- **Smooth Hover Effects**: Card elevation, shimmer animations, and button ripple effects
- **Modern Typography**: Inter font family with multiple weights for visual hierarchy

### 🔧 Technical Implementation
- **SASS/SCSS**: Modular CSS with variables, mixins, and nested selectors
- **BEM Methodology**: Block Element Modifier naming convention for maintainable and reusable components
- **Local Font Hosting**: Self-hosted Inter webfonts for improved performance and privacy
- **Mobile-First Design**: Progressive enhancement approach from mobile to desktop
- **Semantic HTML**: Proper use of semantic elements and ARIA attributes for accessibility
- **Advanced Grid Management**: CSS Grid with grid-auto-rows: 1fr for consistent card heights
- **Smart Text Handling**: Overflow protection and hyphenation for long content

## 📋 Requirements Checklist

All specified requirements have been successfully implemented:

- ✅ **Figma Recreation**: Pixel-perfect implementation using HTML/CSS/SASS without frameworks
- ✅ **Responsive Design**: Mobile-first approach with smooth breakpoint transitions
- ✅ **80rem Max Width**: Container properly constrained with rem units throughout
- ✅ **Local Webfonts**: Inter font hosted locally (no external CDN dependencies)
- ✅ **Creative Hover States**: Custom card and button animations with smooth transitions
- ✅ **Clickable Cards**: Full card interactivity with proper accessibility support
- ✅ **BEM Methodology**: Consistent naming convention for scalable component architecture
- ✅ **Cross-Device Compatibility**: Optimized layouts for mobile, tablet, desktop, and TV screens

## 📁 File Structure
- featured-books/
- ├── 📄 index.html              # Main HTML document
- ├── 📁 css/
- │   ├── 📄 styles.css          # Compiled CSS output // this is been used
- │   └── 📄 styles.scss         # Source SCSS file with variables and mixins // not been used
- ├── 📁 fonts/
- │   └── 📄 inter.css           # Local Inter font definitions
- ├── 📁 assets/                 # Project assets (recommended)
- │   ├── 📄 favicon.ico         # Site favicon
- │   └── 📄 preview.png         # Project screenshot
- ├── 📄 LICENSE                 # Project license
- └── 📄 README.md               # Project documentation

## 🚀 Getting Started

### Prerequisites
- Modern web browser (Chrome 88+, Firefox 85+, Safari 14+, Edge 88+)
- Code editor (VS Code recommended)
- SASS compiler (for development)

### Quick Setup

1. **Clone the repository**
    ```bash
    git clone https://github.com/ayomideesam/featured-books.git
    cd featured-books
2. **Set up local fonts**
    The Inter font files should be downloaded and placed in the /fonts/ directory:

    Use Google Webfonts Helper
    Select charsets: latin
    Select styles: 400, 500, 600, 700
    Place downloaded files alongside inter.css

## 🎨 Design Specifications

### 🎯 What I've Implemented:

#### 📱 Responsive Image Dimension Text

- Mobile (default): Shows "220×150" text with 220px container width and 150px image height
- Tablet+ (48rem+): Shows "150×220" text with 150px container width and 220px image height
- Visual Consistency: Image dimensions perfectly match the displayed text across all breakpoints
- Added CSS classes .card__image-text--desktop and .card__image-text--mobile for responsive text switching

#### 📺 TV-Only Cards (Cards 5 & 6)

- Hidden by Default: Cards 5 & 6 use .card--tv-only class and are hidden on smaller screens
- Large Display Activation: Only appear on 90rem+ screens (TV/large display sizes)
- Enhanced Layout: 3×2 grid layout (3 columns, 2 rows) on TV screens for optimal viewing

### 📐 Layout
- Container: Max-width 80rem, centered with responsive padding
- Grid System: CSS Grid with repeat(3, 1fr) on Tvs or Large Monitors/Desktop, Double or 2 columns on laptops/tablets, single column on mobile.
- Card Structure: Flexbox horizontal layout with image container and content area.
- Spacing: Consistent rem-based spacing that scales across breakpoints.

### 📱 Responsive Breakpoints
    scss// Mobile First Approach with Enhanced Stability
    $mobile-small: 20rem;      // 320px - Small mobile adjustments
    $mobile-large: 36rem;      // 576px - Large mobile optimization
    $tablet: 48rem;            // 768px - 2-column grid with enhanced card stability
    $desktop: 62rem;           // 992px - Increased spacing and sizing
    $large: 75rem;             // 1200px - Maximum optimized layout
    $xl: 87.5rem;              // 1400px - Extra large displays
    $ultra: 115rem and above;  // 1600px - Ultra-wide displays, screens with 3-column layout

### 🎨 Color Palette
    // Primary Colors
    $primary-blue: #3b82f6;        // Button background
    $primary-blue-hover: #2563eb;  // Button hover state

    // Text Colors  
    $text-dark: #1f2937;           // Headings and titles
    $text-medium: #6b7280;         // Body text and descriptions
    $text-light: #9ca3af;          // Placeholder text

    // Background Colors
    $white: #ffffff;               // Card backgrounds
    $gray-light: #f3f4f6;          // Image placeholders
    $gray-lighter: #fafafa;        // Page background

    // Border Colors
    $border-default: #e5e7eb;      // Card borders
    $border-hover: #d1d5db;        // Card border on hover

### 📝 Typography Scale

    Main Heading: 3rem - 4.5rem (responsive)
    Card Titles: 1.5rem - 1.625rem
    Descriptions: 0.875rem - 0.9375rem
    Button Text: 0.875rem
    Font Weights: 400 (regular), 500 (medium), 600 (semibold), 700 (bold)

### 📱 Responsive Breakpoints
    // Mobile First Approach
    $mobile: 20rem;      // 320px - Small mobile adjustments
    $tablet: 48rem;      // 768px - Switch to 2-column grid
    $desktop: 62rem;     // 992px - Increased spacing and sizing
    $large: 75rem;       // 1200px - Maximum optimized layout
    $xl: 87.5rem;        // 1400px - Extra large displays

## ⚡ Performance Optimizations

### Loading Performance

- Local Font Hosting: Eliminates external DNS lookups and reduces FOUT
- Minimal CSS: Only essential styles, no framework bloat
- Efficient Selectors: Optimized CSS for fast parsing and rendering

### Runtime Performance

- Hardware Acceleration: CSS transforms and opacity for smooth animations
- Efficient Repaints: Animations target composite layers only
- Memory Management: No JavaScript means no memory leaks or garbage collection

### ♿ Accessibility Features

- Semantic HTML: Proper use of <main>, <article>, and heading hierarchy
- ARIA Labels: Descriptive labels for interactive elements
- Keyboard Navigation: Full keyboard accessibility with visible focus indicators
- Screen Reader Support: Logical content flow and descriptive text
- Color Contrast: WCAG AA compliant color combinations
- Reduced Motion: Animation preferences respected

## 🐛 Known Issues & Solutions

### Font Loading
    Issue: Fonts may flash during initial load
    Solution: Ensure local server is used for development to properly load webfonts
    Mobile Safari
    Issue: Hover states can stick on mobile Safari
    Solution: Touch events are properly handled with CSS :hover specificity

## 📝 License
    This project is created for the Fat Bee-Hive technical assessment. Please refer to the LICENSE file for usage terms.

## 🤝 Contributing
    This is a technical assessment project, but feedback and suggestions are welcome:

## Fork the repository
- Create a feature branch (git checkout -b feature/improvement)
- Commit your changes (git commit -am 'Add some improvement')
- Push to the branch (git push origin feature/improvement)
- Create a Pull Request

## 📧 Contact
    For questions about this implementation, please reach out through the assessment process or create an issue in this repository.