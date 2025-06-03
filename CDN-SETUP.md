# FlexFrame CSS Framework - CDN Setup Guide

## 🚀 Quick Start with CDN

### Option 1: jsDelivr (Recommended)
\`\`\`html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/flexframe-css@1.0.0/dist/flexframe.css">
\`\`\`

### Option 2: unpkg
\`\`\`html
<link rel="stylesheet" href="https://unpkg.com/flexframe-css@1.0.0/dist/flexframe.css">
\`\`\`

### Option 3: Skypack
\`\`\`html
<link rel="stylesheet" href="https://cdn.skypack.dev/flexframe-css@1.0.0/dist/flexframe.css">
\`\`\`

## 📦 Publishing to NPM for CDN Access

### Step 1: Prepare Your Package
\`\`\`bash
# Build the CSS
npm run build

# Test locally
npm pack
\`\`\`

### Step 2: Publish to NPM
\`\`\`bash
# Login to NPM
npm login

# Publish package
npm publish
\`\`\`

### Step 3: Verify CDN Access
After publishing, your package will be automatically available on:
- jsDelivr: `https://cdn.jsdelivr.net/npm/flexframe-css@latest/dist/flexframe.css`
- unpkg: `https://unpkg.com/flexframe-css@latest/dist/flexframe.css`

## 🔧 Version Management

### Specific Version
\`\`\`html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/flexframe-css@1.0.0/dist/flexframe.css">
\`\`\`

### Latest Version (Auto-updates)
\`\`\`html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/flexframe-css@latest/dist/flexframe.css">
\`\`\`

### Version Range
\`\`\`html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/flexframe-css@^1.0.0/dist/flexframe.css">
\`\`\`

## 🌐 CDN Features

### jsDelivr Benefits
- ✅ Global CDN with 100+ locations
- ✅ HTTP/2 and Brotli compression
- ✅ Automatic minification
- ✅ SRI (Subresource Integrity) support
- ✅ Load balancing and failover

### Performance Optimization
\`\`\`html
<!-- With SRI for security -->
<link rel="stylesheet" 
      href="https://cdn.jsdelivr.net/npm/flexframe-css@1.0.0/dist/flexframe.css"
      integrity="sha384-..."
      crossorigin="anonymous">

<!-- Preload for better performance -->
<link rel="preload" 
      href="https://cdn.jsdelivr.net/npm/flexframe-css@1.0.0/dist/flexframe.css" 
      as="style" 
      onload="this.onload=null;this.rel='stylesheet'">
\`\`\`

## 📊 CDN Analytics

### jsDelivr Stats
View usage statistics at:
`https://www.jsdelivr.com/package/npm/flexframe-css`

### Features Available
- Download statistics
- Geographic distribution
- Version usage
- File popularity

## 🔄 Development vs Production

### Development (Latest)
\`\`\`html
<!-- Always get the newest version -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/flexframe-css@latest/dist/flexframe.css">
\`\`\`

### Production (Pinned)
\`\`\`html
<!-- Pin to specific version for stability -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/flexframe-css@1.0.0/dist/flexframe.css">
\`\`\`

## 🛠️ Custom Builds via CDN

### Combine with Other Libraries
\`\`\`html
<!-- FlexFrame + Custom CSS -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/flexframe-css@1.0.0/dist/flexframe.css">
<link rel="stylesheet" href="your-custom-styles.css">
\`\`\`

### ESM Import (for JS bundlers)
\`\`\`javascript
import 'https://cdn.skypack.dev/flexframe-css@1.0.0/dist/flexframe.css';
\`\`\`

## 📱 Mobile Optimization

\`\`\`html
<head>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/flexframe-css@1.0.0/dist/flexframe.css">
    
    <!-- Critical CSS inline for above-the-fold content -->
    <style>
        .hero { /* critical styles */ }
    </style>
</head>
\`\`\`

## 🔒 Security Considerations

### Subresource Integrity (SRI)
\`\`\`bash
# Generate SRI hash
openssl dgst -sha384 -binary flexframe.css | openssl base64 -A
\`\`\`

\`\`\`html
<link rel="stylesheet" 
      href="https://cdn.jsdelivr.net/npm/flexframe-css@1.0.0/dist/flexframe.css"
      integrity="sha384-GENERATED_HASH_HERE"
      crossorigin="anonymous">
\`\`\`

## 🚀 Getting Started Template

\`\`\`html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My FlexFrame App</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/flexframe-css@1.0.0/dist/flexframe.css">
</head>
<body class="bg-neutral-50">
    <div class="container py-8">
        <h1 class="text-4xl font-bold text-primary-600 text-center">
            Hello FlexFrame!
        </h1>
        <div class="grid grid-cols-1 md:grid-cols-3 gap-6 mt-8">
            <div class="card">
                <div class="card-body">
                    <h3 class="card-title">Card 1</h3>
                    <p class="text-neutral-600">Your content here</p>
                </div>
            </div>
            <!-- More cards... -->
        </div>
    </div>
</body>
</html>
\`\`\`

## 📈 Migration from Local to CDN

### Before (Local)
\`\`\`html
<link rel="stylesheet" href="./css/flexframe.css">
\`\`\`

### After (CDN)
\`\`\`html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/flexframe-css@1.0.0/dist/flexframe.css">
\`\`\`

That's it! Your framework is now globally available via CDN. 🎉
