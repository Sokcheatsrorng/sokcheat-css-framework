# FlexFrame CSS Framework

A modern, utility-first CSS framework designed for rapid development with cutting-edge features and comprehensive browser compatibility.

## Features

### 🎨 Design System
- **Comprehensive Design Tokens**: Color palettes, spacing scales, typography, and more
- **CSS Custom Properties**: Easy theming and customization
- **Dark Mode Support**: Automatic system preference detection
- **Accessibility First**: WCAG compliant components and utilities

### 🚀 Modern CSS Features
- **Container Queries**: Responsive design based on container size
- **Cascade Layers**: Better CSS organization and specificity control
- **CSS Grid & Flexbox**: Modern layout systems
- **Custom Properties**: Dynamic theming capabilities

### 🌐 Cross-Browser Support
- **Browser-Specific Utilities**: Firefox, WebKit, and Safari specific styles
- **Progressive Enhancement**: Graceful fallbacks for older browsers
- **Reduced Motion Support**: Respects user accessibility preferences
- **High Contrast Mode**: Enhanced visibility options

### 📱 Responsive Design
- **Mobile-First Approach**: Optimized for all screen sizes
- **Flexible Grid System**: 12-column responsive grid
- **Breakpoint System**: Consistent responsive utilities
- **Container Queries**: Component-level responsiveness

## Quick Start

### Installation

1. **Download the Framework**
   \`\`\`bash
   # Clone the repository
   git clone https://github.com/your-username/flexframe-css
   cd flexframe-css
   \`\`\`

2. **Compile SCSS (if customizing)**
   \`\`\`bash
   # Install dependencies
   npm install -g sass
   
   # Compile the framework
   sass framework.scss framework.css --watch
   \`\`\`

3. **Include in Your Project**
   \`\`\`html
   <link rel="stylesheet" href="framework.css">
   \`\`\`

### Basic Usage

\`\`\`html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My App</title>
    <link rel="stylesheet" href="framework.css">
</head>
<body>
    <div class="container">
        <h1 class="text-3xl font-bold text-primary-600">Hello FlexFrame!</h1>
        <p class="text-neutral-600 mb-4">Build beautiful interfaces rapidly.</p>
        <button class="btn btn-primary btn-lg">Get Started</button>
    </div>
</body>
</html>
\`\`\`

## Components

### Buttons
\`\`\`html
<!-- Primary Button -->
<button class="btn btn-primary btn-md">Primary</button>

<!-- Secondary Button -->
<button class="btn btn-secondary btn-md">Secondary</button>

<!-- Outline Button -->
<button class="btn btn-outline btn-md">Outline</button>

<!-- Ghost Button -->
<button class="btn btn-ghost btn-md">Ghost</button>
\`\`\`

### Cards
\`\`\`html
<div class="card">
    <div class="card-header">
        <h3 class="card-title">Card Title</h3>
        <p class="card-subtitle">Card subtitle</p>
    </div>
    <div class="card-body">
        <p class="card-text">Card content goes here.</p>
    </div>
    <div class="card-footer">
        <button class="btn btn-primary btn-sm">Action</button>
    </div>
</div>
\`\`\`

### Forms
\`\`\`html
<div class="form-group">
    <label class="form-label" for="email">Email</label>
    <input type="email" id="email" class="form-input" placeholder="Enter email">
    <div class="form-help">We'll never share your email.</div>
</div>
\`\`\`

## Utility Classes

### Spacing
\`\`\`html
<!-- Margin -->
<div class="m-4">Margin all sides</div>
<div class="mt-2 mb-4">Margin top and bottom</div>

<!-- Padding -->
<div class="p-6">Padding all sides</div>
<div class="px-4 py-2">Padding horizontal and vertical</div>
\`\`\`

### Colors
\`\`\`html
<!-- Background Colors -->
<div class="bg-primary-500">Primary background</div>
<div class="bg-success">Success background</div>

<!-- Text Colors -->
<p class="text-primary-600">Primary text</p>
<p class="text-neutral-500">Neutral text</p>
\`\`\`

### Layout
\`\`\`html
<!-- Flexbox -->
<div class="flex items-center justify-between">
    <span>Left content</span>
    <span>Right content</span>
</div>

<!-- Grid -->
<div class="grid grid-cols-1 md:grid-cols-3 gap-4">
    <div>Item 1</div>
    <div>Item 2</div>
    <div>Item 3</div>
</div>
\`\`\`

## Responsive Design

### Breakpoints
- `sm`: 640px and up
- `md`: 768px and up  
- `lg`: 1024px and up
- `xl`: 1280px and up
- `2xl`: 1536px and up

### Usage
\`\`\`html
<!-- Responsive grid -->
<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-4">
    <!-- Grid items -->
</div>

<!-- Responsive text -->
<h1 class="text-2xl md:text-4xl lg:text-5xl">Responsive heading</h1>

<!-- Responsive visibility -->
<div class="hidden md:block">Visible on medium screens and up</div>
\`\`\`

## Modern CSS Features

### Container Queries
\`\`\`html
<div class="container-query">
    <div class="container-sm:text-lg container-md:text-xl">
        Text size based on container width
    </div>
</div>
\`\`\`

### Browser-Specific Utilities
\`\`\`html
<!-- Firefox specific -->
<div class="firefox:bg-red-100">Red background in Firefox</div>

<!-- WebKit specific -->
<div class="webkit:bg-blue-100">Blue background in Chrome/Safari</div>
\`\`\`

## Customization

### CSS Custom Properties
\`\`\`css
:root {
    /* Override default colors */
    --color-primary-500: #your-brand-color;
    --color-primary-600: #your-brand-color-dark;
    
    /* Override spacing */
    --space-4: 1.5rem; /* Instead of 1rem */
    
    /* Override typography */
    --font-family-sans: 'Your Font', sans-serif;
}
\`\`\`

### SCSS Variables
\`\`\`scss
// Override in your own SCSS file before importing
$colors: (
    'primary': (
        500: #your-color,
        600: #your-darker-color,
    ),
    'brand': #your-brand-color,
);

@import 'flexframe/framework';
\`\`\`

## Browser Support

- **Modern Browsers**: Full support for Chrome, Firefox, Safari, Edge
- **Container Queries**: Chrome 105+, Firefox 110+, Safari 16+
- **CSS Grid**: All modern browsers
- **Custom Properties**: All modern browsers
- **Graceful Degradation**: Fallbacks for older browsers

## Performance

- **Optimized CSS**: Minified production build
- **Tree Shaking**: Use only what you need
- **Modern Features**: Leverages browser optimizations
- **Small Footprint**: Efficient utility-first approach

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test across browsers
5. Submit a pull request

## License

MIT License - feel free to use in personal and commercial projects.

## Changelog

### v1.0.0
- Initial release
- Complete utility system
- Component library
- Modern CSS features
- Browser-specific utilities
- Dark mode support
- Container queries
- Responsive grid system

---

Built with ❤️ for the modern web. Happy coding!
