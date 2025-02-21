# AI Business Rankers Landing Page - Maintenance Guide

This guide will help you maintain and customize the AI Business Rankers landing page. Whether you're new to web development or need a quick reference, follow these detailed instructions for common updates.

## Table of Contents
1. [Updating Text and Styling](#updating-text-and-styling)
2. [Managing Links](#managing-links)
3. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains your company name and navigation menu. To update:

```html
<!-- Located at the top of the page -->
<div class="text-xl font-bold text-blue-500">AI Business Rankers</div>
```

To change the company name:
1. Locate this div in the header section
2. Replace "AI Business Rankers" with your desired text
3. Adjust text size using Tailwind classes:
   - `text-xl` (current) - medium large
   - `text-2xl` - larger
   - `text-lg` - slightly smaller

### Hero Section
The main headline and subtitle are in the hero section:

```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-extrabold text-transparent bg-clip-text bg-gradient-to-r from-blue-400 to-blue-600 mb-8">
    A.I. Agents That Make Ben Franklin's Do Back Flips!
</h1>
```

To modify:
1. Replace the text between the `<h1>` tags
2. Keep the classes intact to maintain the gradient effect
3. The responsive sizes are:
   - `text-4xl` - mobile devices
   - `text-5xl` - medium screens
   - `text-6xl` - large screens

### Features Section
Each feature card follows this structure:

```html
<div class="bg-gray-900 p-8 rounded-2xl hover:transform hover:scale-105 transition-all duration-300">
    <h3 class="text-xl font-semibold mb-4">24/7 Operation</h3>
    <p class="text-gray-400">AI Agents that work around the clock...</p>
</div>
```

To add or modify features:
1. Copy the entire `<div>` block
2. Update the heading text in `<h3>`
3. Update the description in `<p>`
4. Maintain the classes for consistent styling

## Managing Links

### Navigation Menu Links
The navigation menu contains internal page links:

```html
<div class="hidden md:flex space-x-8">
    <a href="#features" class="hover:text-blue-400 transition-colors duration-300">Features</a>
    <a href="#benefits" class="hover:text-blue-400 transition-colors duration-300">Benefits</a>
    <a href="#faq" class="hover:text-blue-400 transition-colors duration-300">FAQ</a>
    <a href="#contact" class="hover:text-blue-400 transition-colors duration-300">Contact</a>
</div>
```

To update links:
1. Find the `<a>` tag you want to modify
2. Update the `href` attribute:
   - For internal sections, use `#section-name`
   - For external links, use the full URL: `https://example.com`

### Call-to-Action Buttons
Update the main CTA buttons:

```html
<a href="https://aibusinessrankers.com" class="inline-block px-8 py-4 bg-blue-600 hover:bg-blue-700 rounded-full">
    Transform Your Business Today
</a>
```

Replace:
1. The `href` attribute with your desired URL
2. The button text between the `<a>` tags
3. Maintain the classes for consistent styling

## Adding Privacy and Terms Pages

### Footer Legal Links
Locate the legal section in the footer:

```html
<div>
    <h3 class="text-lg font-semibold mb-4">Legal</h3>
    <ul class="space-y-2">
        <li><a href="#" class="text-gray-400 hover:text-blue-400">Privacy Policy</a></li>
        <li><a href="#" class="text-gray-400 hover:text-blue-400">Terms of Service</a></li>
    </ul>
</div>
```

To link privacy and terms pages:
1. Create your privacy.html and terms.html files
2. Update the href attributes:
```html
<li><a href="privacy.html" class="text-gray-400 hover:text-blue-400">Privacy Policy</a></li>
<li><a href="terms.html" class="text-gray-400 hover:text-blue-400">Terms of Service</a></li>
```

## Troubleshooting

### Common Issues and Solutions

1. **Broken Internal Links**
   - Ensure section IDs match the href attributes
   - Section IDs should not contain spaces
   - Example: `href="#features"` links to `id="features"`

2. **Responsive Design Issues**
   - Keep the responsive classes intact:
   - `md:` prefix for medium screens
   - `lg:` prefix for large screens
   - Example: `class="text-4xl md:text-5xl lg:text-6xl"`

3. **Style Inconsistencies**
   - Copy existing classes when creating new elements
   - Maintain color scheme using Tailwind colors:
     - Primary: `blue-500`
     - Background: `gray-900`
     - Text: `gray-100`, `gray-400`

### Need Help?
If you encounter issues:
1. Check class names for typos
2. Verify all tags are properly closed
3. Test links in multiple browsers
4. Ensure all files are in the correct directory

Remember to backup your files before making significant changes!