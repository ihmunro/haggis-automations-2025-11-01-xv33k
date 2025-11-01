# Haggis Automations Landing Page - Maintenance & Customization Guide

A comprehensive guide for maintaining, updating, and customizing your Haggis Automations landing page. Whether you're new to web development or looking to make quick updates, this guide will walk you through every process step-by-step.

---

## Table of Contents

1. [Getting Started](#getting-started)
2. [Understanding the Page Structure](#understanding-the-page-structure)
3. [Updating Text Content](#updating-text-content)
4. [Modifying Tailwind CSS Classes](#modifying-tailwind-css-classes)
5. [Fixing and Updating Links](#fixing-and-updating-links)
6. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
7. [Common Customizations](#common-customizations)
8. [Troubleshooting](#troubleshooting)
9. [Best Practices](#best-practices)

---

## Getting Started

### What You'll Need

- A text editor (we recommend **Visual Studio Code** - it's free and beginner-friendly)
- Basic understanding of HTML tags (like `<a>`, `<button>`, `<h1>`)
- Your landing page files: `index.html`, `privacy.html`, and `terms.html`

### Opening Your Files

1. Open your text editor
2. Click **File** → **Open Folder**
3. Select the folder containing your landing page files
4. You should see your files listed on the left side

### File Structure You Should Have

```
your-project-folder/
├── index.html          (your main landing page)
├── privacy.html        (privacy policy page)
├── terms.html          (terms of service page)
└── (any other files)
```

---

## Understanding the Page Structure

Your landing page is organized into distinct sections. Here's what each section does:

### Main Sections of Your Page

| Section | Location in Code | Purpose |
|---------|-----------------|---------|
| **Header & Navigation** | Lines 39-77 | Sticky navigation bar at the top with menu links |
| **Hero Section** | Lines 79-141 | Large welcome banner with headline and call-to-action buttons |
| **Features Section** | Lines 143-269 | 6 feature cards showcasing what Haggis Automations offers |
| **Benefits Section** | Lines 271-437 | 3 detailed benefit sections with icons and descriptions |
| **Testimonials Section** | Lines 439-527 | Customer reviews and ratings |
| **CTA Section** | Lines 529-563 | Call-to-action banner with background image |
| **FAQ Section** | Lines 565-717 | Frequently asked questions with expandable answers |
| **About Section** | Lines 719-756 | Information about Haggis Automations |
| **Footer** | Lines 758-859 | Contact info, social links, and legal links |

---

## Updating Text Content

### What is Text Content?

Text content is any visible text on your page that users read. This includes headlines, descriptions, button labels, and testimonials.

### How to Find and Update Text

#### Example 1: Changing the Hero Section Headline

**Current text (around line 96):**
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900 leading-tight tracking-tight mb-4">
    Haggis Automations
</h1>
```

**To change it:**

1. Find the line with `<h1>` that contains "Haggis Automations"
2. Replace `Haggis Automations` with your desired text
3. Keep all the code around it exactly the same

**Example change:**
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900 leading-tight tracking-tight mb-4">
    My Amazing Website Builder
</h1>
```

#### Example 2: Changing the Subtitle

**Current text (around line 100):**
```html
<p class="text-xl md:text-2xl text-purple-600 font-semibold leading-relaxed">
    Free Websites with Website Hosting
</p>
```

**To change it:**
```html
<p class="text-xl md:text-2xl text-purple-600 font-semibold leading-relaxed">
    Build Your Online Presence for Free
</p>
```

#### Example 3: Changing Button Text

**Current text (around line 115):**
```html
<button class="bg-gradient-to-r from-purple-600 to-purple-700 text-white px-8 py-4 rounded-lg font-bold text-lg hover:shadow-lg transition-all duration-300 hover:scale-105 focus:outline-none focus:ring-4 focus:ring-purple-300">
    Get Started Free
</button>
```

**To change it:**
```html
<button class="bg-gradient-to-r from-purple-600 to-purple-700 text-white px-8 py-4 rounded-lg font-bold text-lg hover:shadow-lg transition-all duration-300 hover:scale-105 focus:outline-none focus:ring-4 focus:ring-purple-300">
    Create Your Website Now
</button>
```

### Updating Feature Cards

Your features section has 6 cards. Each card follows this pattern:

**Location: Lines 183-269**

**Example: Changing the First Feature Card Title**

**Current text (around line 194):**
```html
<h3 class="text-xl font-bold text-gray-900 mb-3">Beautiful Templates</h3>
```

**To change it:**
```html
<h3 class="text-xl font-bold text-gray-900 mb-3">Stunning Design Templates</h3>
```

**Example: Changing Feature Description**

**Current text (around line 195):**
```html
<p class="text-gray-700 leading-relaxed mb-4">
    Choose from our carefully curated collection of professionally designed templates...
</p>
```

**To change it:**
```html
<p class="text-gray-700 leading-relaxed mb-4">
    Your custom text here. Keep it clear and benefit-focused...
</p>
```

### Updating Testimonials

**Location: Lines 475-527**

Each testimonial card has:
- A 5-star rating
- Customer quote
- Customer name
- Customer title

**Example: Changing a Testimonial**

**Current text (around line 483):**
```html
<p class="text-gray-700 leading-relaxed mb-6">
    "I was amazed at how easy it was to create my business website..."
</p>
```

**To change it:**
```html
<p class="text-gray-700 leading-relaxed mb-6">
    "Your new testimonial text here. Keep quotes in quotation marks..."
</p>
```

**Update the name (around line 487):**
```html
<h4 class="font-bold text-gray-900">Sarah Mitchell</h4>
```

**To change it:**
```html
<h4 class="font-bold text-gray-900">John Anderson</h4>
```

**Update the title (around line 488):**
```html
<p class="text-sm text-gray-600">Small Business Owner</p>
```

**To change it:**
```html
<p class="text-sm text-gray-600">E-commerce Entrepreneur</p>
```

### Updating FAQ Questions and Answers

**Location: Lines 579-717**

Each FAQ item has a question and an answer.

**Example: Changing an FAQ Question**

**Current text (around line 588):**
```html
<h3 class="text-lg font-bold text-gray-900">Is Haggis Automations really completely free?</h3>
```

**To change it:**
```html
<h3 class="text-lg font-bold text-gray-900">What makes your platform different?</h3>
```

**Example: Changing an FAQ Answer**

**Current text (around line 594):**
```html
<p class="text-gray-700 leading-relaxed">
    Yes, absolutely! Haggis Automations is 100% free and always will be...
</p>
```

**To change it:**
```html
<p class="text-gray-700 leading-relaxed">
    Your answer text here. Be clear and concise...
</p>
```

### Updating Footer Contact Information

**Location: Lines 808-830**

**Current email (around line 815):**
```html
<a href="mailto:iainhmunro@gmail.com" class="text-white hover:text-purple-400 transition-colors duration-300">iainhmunro@gmail.com</a>
```

**To change it:**
```html
<a href="mailto:your-email@example.com" class="text-white hover:text-purple-400 transition-colors duration-300">your-email@example.com</a>
```

---

## Modifying Tailwind CSS Classes

### What is Tailwind CSS?

Tailwind CSS is a system for styling your website using special class names. Instead of writing custom CSS, you add classes to HTML elements to control how they look.

### Understanding Tailwind Classes on This Page

#### Common Classes You'll See

| Class | What It Does | Example |
|-------|-------------|---------|
| `text-4xl` | Makes text very large | Used for main headlines |
| `text-gray-900` | Makes text dark gray/black | Standard text color |
| `text-purple-600` | Makes text purple | Used for accent colors |
| `bg-white` | White background | Card backgrounds |
| `bg-gray-50` | Light gray background | Section backgrounds |
| `px-8` | Adds left and right padding | Spacing inside elements |
| `py-4` | Adds top and bottom padding | Vertical spacing |
| `rounded-lg` | Rounds corners slightly | Card styling |
| `rounded-xl` | Rounds corners more | Larger rounded corners |
| `shadow-md` | Adds a subtle shadow | Depth effect |
| `hover:text-purple-600` | Changes color on hover | Interactive effect |
| `transition-all` | Smooth animation | When things change |
| `md:` prefix | Only applies on medium screens | Responsive design |
| `lg:` prefix | Only applies on large screens | Responsive design |

### How Responsive Design Works

Your page automatically adjusts for different screen sizes using prefixes:

- **No prefix** = Mobile phones (small screens)
- **`md:`** = Tablets (medium screens, 768px+)
- **`lg:`** = Desktops (large screens, 1024px+)

**Example from your code (line 96):**
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900 leading-tight tracking-tight mb-4">
```

This means:
- On phones: text size is `4xl`
- On tablets: text size is `5xl`
- On desktops: text size is `6xl`

### Changing Text Sizes

**Location: Throughout the page**

**Current code (line 96):**
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900">
```

**To make it smaller:**
```html
<h1 class="text-3xl md:text-4xl lg:text-5xl font-bold text-gray-900">
```

**To make it larger:**
```html
<h1 class="text-5xl md:text-6xl lg:text-7xl font-bold text-gray-900">
```

### Changing Colors

**Current code (line 100):**
```html
<p class="text-xl md:text-2xl text-purple-600 font-semibold leading-relaxed">
```

**To change text color to blue:**
```html
<p class="text-xl md:text-2xl text-blue-600 font-semibold leading-relaxed">
```

**Available colors:**
- `text-purple-600`, `text-blue-600`, `text-red-600`, `text-green-600`, `text-gray-600`, `text-indigo-600`, `text-pink-600`

### Changing Background Colors

**Current code (line 151):**
```html
<section id="features" class="py-24 md:py-32 bg-gray-50">
```

**To change background to white:**
```html
<section id="features" class="py-24 md:py-32 bg-white">
```

**To change background to light blue:**
```html
<section id="features" class="py-24 md:py-32 bg-blue-50">
```

### Changing Button Styles

**Location: Lines 115-122 (Hero buttons)**

**Current primary button:**
```html
<button class="bg-gradient-to-r from-purple-600 to-purple-700 text-white px-8 py-4 rounded-lg font-bold text-lg hover:shadow-lg transition-all duration-300 hover:scale-105 focus:outline-none focus:ring-4 focus:ring-purple-300">
    Get Started Free
</button>
```

**To change to solid blue:**
```html
<button class="bg-blue-600 text-white px-8 py-4 rounded-lg font-bold text-lg hover:shadow-lg transition-all duration-300 hover:scale-105 focus:outline-none focus:ring-4 focus:ring-blue-300">
    Get Started Free
</button>
```

**To make button larger:**
```html
<button class="bg-gradient-to-r from-purple-600 to-purple-700 text-white px-10 py-5 rounded-lg font-bold text-lg hover:shadow-lg transition-all duration-300 hover:scale-105 focus:outline-none focus:ring-4 focus:ring-purple-300">
```

### Changing Padding and Spacing

**Padding (internal spacing):**
- `p-4` = small padding all around
- `p-8` = medium padding all around
- `p-12` = large padding all around
- `px-8` = left and right padding only
- `py-4` = top and bottom padding only

**Margin (external spacing):**
- `mb-4` = margin below element
- `mt-4` = margin above element
- `mx-auto` = centers element horizontally

**Example: Changing card padding (line 187):**

**Current:**
```html
<div class="card-hover bg-white rounded-xl shadow-md p-8 border border-gray-100">
```

**To increase padding:**
```html
<div class="card-hover bg-white rounded-xl shadow-md p-12 border border-gray-100">
```

### Changing Border Radius (Rounded Corners)

| Class | Effect |
|-------|--------|
| `rounded-lg` | Slightly rounded corners |
| `rounded-xl` | More rounded corners |
| `rounded-2xl` | Very rounded corners |
| `rounded-full` | Completely circular |

**Example: Making corners rounder (line 187):**

**Current:**
```html
<div class="card-hover bg-white rounded-xl shadow-md p-8 border border-gray-100">
```

**To make rounder:**
```html
<div class="card-hover bg-white rounded-2xl shadow-md p-8 border border-gray-100">
```

### Changing Shadows

| Class | Effect |
|-------|--------|
| `shadow-md` | Medium shadow |
| `shadow-lg` | Large shadow |
| `shadow-xl` | Extra large shadow |
| `shadow-2xl` | Very large shadow |

**Example: Increasing shadow (line 187):**

**Current:**
```html
<div class="card-hover bg-white rounded-xl shadow-md p-8 border border-gray-100">
```

**To increase shadow:**
```html
<div class="card-hover bg-white rounded-xl shadow-lg p-8 border border-gray-100">
```

### Changing Grid Layouts

Your page uses responsive grids that automatically adjust column count.

**Example: Feature cards section (line 162):**
```html
<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
```

This means:
- **Mobile:** 1 column
- **Tablet:** 2 columns
- **Desktop:** 3 columns
- **Gap:** 8 units of space between items

**To change to 2 columns on desktop:**
```html
<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-2 gap-8">
```

**To increase gap between cards:**
```html
<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-12">
```

---

## Fixing and Updating Links

### What is a Link?

A link is code that takes users to a different page or section. Links use the `<a>` tag with an `href` attribute.

### Types of Links on Your Page

#### 1. Internal Navigation Links (Jump to sections on same page)

These links start with `#` and jump to different sections of your landing page.

**Location: Header navigation (lines 50-54)**

```html
<a href="#features" class="text-gray-700 hover:text-purple-600 transition-colors duration-300 font-medium">Features</a>
<a href="#benefits" class="text-gray-700 hover:text-purple-600 transition-colors duration-300 font-medium">Benefits</a>
<a href="#testimonials" class="text-gray-700 hover:text-purple-600 transition-colors duration-300 font-medium">Testimonials</a>
<a href="#faq" class="text-gray-700 hover:text-purple-600 transition-colors duration-300 font-medium">FAQ</a>
<a href="#about" class="text-gray-700 hover:text-purple-600 transition-colors duration-300 font-medium">About</a>
```

**These links work because sections have matching IDs:**
- `href="#features"` → jumps to `<section id="features">`
- `href="#benefits"` → jumps to `<section id="benefits">`
- And so on...

**✓ These links are working correctly and don't need changes.**

#### 2. External Links (Go to other websites)

These links have full URLs starting with `http://` or `https://`

**Location: Social media links in footer (lines 788-803)**

```html
<a href="#" class="text-gray-400 hover:text-purple-400 transition-colors duration-300" aria-label="Facebook">
    <i class="fab fa-facebook-f text-xl"></i>
</a>
```

**⚠️ These links currently go nowhere!** They use `href="#"` which is a placeholder.

**To fix Facebook link:**
```html
<a href="https://www.facebook.com/your-page-name" class="text-gray-400 hover:text-purple-400 transition-colors duration-300" aria-label="Facebook">
    <i class="fab fa-facebook-f text-xl"></i>
</a>
```

**To fix Twitter link:**
```html
<a href="https://www.twitter.com/your-username" class="text-gray-400 hover:text-purple-400 transition-colors duration-300" aria-label="Twitter">
    <i class="fab fa-twitter text-xl"></i>
</a>
```

**To fix LinkedIn link:**
```html
<a href="https://www.linkedin.com/company/your-company" class="text-gray-400 hover:text-purple-400 transition-colors duration-300" aria-label="LinkedIn">
    <i class="fab fa-linkedin-in text-xl"></i>
</a>
```

**To fix Instagram link:**
```html
<a href="https://www.instagram.com/your-username" class="text-gray-400 hover:text-purple-400 transition-colors duration-300" aria-label="Instagram">
    <i class="fab fa-instagram text-xl"></i>
</a>
```

#### 3. Footer Links to Other Pages

**Location: Footer (lines 768-787)**

**Current links:**
```html
<li><a href="blog.html" class="text-gray-400 hover:text-purple-400 transition-colors duration-300">Blog</a></li>
<li><a href="privacy.html" class="text-gray-400 hover:text-purple-400 transition-colors duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="text-gray-400 hover:text-purple-400 transition-colors duration-300">Terms of Service</a></li>
```

**These links need files to exist:**
- `blog.html` - Your blog page
- `privacy.html` - Your privacy policy page
- `terms.html` - Your terms of service page

### Step-by-Step: Fixing All Links

#### Step 1: Update Social Media Links

Find lines 788-803 in your code and replace each `href="#"` with your actual social media URLs.

**Find this:**
```html
<a href="#" class="text-gray-400 hover:text-purple-400 transition-colors duration-300" aria-label="Facebook">
```

**Replace with:**
```html
<a href="https://www.facebook.com/your-business" class="text-gray-400 hover:text-purple-400 transition-colors duration-300" aria-label="Facebook">
```

**Repeat for all 4 social media links.**

#### Step 2: Create Missing Pages

If you don't have `blog.html`, `privacy.html`, and `terms.html` files, you need to create them.

**To create privacy.html:**

1. In your text editor, click **File** → **New File**
2. Click **File** → **Save As**
3. Name it `privacy.html`
4. Save it in the same folder as your `index.html`
5. Add basic content:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Privacy Policy - Haggis Automations</title>
    <script src="https://cdn.tailwindcss.com"></script>
</head>
<body class="bg-white text-gray-900">
    <div class="max-w-4xl mx-auto px-4 py-16">
        <h1 class="text-4xl font-bold mb-8">Privacy Policy</h1>
        <p class="text-gray-700 leading-relaxed mb-4">
            Your privacy policy content goes here.
        </p>
        <a href="index.html" class="text-purple-600 hover:text-purple-700">← Back to Home</a>
    </div>
</body>
</html>
```

**Repeat for terms.html and blog.html**

#### Step 3: Update Footer Links

If you created the pages, the links in the footer should now work:

**Lines 768-787:**
```html
<li><a href="blog.html" class="text-gray-400 hover:text-purple-400 transition-colors duration-300">Blog</a></li>
<li><a href="privacy.html" class="text-gray-400 hover:text-purple-400 transition-colors duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="text-gray-400 hover:text-purple-400 transition-colors duration-300">Terms of Service</a></li>
```

These links will now work because the files exist!

#### Step 4: Update Footer Contact Links

**Line 815:**

**Current:**
```html
<a href="mailto:iainhmunro@gmail.com" class="text-white hover:text-purple-400 transition-colors duration-300">iainhmunro@gmail.com</a>
```

**To change email:**
```html
<a href="mailto:your-email@example.com" class="text-white hover:text-purple-400 transition-colors duration-300">your-email@example.com</a>
```

### Summary of All Links That Need Updating

| Link Location | Current Value | What To Change It To |
|---------------|---------------|----------------------|
| Facebook (line 789) | `href="#"` | Your Facebook page URL |
| Twitter (line 793) | `href="#"` | Your Twitter profile URL |
| LinkedIn (line 797) | `href="#"` | Your LinkedIn company page URL |
| Instagram (line 801) | `href="#"` | Your Instagram profile URL |
| Email (line 815) | `iainhmunro@gmail.com` | Your email address |
| Blog (line 774) | `blog.html` | Your blog page (must exist) |
| Privacy Policy (line 777) | `privacy.html` | Your privacy page (must exist) |
| Terms (line 778) | `terms.html` | Your terms page (must exist) |

---

## Adding Privacy and Terms Pages

### Why You Need These Pages

Privacy and Terms pages are legal requirements for most websites. They explain:
- **Privacy Policy:** How you collect and use user data
- **Terms of Service:** Rules for using your website

### Method 1: Quick Start (Basic Pages)

#### Creating privacy.html

1. Open your text editor
2. Click **File** → **New File**
3. Copy this complete code:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Privacy Policy - Haggis Automations">
    <title>Privacy Policy - Haggis Automations</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        html {
            scroll-behavior: smooth;
        }
        .gradient-text {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
    </style>
</head>
<body class="bg-white text-gray-900">
    <!-- Header Navigation -->
    <header class="sticky top-0 z-50 bg-white shadow-md">
        <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">
                <div class="flex-shrink-0">
                    <a href="index.html" class="text-2xl font-bold gradient-text">
                        <i class="fas fa-cog mr-2"></i>Haggis Automations
                    </a>
                </div>
                <div class="hidden md:flex space-x-8">
                    <a href="index.html#features" class="text-gray-700 hover:text-purple-600 transition-colors duration-300 font-medium">Features</a>
                    <a href="index.html#benefits" class="text-gray-700 hover:text-purple-600 transition-colors duration-300 font-medium">Benefits</a>
                    <a href="index.html#about" class="text-gray-700 hover:text-purple-600 transition-colors duration-300 font-medium">About</a>
                    <a href="index.html" class="text-gray-700 hover:text-purple-600 transition-colors duration-300 font-medium">Home</a>
                </div>
            </div>
        </nav>
    </header>

    <!-- Main Content -->
    <main class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 py-16">
        <h1 class="text-4xl md:text-5xl font-bold text-gray-900 mb-8">Privacy Policy</h1>
        
        <div class="prose prose-lg max-w-none space-y-8 text-gray-700">
            <section>
                <h2 class="text-2xl font-bold text-gray-900 mb-4">1. Introduction</h2>
                <p class="leading-relaxed">
                    Haggis Automations ("we," "us," "our," or "Company") is committed to protecting your privacy. This Privacy Policy explains how we collect, use, disclose, and safeguard your information when you visit our website and use our services.
                </p>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mb-4">2. Information We Collect</h2>
                <p class="leading-relaxed mb-4">We may collect information about you in a variety of ways. The information we may collect on the Site includes:</p>
                <ul class="list-disc list-inside space-y-2">
                    <li><strong>Personal Data:</strong> Name, email address, phone number, and other information you voluntarily provide</li>
                    <li><strong>Device Information:</strong> Browser type, IP address, and device identifiers</li>
                    <li><strong>Usage Information:</strong> Pages visited, time spent on pages, and links clicked</li>
                    <li><strong>Payment Information:</strong> Payment method details (processed securely by third parties)</li>
                </ul>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mb-4">3. Use of Your Information</h2>
                <p class="leading-relaxed mb-4">Having accurate information about you permits us to provide you with a smooth, efficient, and customized experience. Specifically, we may use information collected about you via the Site to:</p>
                <ul class="list-disc list-inside space-y-2">
                    <li>Create and manage your account</li>
                    <li>Process your transactions and send related information</li>
                    <li>Email you regarding your account or order</li>
                    <li>Fulfill and manage purchases, orders, payments, and other transactions related to our Services</li>
                    <li>Generate a personal profile about you</li>
                    <li>Increase the efficiency and operation of our Site</li>
                    <li>Monitor and analyze usage and trends to improve your experience with the Site</li>
                    <li>Notify you of updates to our Site or Services</li>
                    <li>Offer new products, services, and/or recommendations to you</li>
                </ul>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mb-4">4. Disclosure of Your Information</h2>
                <p class="leading-relaxed mb-4">We may share information we have collected about you in certain situations:</p>
                <ul class="list-disc list-inside space-y-2">
                    <li><strong>By Law or to Protect Rights:</strong> If required by law or to protect our legal rights</li>
                    <li><strong>Third-Party Service Providers:</strong> We may share your information with vendors, consultants, and service providers who assist us</li>
                    <li><strong>Business Transfers:</strong> Your information may be transferred as part of a merger, sale, or acquisition</li>
                </ul>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mb-4">5. Security of Your Information</h2>
                <p class="leading-relaxed">
                    We use administrative, technical, and physical security measures to protect your personal information. However, no method of transmission over the Internet or method of electronic storage is 100% secure. While we strive to use commercially acceptable means to protect your personal information, we cannot guarantee its absolute security.
                </p>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mb-4">6. Contact Us</h2>
                <p class="leading-relaxed">
                    If you have questions or comments about this Privacy Policy, please contact us at:
                </p>
                <p class="mt-4">
                    <strong>Email:</strong> <a href="mailto:iainhmunro@gmail.com" class="text-purple-600 hover:text-purple-700">iainhmunro@gmail.com</a><br>
                    <strong>Website:</strong> <a href="index.html" class="text-purple-600 hover:text-purple-700">Haggis Automations</a>
                </p>
            </section>

            <section class="border-t border-gray-200 pt-8 mt-8">
                <p class="text-sm text-gray-600">
                    <strong>Last Updated:</strong> 2025<br>
                    This Privacy Policy is subject to change at any time. We encourage you to review this policy regularly for any updates.
                </p>
            </section>
        </div>

        <!-- Back to Home -->
        <div class="mt-12 pt-8 border-t border-gray-200">
            <a href="index.html" class="inline-flex items-center text-purple-600 hover:text-purple-700 font-semibold transition-colors">
                <i class="fas fa-arrow-left mr-2"></i>Back to Home
            </a>
        </div>
    </main>

    <!-- Footer -->
    <footer class="bg-gray-900 text-gray-300 py-8 mt-16">
        <div class="max-w-7xl mx-auto px-4 text-center">
            <p class="text-sm">
                &copy; 2025 Haggis Automations. All rights reserved.
            </p>
        </div>
    </footer>
</body>
</html>
```

4. Click **File** → **Save As**
5. Name it `privacy.html`
6. Save in the same folder as `index.html`

#### Creating terms.html

1. Click **File** → **New File**
2. Copy this complete code:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Terms of Service - Haggis Automations">
    <title>Terms of Service - Haggis Automations</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        html {
            scroll-behavior: smooth;
        }
        .gradient-text {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
    </style>
</head>
<body class="bg-white text-gray-900">
    <!-- Header Navigation -->
    <header class="sticky top-0 z-50 bg-white shadow-md">
        <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">
                <div class="flex-shrink-0">
                    <a href="index.html" class="text-2xl font-bold gradient-text">
                        <i class="fas fa-cog mr-2"></i>Haggis Automations
                    </a>
                </div>
                <div class="hidden md:flex space-x-8">
                    <a href="index.html#features" class="text-gray-700 hover:text-purple-600 transition-colors duration-300 font-medium">Features</a>
                    <a href="index.html#benefits" class="text-gray-700 hover:text-purple-600 transition-colors duration-300 font-medium">Benefits</a>
                    <a href="index.html#about" class="text-gray-700 hover:text-purple-600 transition-colors duration-300 font-medium">About</a>
                    <a href="index.html" class="text-gray-700 hover:text-purple-600 transition-colors duration-300 font-medium">Home</a>
                </div>
            </div>
        </nav>
    </header>

    <!-- Main Content -->
    <main class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 py-16">
        <h1 class="text-4xl md:text-5xl font-bold text-gray-900 mb-8">Terms of Service</h1>
        
        <div class="prose prose-lg max-w-none space-y-8 text-gray-700">
            <section>
                <h2 class="text-2xl font-bold text-gray-900 mb-4">1. Agreement to Terms</h2>
                <p class="leading-relaxed">
                    By accessing and using the Haggis Automations website and services, you accept and agree to be bound by the terms and provision of this agreement. If you do not agree to abide by the above, please do not use this service.
                </p>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mb-4">2. Use License</h2>
                <p class="leading-relaxed mb-4">Permission is granted to temporarily download one copy of the materials (information or software) on Haggis Automations' website for personal, non-commercial transitory viewing only. This is the grant of a license, not a transfer of title, and under this license you may not:</p>
                <ul class="list-disc list-inside space-y-2">
                    <li>Modifying or copying the materials</li>
                    <li>Using the materials for any commercial purpose or for any public display</li>
                    <li>Attempting to decompile or reverse engineer any software contained on the website</li>
                    <li>Removing any copyright or other proprietary notations from the materials</li>
                    <li>Transferring the materials to another person or "mirroring" the materials on any other server</li>
                </ul>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mb-4">3. Disclaimer</h2>
                <p class="leading-relaxed">
                    The materials on Haggis Automations' website are provided "as is." Haggis Automations makes no warranties, expressed or implied, and hereby disclaims and negates all other warranties including, without limitation, implied warranties or conditions of merchantability, fitness for a particular purpose, or non-infringement of intellectual property or other violation of rights.
                </p>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mb-4">4. Limitations</h2>
                <p class="leading-relaxed">
                    In no event shall Haggis Automations or its suppliers be liable for any damages (including, without limitation, damages for loss of data or profit, or due to business interruption) arising out of the use or inability to use the materials on Haggis Automations' website, even if we or an authorized representative has been notified orally or in writing of the possibility of such damage.
                </p>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mb-4">5. Accuracy of Materials</h2>
                <p class="leading-relaxed">
                    The materials appearing on Haggis Automations' website could include technical, typographical, or photographic errors. Haggis Automations does not warrant that any of the materials on the website are accurate, complete, or current. Haggis Automations may make changes to the materials contained on the website at any time without notice.
                </p>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mb-4">6. Links</h2>
                <p class="leading-relaxed">
                    Haggis Automations has not reviewed all of the sites linked to its website and is not responsible for the contents of any such linked site. The inclusion of any link does not imply endorsement by Haggis Automations of the site. Use of any such linked website is at the user's own risk.
                </p>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mb-4">7. Modifications</h2>
                <p class="leading-relaxed">
                    Haggis Automations may revise these terms of service for the website at any time without notice. By using this website, you are agreeing to be bound by the then current version of these terms of service.
                </p>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mb-4">8. Governing Law</h2>
                <p class="leading-relaxed">
                    These terms and conditions are governed by and construed in accordance with the laws of the jurisdiction in which Haggis Automations operates, and you irrevocably submit to the exclusive jurisdiction of the courts in that location.
                </p>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mb-4">9. Contact Information</h2>
                <p class="leading-relaxed">
                    If you have any questions about these Terms of Service, please contact us at:
                </p>
                <p class="mt-4">
                    <strong>Email:</strong> <a href="mailto:iainhmunro@gmail.com" class="text-purple-600 hover:text-purple-700">iainhmunro@gmail.com</a><br>
                    <strong>Website:</strong> <a href="index.html" class="text-purple-600 hover:text-purple-700">Haggis Automations</a>
                </p>
            </section>

            <section class="border-t border-gray-200 pt-8 mt-8">
                <p class="text-sm text-gray-600">
                    <strong>Last Updated:</strong> 2025<br>
                    These Terms of Service are subject to change at any time. We encourage you to review them regularly for any updates.
                </p>
            </section>
        </div>

        <!-- Back to Home -->
        <div class="mt-12 pt-8 border-t border-gray-200">
            <a href="index.html" class="inline-flex items-center text-purple-600 hover:text-purple-700 font-semibold transition-colors">
                <i class="fas fa-arrow-left mr-2"></i>Back to Home
            </a>
        </div>
    </main>

    <!-- Footer -->
    <footer class="bg-gray-900 text-gray-300 py-8 mt-16">
        <div class="max-w-7xl mx-auto px-4 text-center">
            <p class="text-sm">
                &copy; 2025 Haggis Automations. All rights reserved.
            </p>
        </div>
    </footer>
</body>
</html>
```

3. Click **File** → **Save As**
4. Name it `terms.html`
5. Save in the same folder as `index.html`

### Method 2: Customizing Your Pages

#### Updating Email Addresses

In both `privacy.html` and `terms.html`, find this line:

```html
<a href="mailto:iainhmunro@gmail.com" class="text-purple-600 hover:text-purple-700">iainhmunro@gmail.com</a>
```

Replace with your email:

```html
<a href="mailto:your-email@example.com" class="text-purple-600 hover:text-purple-700">your-email@example.com</a>
```

#### Updating the Last Updated Date

Find this line in both files:

```html
<strong>Last Updated:</strong> 2025<br>
```

Change to:

```html
<strong>Last Updated:</strong> January 15, 2025<br>
```

#### Adding Company Information

Find this section in both files:

```html
<p class="mt-4">
    <strong>Email:</strong> <a href="mailto:iainhmunro@gmail.com" class="text-purple-600 hover:text-purple-700">iainhmunro@gmail.com</a><br>
    <strong>Website:</strong> <a href="index.html" class="text-purple-600 hover:text-purple-700">Haggis Automations</a>
</p>
```

You can add more information:

```html
<p class="mt-4">
    <strong>Email:</strong> <a href="mailto:your-email@example.com" class="text-purple-600 hover:text-purple-700">your-email@example.com</a><br>
    <strong>Website:</strong> <a href="index.html" class="text-purple-600 hover:text-purple-700">Haggis Automations</a><br>
    <strong>Address:</strong> Your Company Address<br>
    <strong>Phone:</strong> Your Phone Number
</p>
```

### Verifying Links Work

After creating the pages:

1. Open `index.html` in your browser
2. Scroll to the footer
3. Click on "Privacy Policy" - should open `privacy.html`
4. Click on "Terms of Service" - should open `terms.html`
5. Both pages should have a "Back to Home" link that returns you to `index.html`

---

## Common Customizations

### Changing the Brand Color (Purple to Another Color)

Your current design uses purple as the accent color. To change it:

#### Step 1: Identify All Purple Classes

Purple classes in your code:
- `text-purple-600` (purple text)
- `bg-purple-600` (purple background)
- `from-purple-600` (gradient start)
- `to-purple-700` (gradient end)
- `hover:text-purple-600` (hover effect)
- `focus:ring-purple-300` (focus effect)

#### Step 2: Replace with New Color

**To change to blue:**

Find all instances of:
- `text-purple-600` → Replace with `text-blue-600`
- `bg-purple-600` → Replace with `bg-blue-600`
- `from-purple-600` → Replace with `from-blue-600`
- `to-purple-700` → Replace with `to-blue-700`
- `hover:text-purple-600` → Replace with `hover:text-blue-600`
- `focus:ring-purple-300` → Replace with `focus:ring-blue-300`

**To change to green:**

- Replace `purple-600` with `green-600`
- Replace `purple-700` with `green-700`
- Replace `purple-300` with `green-300`

### Adding a Company Logo

**Location: Line 43 (in header)**

**Current:**
```html
<a href="#" class="text-2xl font-bold gradient-text">
    <i class="fas fa-cog mr-2"></i>Haggis Automations
</a>
```

**To add an image logo:**
```html
<a href="#" class="flex items-center">
    <img src="your-logo.png" alt="Haggis Automations" class="h-10 w-auto mr-3">
    <span class="text-2xl font-bold gradient-text">Haggis Automations</span>
</a>
```

**Note:** You need to have `your-logo.png` in your project folder.

### Changing the Hero Background Image

**Location: Line 540 (in CTA section)**

**Current:**
```html
<div class="absolute inset-0 bg-cover bg-center" style="background-image: url('https://images.unsplash.com/photo-1552664730-d307ca884978?w=1200&h=400&fit=crop'); background-attachment: fixed;">
```

**To change the image:**
```html
<div class="absolute inset-0 bg-cover bg-center" style="background-image: url('https://your-image-url.jpg'); background-attachment: fixed;">
```

You can find free images at:
- Unsplash.com
- Pexels.com
- Pixabay.com

### Adding More Testimonials

Each testimonial card is identical. To add another:

**Find the testimonials section (around line 475)**

**Copy an entire testimonial block:**
```html
<div class="card-hover bg-white rounded-xl shadow-md p-8 border border-gray-100">
    <div class="flex items-center mb-4">
        <i class="fas fa-star text-yellow-400"></i>
        <i class="fas fa-star text-yellow-400"></i>
        <i class="fas fa-star text-yellow-400"></i>
        <i class="fas fa-star text-yellow-400"></i>
        <i class="fas fa-star text-yellow-400"></i>
    </div>
    <p class="text-gray-700 leading-relaxed mb-6">
        "Your testimonial text here..."
    </p>
    <div class="border-t border-gray-200 pt-4">
        <h4 class="font-bold text-gray-900">Name</h4>
        <p class="text-sm text-gray-600">Title</p>
    </div>
</div>
```

**Paste it before the closing `</div>` of the grid and update with new information.**

### Changing Feature Icons

**Location: Lines 183-269 (Features section)**

**Current example (line 188):**
```html
<i class="fas fa-star text-purple-600 text-2xl"></i>
```

**To change the icon:**

Replace `fa-star` with any Font Awesome icon:
- `fa-star` → Star icon
- `fa-lock` → Lock icon
- `fa-globe` → Globe icon
- `fa-paint-brush` → Paintbrush icon
- `fa-chart-line` → Chart icon
- `fa-headset` → Headset icon
- `fa-heart` → Heart icon
- `fa-rocket` → Rocket icon
- `fa-check` → Checkmark icon

**Example change:**
```html
<i class="fas fa-rocket text-purple-600 text-2xl"></i>
```

Find all Font Awesome icons at: https://fontawesome.com/icons

### Adding More FAQ Items

**Location: Lines 579-717 (FAQ section)**

**Copy this complete template:**
```html
<div class="faq-item bg-gray-50 rounded-lg border border-gray-200 overflow-hidden transition-all duration-300">
    <button class="faq-question w-full px-6 py-5 text-left flex items-center justify-between hover:bg-gray-100 transition-colors duration-300 focus:outline-none focus:ring-2 focus:ring-purple-600 focus:ring-inset">
        <h3 class="text-lg font-bold text-gray-900">Your Question Here?</h3>
        <i class="faq-icon fas fa-chevron-down text-purple-600 transition-transform duration-300"></i>
    </button>
    <div class="faq-answer hidden px-6 pb-5 border-t border-gray-200">
        <p class="text-gray-700 leading-relaxed">
            Your answer text here. Make it helpful and clear.
        </p>
    </div>
</div>
```

**Paste it before the closing `</div>` of the FAQ section and update your question and answer.**

---

## Troubleshooting

### Common Issues and Solutions

#### Issue 1: Links Not Working

**Problem:** Clicking a link does nothing or shows "Page not found"

**Solutions:**

1. **Check the href value:**
   ```html
   <!-- Wrong -->
   <a href="privacy">Privacy Policy</a>
   
   <!-- Correct -->
   <a href="privacy.html">Privacy Policy</a>
   ```

2. **Check file exists:**
   - Make sure `privacy.html`, `terms.html`, and `blog.html` are in the same folder as `index.html`
   - Check spelling matches exactly (case-sensitive on some systems)

3. **Check internal links:**
   ```html
   <!-- Wrong -->
   <a href="#feature">Features</a>
   
   <!-- Correct -->
   <a href="#features">Features</a>
   ```
   Make sure the `href` matches the section's `id`

#### Issue 2: Styling Looks Wrong

**Problem:** Colors, spacing, or sizing looks incorrect

**Solutions:**

1. **Hard refresh your browser:**
   - Windows: Press `Ctrl + Shift + R`
   - Mac: Press `Cmd + Shift + R`

2. **Check Tailwind classes are spelled correctly:**
   ```html
   <!-- Wrong -->
   <div class="text-purpl-600">
   
   <!-- Correct -->
   <div class="text-purple-600">
   ```

3. **Check class values are valid:**
   ```html
   <!-- Wrong -->
   <div class="text-99xl">
   
   <!-- Correct -->
   <div class="text-6xl">
   ```

#### Issue 3: Mobile Menu Not Working

**Problem:** Mobile menu button doesn't open/close menu

**Solutions:**

1. **Check JavaScript is not blocked:**
   - Look for browser console errors (press F12)
   - Check if scripts are loading

2. **Verify HTML structure:**
   - Make sure `.mobile-menu-button` element exists (line 67)
   - Make sure `.mobile-menu` element exists (line 71)

3. **Check for typos in class names:**
   ```html
   <!-- Wrong -->
   <button class="mobile-menu-button">
   <div class="mobile-menu">
   
   <!-- Correct - must match exactly -->
   <button class="mobile-menu-button">
   <div class="mobile-menu">
   ```

#### Issue 4: FAQ Accordion Not Working

**Problem:** Clicking FAQ questions doesn't expand/collapse answers

**Solutions:**

1. **Check HTML structure:**
   - Each FAQ item must have `.faq-item` class
   - Must contain `.faq-question` button
   - Must contain `.faq-answer` div
   - Must contain `.faq-icon` for the chevron

2. **Verify JavaScript is loading:**
   - Check browser console for errors (press F12)
   - Make sure script section at bottom is intact

#### Issue 5: Images Not Showing

**Problem:** Images appear as broken icons

**Solutions:**

1. **Check image URL:**
   ```html
   <!-- Wrong - URL doesn't exist -->
   <img src="https://invalid-url.com/image.jpg">
   
   <!-- Correct - use valid URL -->
   <img src="https://images.unsplash.com/photo-valid-id">
   ```

2. **Check file path:**
   ```html
   <!-- Wrong - file not in folder -->
   <img src="images/logo.png">
   
   <!-- Correct - file exists in same folder -->
   <img src="logo.png">
   ```

#### Issue 6: Colors Changed Unexpectedly

**Problem:** Purple colors changed to different color

**Solutions:**

1. **Check for accidental edits:**
   - Search for color classes
   - Verify they haven't been changed

2. **Use Ctrl+Z to undo:**
   - If you made recent changes, undo them

3. **Check browser cache:**
   - Hard refresh: `Ctrl + Shift + R` (Windows) or `Cmd + Shift + R` (Mac)

#### Issue 7: Text Overlapping or Misaligned

**Problem:** Text appears to overlap or is positioned incorrectly

**Solutions:**

1. **Check responsive classes:**
   ```html
   <!-- Make sure responsive prefixes are correct -->
   <h1 class="text-4xl md:text-5xl lg:text-6xl">
   ```

2. **Verify padding/margin classes:**
   ```html
   <!-- Check padding is sufficient -->
   <div class="p-8">
   
   <!-- Check margins between elements -->
   <div class="mb-8">
   ```

3. **Check grid layout:**
   ```html
   <!-- Verify grid columns -->
   <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3">
   ```

### Getting Help

If you encounter an issue not listed above:

1. **Check browser console for errors:**
   - Press F12
   - Click "Console" tab
   - Look for red error messages

2. **Validate your HTML:**
   - Copy your code to https://validator.w3.org/
   - Look for errors highlighted

3. **Compare with original:**
   - Check if changes you made caused the issue
   - Try reverting recent changes

---

## Best Practices

### 1. Always Make Backups

Before making major changes:

1. Duplicate your files
2. Name them with date: `index-backup-2025-01-15.html`
3. Keep them in a safe location

### 2. Make One Change at a Time

1. Change one thing
2. Save the file
3. Test in browser
4. If it works, move to next change
5. If it breaks, undo the change

### 3. Use Consistent Formatting

Keep your code readable:

```html
<!-- Good - easy to read -->
<div class="card-hover bg-white rounded-xl shadow-md p-8 border border-gray-100">
    <h3 class="text-xl font-bold text-gray-900 mb-3">Title</h3>
    <p class="text-gray-700 leading-relaxed">Description</p>
</div>

<!-- Hard to read - avoid -->
<div class="card-hover bg-white rounded-xl shadow-md p-8 border border-gray-100"><h3 class="text-xl font-bold text-gray-900 mb-3">Title</h3><p class="text-gray-700 leading-relaxed">Description</p></div>
```

### 4. Test Responsiveness

After changes, test on multiple devices:

1. **Desktop:** Open in browser (full width)
2. **Tablet:** Resize browser to ~768px width
3. **Mobile:** Resize browser to ~375px width
4. Or use browser DevTools: Press F12, click device icon

### 5. Check Links Regularly

Monthly, test all links:

1. Click every navigation link
2. Click every footer link
3. Click every button
4. Verify they go to correct pages

### 6. Update Content Regularly

Keep your site fresh:

1. Update testimonials quarterly
2. Add new features as you develop them
3. Update "About" section with company changes
4. Keep FAQ current with user questions

### 7. Use Descriptive Text

Make content clear:

```html
<!-- Vague -->
<p>Click here to learn more.</p>

<!-- Clear -->
<p>Learn how Haggis Automations can help your business grow online.</p>
```

### 8. Maintain Consistency

Keep styling consistent:

- Use same colors throughout
- Use same font sizes for similar elements
- Use same spacing between sections
- Keep tone of voice consistent

### 9. Test Before Publishing

Always test changes:

1. Save file
2. Refresh browser (Ctrl+Shift+R)
3. Test on mobile
4. Test all links
5. Check all text displays correctly
6. Then publish

### 10. Document Your Changes

Keep notes of what you changed:

```
2025-01-15:
- Updated hero headline to "Build Your Dreams Online"
- Changed button text to "Start Free Today"
- Added 2 new testimonials
- Updated email to contact@example.com
```

---

## Quick Reference Guide

### File Locations for Common Updates

| What to Update | File | Line(s) |
|---|---|---|
| Header logo/text | index.html | 43-48 |
| Navigation links | index.html | 50-54 |
| Hero headline | index.html | 96-98 |
| Hero subtitle | index.html | 100-102 |
| Hero description | index.html | 104-107 |
| Feature titles | index.html | 194, 209, 224, 239, 254, 269 |
| Testimonials | index.html | 475-527 |
| FAQ questions | index.html | 588, 603, 618, 633, 648 |
| FAQ answers | index.html | 594, 609, 624, 639, 654 |
| Footer email | index.html | 815 |
| Footer social links | index.html | 788-803 |
| Privacy policy content | privacy.html | Entire file |
| Terms content | terms.html | Entire file |

### Common Tailwind Color Classes

```
text-purple-600, text-blue-600, text-red-600, text-green-600, 
text-indigo-600, text-pink-600, text-gray-600, text-yellow-600
```

### Common Tailwind Size Classes

```
Text: text-sm, text-base, text-lg, text-xl, text-2xl, text-3xl, text-4xl, text-5xl, text-6xl
Padding: p-2, p-4, p-6, p-8, p-12, p-16
Margin: m-2, m-4, m-6, m-8, m-12
```

### Keyboard Shortcuts

| Action | Windows | Mac |
|---|---|---|
| Save | Ctrl+S | Cmd+S |
| Undo | Ctrl+Z | Cmd+Z |
| Redo | Ctrl+Y | Cmd+Y |
| Find | Ctrl+F | Cmd+F |
| Find & Replace | Ctrl+H | Cmd+Option+F |
| Hard Refresh | Ctrl+Shift+R | Cmd+Shift+R |
| Developer Tools | F12 | Cmd+Option+I |

---

## Summary

You now have everything you need to maintain and customize your Haggis Automations landing page. Remember:

✅ **Always backup before major changes**

✅ **Test changes in your browser**

✅ **Keep one change per save**

✅ **Use this guide as reference**

✅ **Don't be afraid to experiment**

Your landing page is built on solid, modern technology (Tailwind CSS, Font Awesome icons, responsive design). With these instructions, you can confidently make updates, fix issues, and customize your site to perfectly represent your brand.

**Happy customizing!**