# Local Business Directory

> Discover the best local businesses in one place

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Version](https://img.shields.io/badge/version-1.0.0-green.svg)

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Getting Started](#getting-started)
- [Directory Structure](#directory-structure)
- [Customization Guide](#customization-guide)
- [Deployment](#deployment)
- [Custom Domain Setup](#custom-domain-setup)
- [Troubleshooting](#troubleshooting)
- [Resources & Support](#resources--support)

## Overview

Local Business Directory is a responsive, modern directory website featuring a clean 3-column grid layout. The platform helps users discover and connect with local businesses through an intuitive categorization system and search functionality.

## Features

- 🎯 Responsive 3-column grid layout
- 🔍 Search functionality
- 🏷️ Category filtering
- 📱 Mobile-friendly design
- 🖼️ Custom hero section
- 🎨 Customizable styling
- 📊 Business analytics integration
- 💨 Fast loading times

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn
- Git

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/local-business-directory

# Navigate to project directory
cd local-business-directory

# Install dependencies
npm install

# Start development server
npm run dev
```

## Directory Structure

```
local-business-directory/
├── src/
│   ├── components/
│   │   ├── Directory/
│   │   ├── Hero/
│   │   └── Search/
│   ├── data/
│   │   └── businesses.json
│   └── styles/
├── public/
│   └── images/
├── config/
└── package.json
```

## Customization Guide

### Adding/Editing Directory Items

1. Navigate to `src/data/businesses.json`
2. Add new business entries using the following format:

```json
{
  "id": "unique-id",
  "name": "Business Name",
  "category": "Category",
  "description": "Business description",
  "address": "Business address",
  "phone": "Phone number",
  "website": "Website URL",
  "image": "image-filename.jpg"
}
```

### Modifying Category Labels

1. Open `src/config/categories.js`
2. Edit the category array:

```javascript
export const categories = [
  {
    id: "category-1",
    label: "Restaurants",
    icon: "restaurant-icon"
  },
  // Add more categories
];
```

### Updating Hero Section

1. Locate `src/components/Hero/Hero.js`
2. Modify the content:

```javascript
<div className="hero">
  <h1>Your Custom Heading</h1>
  <p>Your custom description</p>
  <img src="/path/to/image" alt="Hero image" />
</div>
```

### Customizing Colors and Styling

1. Navigate to `src/styles/variables.scss`
2. Update color variables:

```scss
$primary-color: #your-color;
$secondary-color: #your-color;
$accent-color: #your-color;
```

## Deployment

### Building for Production

```bash
# Create production build
npm run build

# Test production build locally
npm run serve
```

### Deployment Platforms

- Vercel: [![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/yourusername/local-business-directory)
- Netlify: [![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/yourusername/local-business-directory)

## Custom Domain Setup

1. Purchase domain from preferred registrar
2. Add custom domain in deployment platform
3. Configure DNS settings:
   ```
   A Record: @ → deployment-platform-ip
   CNAME: www → yourdomain.com
   ```
4. Wait for DNS propagation (24-48 hours)

## Troubleshooting

### Common Issues

1. **Images not loading**
   - Verify image paths in `businesses.json`
   - Check image formats (supported: jpg, png, webp)
   - Ensure images are in `public/images/`

2. **Styling issues**
   - Clear browser cache
   - Check CSS compilation
   - Verify media queries for responsive design

3. **Search not working**
   - Check browser console for errors
   - Verify search component props
   - Validate data structure in `businesses.json`

## Resources & Support

- [Documentation Wiki](https://github.com/yourusername/local-business-directory/wiki)
- [Issue Tracker](https://github.com/yourusername/local-business-directory/issues)
- [Contributing Guidelines](CONTRIBUTING.md)

### Community & Help

- [Discord Community](https://discord.gg/yourdiscord)
- [Stack Overflow](https://stackoverflow.com/questions/tagged/local-business-directory)
- Email Support: support@yourdomain.com

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Made with ❤️ by [Your Name](https://github.com/yourusername)