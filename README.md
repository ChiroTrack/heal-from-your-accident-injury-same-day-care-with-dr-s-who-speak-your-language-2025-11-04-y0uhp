# Oakland Accident Care Landing Page - Maintenance & Customization Guide

Welcome! This comprehensive guide will help you maintain and customize the Oakland Accident Care landing page. Whether you're updating text, fixing links, or adding new pages, you'll find clear, step-by-step instructions below.

---

## Table of Contents

1. [Understanding the Page Structure](#understanding-the-page-structure)
2. [Updating Text Content](#updating-text-content)
3. [Modifying Tailwind CSS Classes](#modifying-tailwind-css-classes)
4. [Fixing Broken Links](#fixing-broken-links)
5. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
6. [Troubleshooting Common Issues](#troubleshooting-common-issues)
7. [Best Practices](#best-practices)

---

## Understanding the Page Structure

Before making changes, let's understand how this landing page is organized. The page consists of these main sections:

```
Header/Navigation (sticky at top)
    ↓
Hero Section (main headline and call-to-action)
    ↓
Features Section (Why Choose Us - 3 cards)
    ↓
Benefits Section (3 benefit cards with icons)
    ↓
Testimonials Section (4 customer reviews)
    ↓
About Us Section (company information)
    ↓
Call-to-Action Section (with background image)
    ↓
FAQ Section (5 frequently asked questions)
    ↓
Footer (contact info, links, social media)
```

### Key Technologies Used

- **HTML**: Provides the structure and content
- **Tailwind CSS**: A utility-first CSS framework that handles styling through class names
- **Font Awesome**: Icon library for symbols and graphics
- **Vanilla JavaScript**: Powers interactive features like the mobile menu and FAQ accordion

---

## Updating Text Content

Updating text on your landing page is straightforward. Here's how to do it for each major section:

### 1. Header/Navigation Text

**Location**: Lines 60-77 (Desktop Menu) and 80-87 (Mobile Menu)

**Current Navigation Links:**
```html
<a href="#features" class="text-gray-700 hover:text-blue-600 font-medium transition-colors duration-300">Features</a>
<a href="#benefits" class="text-gray-700 hover:text-blue-600 font-medium transition-colors duration-300">Benefits</a>
<a href="#testimonials" class="text-gray-700 hover:text-blue-600 font-medium transition-colors duration-300">Testimonials</a>
<a href="#faq" class="text-gray-700 hover:text-blue-600 font-medium transition-colors duration-300">FAQ</a>
<a href="#about" class="text-gray-700 hover:text-blue-600 font-medium transition-colors duration-300">About</a>
```

**How to Update Navigation Text:**

1. Open your `index.html` file in a text editor (like VS Code, Notepad++, or Sublime Text)
2. Find the word you want to change (for example, "Features")
3. Replace it with your new text (for example, "Our Services")
4. Make sure you update it in **both** places:
   - Desktop menu (around line 70)
   - Mobile menu (around line 84)

**Example:**
```html
<!-- BEFORE -->
<a href="#features" class="text-gray-700 hover:text-blue-600 font-medium transition-colors duration-300">Features</a>

<!-- AFTER -->
<a href="#features" class="text-gray-700 hover:text-blue-600 font-medium transition-colors duration-300">Our Services</a>
```

### 2. Company Name in Header

**Location**: Lines 51-56

**Current Code:**
```html
<span class="text-2xl font-bold text-gray-900 hidden sm:inline">Oakland Accident Care</span>
<span class="text-xl font-bold text-gray-900 sm:hidden">OAC</span>
```

**How to Update:**

1. Find "Oakland Accident Care" on line 54
2. Replace with your clinic name
3. Also update the abbreviated version "OAC" on line 55

**Example:**
```html
<!-- BEFORE -->
<span class="text-2xl font-bold text-gray-900 hidden sm:inline">Oakland Accident Care</span>
<span class="text-xl font-bold text-gray-900 sm:hidden">OAC</span>

<!-- AFTER -->
<span class="text-2xl font-bold text-gray-900 hidden sm:inline">City Accident Recovery</span>
<span class="text-xl font-bold text-gray-900 sm:hidden">CAR</span>
```

### 3. Hero Section (Main Headline)

**Location**: Lines 103-106

**Current Code:**
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900 leading-tight md:leading-tight lg:leading-tight tracking-tight mb-6">
    Heal from Your Accident Injury
</h1>
```

**How to Update:**

1. Find the text "Heal from Your Accident Injury"
2. Replace with your main headline
3. Keep the HTML tags (`<h1>` and `</h1>`) exactly as they are

**Example:**
```html
<!-- BEFORE -->
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900 leading-tight md:leading-tight lg:leading-tight tracking-tight mb-6">
    Heal from Your Accident Injury
</h1>

<!-- AFTER -->
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900 leading-tight md:leading-tight lg:leading-tight tracking-tight mb-6">
    Get Back on Your Feet After an Accident
</h1>
```

### 4. Hero Subtitle

**Location**: Lines 108-110

**Current Code:**
```html
<p class="text-xl md:text-2xl text-gray-700 font-semibold mb-4">
    Same-Day Care with Dr.'s Who Speak Your Language
</p>
```

**How to Update:**

1. Find the subtitle text
2. Replace with your own subtitle
3. Keep all the class names and HTML tags

**Example:**
```html
<!-- BEFORE -->
<p class="text-xl md:text-2xl text-gray-700 font-semibold mb-4">
    Same-Day Care with Dr.'s Who Speak Your Language
</p>

<!-- AFTER -->
<p class="text-xl md:text-2xl text-gray-700 font-semibold mb-4">
    Expert Treatment • Bilingual Doctors • Zero Cost Upfront
</p>
```

### 5. Hero Description Paragraph

**Location**: Lines 111-115

**Current Code:**
```html
<p class="text-lg md:text-xl text-gray-600 mb-8 max-w-3xl mx-auto leading-relaxed">
    Oakland's car accident recovery clinic where healing happens. Expert medical care, zero cost upfront, and compassionate treatment for all your accident-related injuries.
</p>
```

**How to Update:**

1. Find the description text
2. Replace with your own description
3. This is typically 2-3 sentences explaining what you offer

**Example:**
```html
<!-- BEFORE -->
<p class="text-lg md:text-xl text-gray-600 mb-8 max-w-3xl mx-auto leading-relaxed">
    Oakland's car accident recovery clinic where healing happens. Expert medical care, zero cost upfront, and compassionate treatment for all your accident-related injuries.
</p>

<!-- AFTER -->
<p class="text-lg md:text-xl text-gray-600 mb-8 max-w-3xl mx-auto leading-relaxed">
    We provide comprehensive accident recovery services in Oakland with experienced doctors who speak your language. No upfront costs, same-day appointments, and coordinated care from start to finish.
</p>
```

### 6. Call-to-Action Buttons

**Location**: Lines 117-127

**Current Code:**
```html
<a href="https://oaklandaccidentcare.com" class="px-8 py-4 bg-blue-600 text-white text-lg font-bold rounded-lg btn-primary hover:bg-blue-700 shadow-lg inline-flex items-center space-x-2">
    <span>Schedule Your Appointment Today</span>
    <i class="fas fa-arrow-right"></i>
</a>
<a href="#features" class="px-8 py-4 border-2 border-blue-600 text-blue-600 text-lg font-bold rounded-lg hover:bg-blue-50 transition-colors duration-300 inline-flex items-center space-x-2">
    <span>Learn More</span>
    <i class="fas fa-chevron-down"></i>
</a>
```

**How to Update Button Text:**

1. Find the button text you want to change (e.g., "Schedule Your Appointment Today")
2. Replace with your new button text
3. Keep the `<span>` tags and icon `<i>` tags intact

**Example:**
```html
<!-- BEFORE -->
<span>Schedule Your Appointment Today</span>

<!-- AFTER -->
<span>Book Now - Same Day Available</span>
```

### 7. Hero Stats Section

**Location**: Lines 132-147

**Current Code:**
```html
<div class="grid grid-cols-1 md:grid-cols-3 gap-8 mt-16">
    <div class="text-center">
        <div class="text-4xl md:text-5xl font-bold text-blue-600 mb-2">24/7</div>
        <p class="text-gray-700 text-lg font-semibold">Same-Day Care Available</p>
    </div>
    <div class="text-center">
        <div class="text-4xl md:text-5xl font-bold text-blue-600 mb-2">100%</div>
        <p class="text-gray-700 text-lg font-semibold">Zero Cost Upfront</p>
    </div>
    <div class="text-center">
        <div class="text-4xl md:text-5xl font-bold text-blue-600 mb-2">5★</div>
        <p class="text-gray-700 text-lg font-semibold">Patient Satisfaction</p>
    </div>
</div>
```

**How to Update Stats:**

1. Find the stat numbers (24/7, 100%, 5★)
2. Replace with your own statistics
3. Update the description text below each number

**Example:**
```html
<!-- BEFORE -->
<div class="text-4xl md:text-5xl font-bold text-blue-600 mb-2">24/7</div>
<p class="text-gray-700 text-lg font-semibold">Same-Day Care Available</p>

<!-- AFTER -->
<div class="text-4xl md:text-5xl font-bold text-blue-600 mb-2">500+</div>
<p class="text-gray-700 text-lg font-semibold">Patients Helped This Year</p>
```

### 8. Features Section Title

**Location**: Lines 153-159

**Current Code:**
```html
<h2 class="section-title text-3xl md:text-4xl lg:text-5xl font-bold text-gray-900 mb-4">
    Why Choose Oakland Accident Care?
</h2>
<p class="text-lg text-gray-600 max-w-2xl mx-auto">
    We've designed our clinic specifically to support your recovery with features that prioritize your comfort and healing.
</p>
```

**How to Update:**

1. Replace "Why Choose Oakland Accident Care?" with your own title
2. Update the description paragraph below

**Example:**
```html
<!-- BEFORE -->
<h2 class="section-title text-3xl md:text-4xl lg:text-5xl font-bold text-gray-900 mb-4">
    Why Choose Oakland Accident Care?
</h2>

<!-- AFTER -->
<h2 class="section-title text-3xl md:text-4xl lg:text-5xl font-bold text-gray-900 mb-4">
    What Makes Us Different
</h2>
```

### 9. Individual Feature Cards

**Location**: Lines 162-212 (Three feature cards)

**Current Code Example (First Card):**
```html
<div class="card-hover bg-gradient-to-br from-blue-50 to-indigo-50 rounded-xl p-8 border border-blue-100">
    <div class="w-16 h-16 rounded-lg bg-blue-600 flex items-center justify-center mb-6">
        <i class="fas fa-dollar-sign text-white text-2xl"></i>
    </div>
    <h3 class="text-2xl font-bold text-gray-900 mb-4">Zero Cost Up Front</h3>
    <p class="text-gray-700 leading-relaxed mb-4">
        We understand that accident injuries come with unexpected expenses...
    </p>
    <ul class="space-y-3">
        <li class="flex items-start space-x-3">
            <i class="fas fa-check text-green-500 mt-1 flex-shrink-0"></i>
            <span class="text-gray-700">Direct insurance billing</span>
        </li>
        <!-- More list items -->
    </ul>
</div>
```

**How to Update Feature Cards:**

1. **Change the title**: Replace "Zero Cost Up Front" with your feature title
2. **Change the description**: Replace the paragraph text
3. **Update bullet points**: Replace each list item text
4. **Keep everything else**: Don't modify class names or HTML structure

**Example:**
```html
<!-- BEFORE -->
<h3 class="text-2xl font-bold text-gray-900 mb-4">Zero Cost Up Front</h3>
<p class="text-gray-700 leading-relaxed mb-4">
    We understand that accident injuries come with unexpected expenses...
</p>

<!-- AFTER -->
<h3 class="text-2xl font-bold text-gray-900 mb-4">Affordable Treatment Plans</h3>
<p class="text-gray-700 leading-relaxed mb-4">
    We work with your insurance to make treatment affordable for everyone...
</p>
```

### 10. Benefits Section

**Location**: Lines 216-295

Similar to features, you can update:
- Section title (line 217-221)
- Individual benefit card titles (look for `<h3>` tags)
- Benefit descriptions
- Bullet point lists

### 11. Testimonials Section

**Location**: Lines 299-373

**Current Code Example:**
```html
<div class="card-hover bg-gradient-to-br from-blue-50 to-indigo-50 rounded-xl p-8 border border-blue-100">
    <div class="flex items-center mb-4">
        <div class="w-12 h-12 rounded-full bg-blue-600 flex items-center justify-center text-white font-bold mr-4">
            MJ
        </div>
        <div>
            <h4 class="font-bold text-gray-900">Maria Johnson</h4>
            <p class="text-sm text-gray-600">Oakland, CA</p>
        </div>
    </div>
    <div class="flex items-center mb-4">
        <i class="fas fa-star text-yellow-400"></i>
        <i class="fas fa-star text-yellow-400"></i>
        <i class="fas fa-star text-yellow-400"></i>
        <i class="fas fa-star text-yellow-400"></i>
        <i class="fas fa-star text-yellow-400"></i>
    </div>
    <p class="text-gray-700 leading-relaxed">
        "After my car accident, I was in severe pain..."
    </p>
</div>
```

**How to Update Testimonials:**

1. **Update initials**: Change "MJ" to match the patient's name
2. **Update name**: Replace "Maria Johnson" with actual patient name
3. **Update location**: Replace "Oakland, CA" with patient location or job title
4. **Update testimonial text**: Replace the quote with actual customer feedback
5. **Adjust stars**: Remove or add `<i class="fas fa-star text-yellow-400"></i>` lines for different ratings

**Example:**
```html
<!-- BEFORE -->
<h4 class="font-bold text-gray-900">Maria Johnson</h4>
<p class="text-sm text-gray-600">Oakland, CA</p>
<!-- ... -->
<p class="text-gray-700 leading-relaxed">
    "After my car accident, I was in severe pain..."
</p>

<!-- AFTER -->
<h4 class="font-bold text-gray-900">James Williams</h4>
<p class="text-sm text-gray-600">Construction Worker</p>
<!-- ... -->
<p class="text-gray-700 leading-relaxed">
    "The team helped me recover quickly and got me back to work..."
</p>
```

### 12. About Us Section

**Location**: Lines 377-406

**Current Code:**
```html
<h2 class="text-3xl md:text-4xl lg:text-5xl font-bold mb-8 leading-tight">
    About Oakland Accident Care
</h2>

<div class="space-y-8">
    <p class="text-lg leading-relaxed opacity-95">
        Oakland Accident Care was founded in 2015...
    </p>
    
    <p class="text-lg leading-relaxed opacity-95">
        Our core values are deeply rooted...
    </p>
</div>

<div class="grid grid-cols-3 gap-6 mt-12 pt-8 border-t border-white border-opacity-20">
    <div>
        <div class="text-3xl md:text-4xl font-bold mb-2">10+</div>
        <p class="text-sm md:text-base opacity-90">Years of Excellence</p>
    </div>
    <!-- More stats -->
</div>
```

**How to Update About Section:**

1. **Update title**: Change "About Oakland Accident Care" to your company name
2. **Update paragraphs**: Replace the company history and values paragraphs
3. **Update stats**: Change the numbers and descriptions

**Example:**
```html
<!-- BEFORE -->
<h2 class="text-3xl md:text-4xl lg:text-5xl font-bold mb-8 leading-tight">
    About Oakland Accident Care
</h2>

<!-- AFTER -->
<h2 class="text-3xl md:text-4xl lg:text-5xl font-bold mb-8 leading-tight">
    About Our Clinic
</h2>
```

### 13. FAQ Section

**Location**: Lines 441-595

**Current Code Example (First FAQ Item):**
```html
<div class="faq-item bg-white rounded-xl border border-gray-200 overflow-hidden shadow-md hover:shadow-lg transition-shadow duration-300">
    <button class="faq-question w-full px-8 py-6 text-left flex items-center justify-between hover:bg-blue-50 transition-colors duration-300 cursor-pointer">
        <span class="text-lg md:text-xl font-semibold text-gray-900">What should I do immediately after a car accident?</span>
        <i class="faq-icon fas fa-chevron-down text-blue-600 text-xl transition-transform duration-300"></i>
    </button>
    <div class="faq-answer hidden px-8 pb-6 border-t border-gray-200">
        <p class="text-gray-700 leading-relaxed mb-4">
            First, ensure your safety and the safety of others...
        </p>
        <p class="text-gray-700 leading-relaxed">
            Don't wait to feel pain or symptoms...
        </p>
    </div>
</div>
```

**How to Update FAQ:**

1. **Update question**: Replace the text in the `<span>` tag with your question
2. **Update answer**: Replace the text in the `<div class="faq-answer">` section
3. You can add multiple paragraphs by using multiple `<p>` tags

**Example:**
```html
<!-- BEFORE -->
<span class="text-lg md:text-xl font-semibold text-gray-900">What should I do immediately after a car accident?</span>

<!-- AFTER -->
<span class="text-lg md:text-xl font-semibold text-gray-900">How quickly can I get an appointment?</span>
```

### 14. Footer Text

**Location**: Lines 599-680

**Current Code Example:**
```html
<p class="text-gray-400 leading-relaxed mb-6">
    Your trusted partner in accident recovery. Same-day care, zero cost upfront, and compassionate treatment.
</p>
```

**How to Update Footer:**

1. Update the company description
2. Update contact information
3. Update footer links

**Example:**
```html
<!-- BEFORE -->
<p class="text-gray-400 leading-relaxed mb-6">
    Your trusted partner in accident recovery. Same-day care, zero cost upfront, and compassionate treatment.
</p>

<!-- AFTER -->
<p class="text-gray-400 leading-relaxed mb-6">
    Serving the Oakland community with quality accident care since 2015. Bilingual doctors, zero upfront costs, same-day appointments.
</p>
```

---

## Modifying Tailwind CSS Classes

Tailwind CSS uses utility classes (like `text-blue-600`, `bg-white`, `p-8`) to style elements. If you're comfortable making changes, here's how to modify colors, sizes, and spacing.

### Understanding Tailwind Class Names

Each class name follows a pattern: `property-value`

**Examples:**
- `text-blue-600` = Text color blue, shade 600
- `bg-white` = Background color white
- `p-8` = Padding 8 units
- `rounded-lg` = Border radius large
- `text-2xl` = Font size 2xl

### Common Tailwind Classes in This Page

| Class | What It Does | Example |
|-------|-------------|---------|
| `text-[color]-[shade]` | Text color | `text-blue-600`, `text-gray-900` |
| `bg-[color]-[shade]` | Background color | `bg-blue-600`, `bg-white` |
| `border-[color]-[shade]` | Border color | `border-blue-100` |
| `p-[number]` | Padding (inside space) | `p-8`, `p-4` |
| `m-[number]` | Margin (outside space) | `mb-4` (margin bottom) |
| `text-[size]` | Font size | `text-lg`, `text-2xl`, `text-4xl` |
| `font-[weight]` | Font weight | `font-bold`, `font-semibold` |
| `rounded-[size]` | Border radius | `rounded-lg`, `rounded-xl` |

### Changing Colors

**Location**: Throughout the page, you'll see color classes like `bg-blue-600`, `text-blue-600`, `border-blue-100`

**Current Color Scheme:**
- Primary Blue: `bg-blue-600`, `text-blue-600`
- Light Blue: `bg-blue-50`, `border-blue-100`
- Gray Text: `text-gray-900`, `text-gray-700`, `text-gray-600`

**How to Change the Primary Color:**

1. **Identify all instances** of the color you want to change (e.g., `blue-600`)
2. **Replace with new color** (e.g., `green-600`)
3. **Test on different sections** to ensure consistency

**Example - Changing from Blue to Green:**

```html
<!-- BEFORE: Header button -->
<a href="https://oaklandaccidentcare.com" class="px-6 py-2 bg-blue-600 text-white rounded-lg font-semibold btn-primary hover:bg-blue-700">
    Get Started
</a>

<!-- AFTER: Header button -->
<a href="https://oaklandaccidentcare.com" class="px-6 py-2 bg-green-600 text-white rounded-lg font-semibold btn-primary hover:bg-green-700">
    Get Started
</a>
```

**Available Tailwind Colors:**
- `blue`, `green`, `red`, `yellow`, `purple`, `pink`, `orange`, `emerald`, `teal`, `indigo`, `gray`, `slate`, `stone`, `neutral`, `zinc`

**Color Shades:**
- `50` (very light), `100`, `200`, `300`, `400`, `500`, `600`, `700`, `800`, `900` (very dark)

### Changing Text Size

**Location**: Look for classes like `text-lg`, `text-2xl`, `text-4xl`

**Current Sizes Used:**
- `text-sm` = Small
- `text-lg` = Large
- `text-xl` = Extra Large
- `text-2xl` = 2x Extra Large
- `text-3xl` = 3x Extra Large
- `text-4xl` = 4x Extra Large
- `text-5xl` = 5x Extra Large
- `text-6xl` = 6x Extra Large

**How to Make Text Larger:**

```html
<!-- BEFORE: Hero title -->
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900">
    Heal from Your Accident Injury
</h1>

<!-- AFTER: Larger hero title -->
<h1 class="text-5xl md:text-6xl lg:text-7xl font-bold text-gray-900">
    Heal from Your Accident Injury
</h1>
```

**How to Make Text Smaller:**

```html
<!-- BEFORE: Feature title -->
<h3 class="text-2xl font-bold text-gray-900 mb-4">Zero Cost Up Front</h3>

<!-- AFTER: Smaller feature title -->
<h3 class="text-xl font-bold text-gray-900 mb-4">Zero Cost Up Front</h3>
```

### Changing Spacing (Padding & Margin)

**Padding Classes** (space inside an element):
- `p-4` = Small padding
- `p-8` = Medium padding
- `p-12` = Large padding

**Margin Classes** (space outside an element):
- `mb-4` = Margin bottom small
- `mb-8` = Margin bottom medium
- `mt-6` = Margin top medium
- `gap-8` = Space between grid items

**Example - Increasing Button Padding:**

```html
<!-- BEFORE: Compact button -->
<a href="#" class="px-6 py-2 bg-blue-600 text-white rounded-lg">Get Started</a>

<!-- AFTER: Larger button -->
<a href="#" class="px-8 py-4 bg-blue-600 text-white rounded-lg">Get Started</a>
```

### Responsive Design Classes

This page uses **responsive prefixes** to change styling at different screen sizes:
- `sm:` = Small screens (640px and up)
- `md:` = Medium screens (768px and up)
- `lg:` = Large screens (1024px and up)

**Example - Understanding Responsive Classes:**

```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold">
    Heal from Your Accident Injury
</h1>
```

This means:
- On small phones: `text-4xl` (size 36px)
- On tablets (768px+): `md:text-5xl` (size 48px)
- On desktops (1024px+): `lg:text-6xl` (size 60px)

**How to Modify Responsive Sizing:**

```html
<!-- BEFORE: Small on mobile, grows on larger screens -->
<h2 class="text-3xl md:text-4xl lg:text-5xl font-bold">
    Why Choose Us?
</h2>

<!-- AFTER: Larger on all screens -->
<h2 class="text-4xl md:text-5xl lg:text-6xl font-bold">
    Why Choose Us?
</h2>
```

### Important: Do NOT Modify

⚠️ **Avoid changing these classes** as they control important functionality:

- `sticky`, `top-0`, `z-50` (header positioning)
- `hidden`, `flex`, `grid` (layout structure)
- `transition-all`, `duration-300` (animations)
- `absolute`, `relative` (positioning)

---

## Fixing Broken Links

Broken links prevent users from navigating your site properly. Let's identify and fix all links on this page.

### Types of Links on This Page

1. **Internal Links** - Links that point to sections within the same page (using `#`)
2. **External Links** - Links that point to external websites
3. **Contact Links** - Email and phone links
4. **Policy Links** - Privacy and Terms pages

### Finding All Links

Here's a complete list of all links currently in the page:

| Link Type | Location | Current Value | Purpose |
|-----------|----------|----------------|---------|
| Features Nav | Header (Line 68) | `#features` | Jump to Features section |
| Benefits Nav | Header (Line 69) | `#benefits` | Jump to Benefits section |
| Testimonials Nav | Header (Line 70) | `#testimonials` | Jump to Testimonials section |
| FAQ Nav | Header (Line 71) | `#faq` | Jump to FAQ section |
| About Nav | Header (Line 72) | `#about` | Jump to About section |
| Get Started (Header) | Header (Line 73) | `https://oaklandaccidentcare.com` | External booking page |
| Schedule Button (Hero) | Hero (Line 119) | `https://oaklandaccidentcare.com` | External booking page |
| Learn More Button | Hero (Line 124) | `#features` | Jump to Features section |
| Book Appointment (CTA) | CTA Section (Line 378) | `https://oaklandaccidentcare.com` | External booking page |
| Email Us (CTA) | CTA Section (Line 382) | `mailto:Frontdesk@oaklandaccidentcare.com` | Send email |
| Privacy Policy (Footer) | Footer (Line 631) | `privacy.html` | Privacy policy page |
| Terms of Service (Footer) | Footer (Line 635) | `terms.html` | Terms page |
| Blog (Footer) | Footer (Line 639) | `blog.html` | Blog page |
| Social Media (Footer) | Footer (Lines 618-627) | `#` | Placeholder links |

### How to Fix Internal Navigation Links

**Location**: Lines 68-72 (Desktop Navigation)

**Current Code:**
```html
<a href="#features" class="text-gray-700 hover:text-blue-600 font-medium transition-colors duration-300">Features</a>
<a href="#benefits" class="text-gray-700 hover:text-blue-600 font-medium transition-colors duration-300">Benefits</a>
<a href="#testimonials" class="text-gray-700 hover:text-blue-600 font-medium transition-colors duration-300">Testimonials</a>
<a href="#faq" class="text-gray-700 hover:text-blue-600 font-medium transition-colors duration-300">FAQ</a>
<a href="#about" class="text-gray-700 hover:text-blue-600 font-medium transition-colors duration-300">About</a>
```

**Step-by-Step: Verify Internal Links Work**

1. Open the page in a web browser
2. Click each navigation link
3. Verify it jumps to the correct section
4. If it doesn't work, check that the section ID matches the link

**Example - Fixing a Broken Internal Link:**

```html
<!-- BEFORE: Link points to non-existent section -->
<a href="#services" class="text-gray-700 hover:text-blue-600 font-medium transition-colors duration-300">Services</a>

<!-- AFTER: Link points to correct section ID -->
<a href="#benefits" class="text-gray-700 hover:text-blue-600 font-medium transition-colors duration-300">Services</a>
```

**Verify Section IDs Exist:**

Make sure every link target has a matching section ID:

```html
<!-- Navigation link -->
<a href="#features">Features</a>

<!-- Must have matching section with this ID -->
<section id="features">
    <!-- Section content -->
</section>
```

### How to Fix External Links

**Location**: Multiple locations (lines 73, 119, 124, 378, 382)

**Current Code Examples:**
```html
<!-- Header button -->
<a href="https://oaklandaccidentcare.com" class="px-6 py-2 bg-blue-600 text-white rounded-lg">Get Started</a>

<!-- Hero button -->
<a href="https://oaklandaccidentcare.com" class="px-8 py-4 bg-blue-600 text-white rounded-lg">Schedule Your Appointment Today</a>

<!-- Email link -->
<a href="mailto:Frontdesk@oaklandaccidentcare.com" class="text-gray-400 hover:text-blue-400">Frontdesk@oaklandaccidentcare.com</a>
```

**Step-by-Step: Update External Links**

1. **Identify the link** you want to change
2. **Update the `href` attribute** with your new URL
3. **Test the link** in a web browser

**Example - Updating Booking Page Link:**

```html
<!-- BEFORE: Points to old booking page -->
<a href="https://oaklandaccidentcare.com" class="px-6 py-2 bg-blue-600 text-white rounded-lg">Get Started</a>

<!-- AFTER: Points to new booking page -->
<a href="https://mybookingapp.com/oakland-care" class="px-6 py-2 bg-blue-600 text-white rounded-lg">Get Started</a>
```

### How to Update Email Links

**Location**: Line 382 (CTA Section) and Line 650 (Footer)

**Current Code:**
```html
<a href="mailto:Frontdesk@oaklandaccidentcare.com" class="inline-flex items-center space-x-2">
    <span>Email Us</span>
    <i class="fas fa-envelope"></i>
</a>
```

**Step-by-Step: Change Email Address**

1. Find `mailto:Frontdesk@oaklandaccidentcare.com`
2. Replace with your email address
3. Keep the `mailto:` prefix

**Example:**
```html
<!-- BEFORE -->
<a href="mailto:Frontdesk@oaklandaccidentcare.com">Email Us</a>

<!-- AFTER -->
<a href="mailto:contact@yourclinic.com">Email Us</a>
```

### How to Fix Policy Links

**Location**: Lines 631-639 (Footer)

**Current Code:**
```html
<div class="text-center md:text-left">
    <a href="privacy.html" class="text-gray-400 hover:text-blue-400 transition-colors duration-300 font-medium">Privacy Policy</a>
</div>
<div class="text-center">
    <a href="terms.html" class="text-gray-400 hover:text-blue-400 transition-colors duration-300 font-medium">Terms of Service</a>
</div>
<div class="text-center md:text-right">
    <a href="blog.html" class="text-gray-400 hover:text-blue-400 transition-colors duration-300 font-medium">Blog</a>
</div>
```

**Step-by-Step: Fix Policy Links**

1. **Check if files exist** - Do you have `privacy.html`, `terms.html`, and `blog.html` files?
2. **If files exist** - Verify the file paths are correct
3. **If files don't exist** - Either create them or remove the links

**Example - If Files Exist in Same Directory:**

```html
<!-- BEFORE: Links to files -->
<a href="privacy.html">Privacy Policy</a>
<a href="terms.html">Terms of Service</a>
<a href="blog.html">Blog</a>

<!-- AFTER: Files verified and working -->
<!-- (No change needed if paths are correct) -->
```

**Example - If Files Are in a Subdirectory:**

```html
<!-- BEFORE: Files in root directory -->
<a href="privacy.html">Privacy Policy</a>

<!-- AFTER: Files in /pages directory -->
<a href="pages/privacy.html">Privacy Policy</a>
```

### How to Fix Social Media Links

**Location**: Lines 618-627 (Footer)

**Current Code:**
```html
<a href="#" class="w-10 h-10 rounded-lg bg-gray-800 flex items-center justify-center hover:bg-blue-600 transition-colors duration-300" aria-label="Facebook">
    <i class="fab fa-facebook-f text-white"></i>
</a>
<a href="#" class="w-10 h-10 rounded-lg bg-gray-800 flex items-center justify-center hover:bg-blue-600 transition-colors duration-300" aria-label="Twitter">
    <i class="fab fa-twitter text-white"></i>
</a>
<a href="#" class="w-10 h-10 rounded-lg bg-gray-800 flex items-center justify-center hover:bg-blue-600 transition-colors duration-300" aria-label="Instagram">
    <i class="fab fa-instagram text-white"></i>
</a>
<a href="#" class="w-10 h-10 rounded-lg bg-gray-800 flex items-center justify-center hover:bg-blue-600 transition-colors duration-300" aria-label="LinkedIn">
    <i class="fab fa-linkedin-in text-white"></i>
</a>
```

**Step-by-Step: Update Social Media Links**

1. **Replace the `#`** with your social media profile URL
2. **Keep the icon class** (e.g., `fa-facebook-f`) the same

**Example - Updating Social Media:**

```html
<!-- BEFORE: Placeholder links -->
<a href="#" aria-label="Facebook">
    <i class="fab fa-facebook-f text-white"></i>
</a>

<!-- AFTER: Actual social media links -->
<a href="https://www.facebook.com/oaklandaccidentcare" aria-label="Facebook">
    <i class="fab fa-facebook-f text-white"></i>
</a>
```

### Troubleshooting Link Issues

**Problem: Link doesn't work when clicked**

**Solutions:**
1. Check that the `href` value is correct
2. For internal links, verify the target section has the matching `id`
3. For external links, test the URL in a new browser tab
4. Check for typos in the URL

**Problem: Email link doesn't open email client**

**Solution:**
- Make sure the link starts with `mailto:` followed by the email address
- Example: `<a href="mailto:contact@example.com">`

**Problem: Navigation links don't scroll to sections**

**Solutions:**
1. Verify the link has a `#` followed by the section ID
2. Verify the section has a matching `id` attribute
3. Check that you're not using the same ID twice on the page

---

## Adding Privacy and Terms Pages

Currently, the footer links to `privacy.html` and `terms.html` files that don't exist. Let's create these pages and link them properly.

### Step 1: Create the Privacy Policy Page

**Step-by-Step Instructions:**

1. **Create a new file** in the same folder as your `index.html`
   - Right-click in your file explorer
   - Select "New" → "Text Document"
   - Name it `privacy.html`

2. **Copy the following code** into your new `privacy.html` file:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Privacy Policy for Oakland Accident Care">
    <title>Privacy Policy - Oakland Accident Care</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        html {
            scroll-behavior: smooth;
        }
    </style>
</head>
<body class="bg-white text-gray-900">
    <!-- Header & Navigation -->
    <header class="sticky top-0 z-50 bg-white shadow-md">
        <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-20">
                <div class="flex items-center space-x-2">
                    <div class="w-10 h-10 rounded-lg bg-blue-600 flex items-center justify-center">
                        <i class="fas fa-heart text-white text-lg"></i>
                    </div>
                    <a href="index.html" class="text-2xl font-bold text-gray-900 hidden sm:inline">Oakland Accident Care</a>
                    <a href="index.html" class="text-xl font-bold text-gray-900 sm:hidden">OAC</a>
                </div>
                <a href="index.html" class="px-6 py-2 bg-blue-600 text-white rounded-lg font-semibold hover:bg-blue-700">
                    Back to Home
                </a>
            </div>
        </nav>
    </header>

    <!-- Main Content -->
    <section class="py-20 md:py-28 lg:py-32">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <h1 class="text-4xl md:text-5xl font-bold text-gray-900 mb-8">Privacy Policy</h1>
            <div class="prose prose-lg max-w-none">
                <p class="text-gray-700 leading-relaxed mb-6">
                    <strong>Last Updated: January 2025</strong>
                </p>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">1. Introduction</h2>
                <p class="text-gray-700 leading-relaxed mb-6">
                    Oakland Accident Care ("we," "us," "our," or "Company") is committed to protecting your privacy. This Privacy Policy explains how we collect, use, disclose, and safeguard your information when you visit our website.
                </p>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">2. Information We Collect</h2>
                <p class="text-gray-700 leading-relaxed mb-4">
                    We may collect information about you in a variety of ways. The information we may collect on the Site includes:
                </p>
                <ul class="list-disc list-inside text-gray-700 mb-6 space-y-2">
                    <li>Personal Data: Name, email address, phone number, and appointment information</li>
                    <li>Medical Information: Health history and treatment details (with your consent)</li>
                    <li>Insurance Information: Insurance provider and policy details</li>
                    <li>Usage Data: Browser type, IP address, pages visited, and time spent on pages</li>
                </ul>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">3. How We Use Your Information</h2>
                <p class="text-gray-700 leading-relaxed mb-4">
                    Having accurate information about you permits us to provide you with a smooth, efficient, and customized experience. Specifically, we may use information collected about you via the Site to:
                </p>
                <ul class="list-disc list-inside text-gray-700 mb-6 space-y-2">
                    <li>Schedule and manage your medical appointments</li>
                    <li>Process insurance claims and billing</li>
                    <li>Provide medical treatment and care coordination</li>
                    <li>Communicate with you about your care</li>
                    <li>Improve our website and services</li>
                    <li>Comply with legal obligations</li>
                </ul>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">4. Protection of Your Information</h2>
                <p class="text-gray-700 leading-relaxed mb-6">
                    We implement a variety of security measures to maintain the safety of your personal information. Your personal information is contained behind secured networks and is only accessible by a limited number of persons who have special access rights to such systems, and are required to keep the information confidential.
                </p>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">5. Disclosure of Your Information</h2>
                <p class="text-gray-700 leading-relaxed mb-6">
                    We may share your information with third parties only when necessary to provide our services, including insurance providers, healthcare partners, and legal authorities when required by law.
                </p>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">6. Contact Us</h2>
                <p class="text-gray-700 leading-relaxed mb-6">
                    If you have questions or comments about this Privacy Policy, please contact us at:
                </p>
                <p class="text-gray-700 leading-relaxed mb-6">
                    Oakland Accident Care<br>
                    Email: <a href="mailto:Frontdesk@oaklandaccidentcare.com" class="text-blue-600 hover:text-blue-800">Frontdesk@oaklandaccidentcare.com</a><br>
                    Location: Oakland, California
                </p>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-gray-300 py-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <p class="text-gray-500">
                &copy; 2025 Oakland Accident Care. All rights reserved.
            </p>
        </div>
    </footer>
</body>
</html>
```

3. **Save the file** in the same folder as your `index.html`

### Step 2: Create the Terms of Service Page

**Step-by-Step Instructions:**

1. **Create a new file** named `terms.html`
2. **Copy the following code** into your new `terms.html` file:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Terms of Service for Oakland Accident Care">
    <title>Terms of Service - Oakland Accident Care</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        html {
            scroll-behavior: smooth;
        }
    </style>
</head>
<body class="bg-white text-gray-900">
    <!-- Header & Navigation -->
    <header class="sticky top-0 z-50 bg-white shadow-md">
        <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-20">
                <div class="flex items-center space-x-2">
                    <div class="w-10 h-10 rounded-lg bg-blue-600 flex items-center justify-center">
                        <i class="fas fa-heart text-white text-lg"></i>
                    </div>
                    <a href="index.html" class="text-2xl font-bold text-gray-900 hidden sm:inline">Oakland Accident Care</a>
                    <a href="index.html" class="text-xl font-bold text-gray-900 sm:hidden">OAC</a>
                </div>
                <a href="index.html" class="px-6 py-2 bg-blue-600 text-white rounded-lg font-semibold hover:bg-blue-700">
                    Back to Home
                </a>
            </div>
        </nav>
    </header>

    <!-- Main Content -->
    <section class="py-20 md:py-28 lg:py-32">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <h1 class="text-4xl md:text-5xl font-bold text-gray-900 mb-8">Terms of Service</h1>
            <div class="prose prose-lg max-w-none">
                <p class="text-gray-700 leading-relaxed mb-6">
                    <strong>Last Updated: January 2025</strong>
                </p>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">1. Acceptance of Terms</h2>
                <p class="text-gray-700 leading-relaxed mb-6">
                    By accessing and using this website, you accept and agree to be bound by the terms and provision of this agreement. If you do not agree to abide by the above, please do not use this service.
                </p>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">2. Use License</h2>
                <p class="text-gray-700 leading-relaxed mb-6">
                    Permission is granted to temporarily download one copy of the materials (information or software) on Oakland Accident Care's website for personal, non-commercial transitory viewing only. This is the grant of a license, not a transfer of title, and under this license you may not:
                </p>
                <ul class="list-disc list-inside text-gray-700 mb-6 space-y-2">
                    <li>Modifying or copying the materials</li>
                    <li>Using the materials for any commercial purpose or for any public display</li>
                    <li>Attempting to decompile or reverse engineer any software contained on the website</li>
                    <li>Removing any copyright or other proprietary notations from the materials</li>
                    <li>Transferring the materials to another person or "mirroring" the materials on any other server</li>
                </ul>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">3. Disclaimer</h2>
                <p class="text-gray-700 leading-relaxed mb-6">
                    The materials on Oakland Accident Care's website are provided "as is". Oakland Accident Care makes no warranties, expressed or implied, and hereby disclaims and negates all other warranties including, without limitation, implied warranties or conditions of merchantability, fitness for a particular purpose, or non-infringement of intellectual property or other violation of rights.
                </p>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">4. Limitations</h2>
                <p class="text-gray-700 leading-relaxed mb-6">
                    In no event shall Oakland Accident Care or its suppliers be liable for any damages (including, without limitation, damages for loss of data or profit, or due to business interruption) arising out of the use or inability to use the materials on Oakland Accident Care's website.
                </p>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">5. Accuracy of Materials</h2>
                <p class="text-gray-700 leading-relaxed mb-6">
                    The materials appearing on Oakland Accident Care's website could include technical, typographical, or photographic errors. Oakland Accident Care does not warrant that any of the materials on its website are accurate, complete, or current. Oakland Accident Care may make changes to the materials contained on its website at any time without notice.
                </p>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">6. Links</h2>
                <p class="text-gray-700 leading-relaxed mb-6">
                    Oakland Accident Care has not reviewed all of the sites linked to its website and is not responsible for the contents of any such linked site. The inclusion of any link does not imply endorsement by Oakland Accident Care of the site. Use of any such linked website is at the user's own risk.
                </p>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">7. Modifications</h2>
                <p class="text-gray-700 leading-relaxed mb-6">
                    Oakland Accident Care may revise these terms of service for its website at any time without notice. By using this website, you are agreeing to be bound by the then current version of these terms of service.
                </p>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">8. Contact Us</h2>
                <p class="text-gray-700 leading-relaxed mb-6">
                    If you have any questions about these Terms of Service, please contact us at:
                </p>
                <p class="text-gray-700 leading-relaxed mb-6">
                    Oakland Accident Care<br>
                    Email: <a href="mailto:Frontdesk@oaklandaccidentcare.com" class="text-blue-600 hover:text-blue-800">Frontdesk@oaklandaccidentcare.com</a><br>
                    Location: Oakland, California
                </p>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-gray-300 py-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <p class="text-gray-500">
                &copy; 2025 Oakland Accident Care. All rights reserved.
            </p>
        </div>
    </footer>
</body>
</html>
```

3. **Save the file** in the same folder as your `index.html`

### Step 3: Verify the Links Work

**Step-by-Step Verification:**

1. **Open your `index.html`** in a web browser
2. **Scroll to the footer** at the bottom of the page
3. **Click on "Privacy Policy"** link
4. **Verify it opens** the privacy page you just created
5. **Click "Back to Home"** to return to the main page
6. **Click on "Terms of Service"** link
7. **Verify it opens** the terms page you just created

### Step 4: Update Footer Links (If Needed)

**Location**: Lines 631-639 in your `index.html`

**Current Code:**
```html
<div class="text-center md:text-left">
    <a href="privacy.html" class="text-gray-400 hover:text-blue-400 transition-colors duration-300 font-medium">Privacy Policy</a>
</div>
<div class="text-center">
    <a href="terms.html" class="text-gray-400 hover:text-blue-400 transition-colors duration-300 font-medium">Terms of Service</a>
</div>
```

**If your files are in the same folder as `index.html`**, the links are already correct!

**If your files are in a subdirectory**, update the paths:

```html
<!-- BEFORE: Files in root directory -->
<a href="privacy.html">Privacy Policy</a>
<a href="terms.html">Terms of Service</a>

<!-- AFTER: Files in /legal directory -->
<a href="legal/privacy.html">Privacy Policy</a>
<a href="legal/terms.html">Terms of Service</a>
```

### Step 5: Optional - Create a Blog Page

If you want to enable the blog link in the footer, follow the same process:

1. **Create a new file** named `blog.html`
2. **Copy the privacy page code** as a template
3. **Modify the title and content** for your blog
4. **Save the file** in the same folder as `index.html`

---

## Troubleshooting Common Issues

### Issue 1: Changes Don't Appear on the Website

**Problem:** You made changes to the HTML file, but they don't show up when you view the page.

**Solutions:**

1. **Hard refresh your browser**
   - Windows: Press `Ctrl + Shift + R`
   - Mac: Press `Cmd + Shift + R`
   - Or clear your browser cache

2. **Save your file**
   - Make sure you saved the changes in your text editor
   - Look for a dot or asterisk next to the filename (indicates unsaved changes)

3. **Reload the page**
   - Click the refresh button in your browser
   - Or press `F5` or `Ctrl + R`

### Issue 2: Styling Looks Broken (Colors Wrong, Text Misaligned)

**Problem:** After making changes, the page styling looks broken.

**Solutions:**

1. **Check for typos in class names**
   - Tailwind class names are case-sensitive
   - Example: `text-Blue-600` won't work; use `text-blue-600`

2. **Don't remove class attributes**
   - Example of WRONG: `<div>Text</div>`
   - Example of RIGHT: `<div class="text-blue-600">Text</div>`

3. **Verify you didn't break HTML structure**
   - Make sure all opening tags have closing tags
   - Example: `<div class="...">content</div>` (not `<div>content`)

4. **Check the browser console for errors**
   - Press `F12` to open Developer Tools
   - Look for red error messages in the Console tab

### Issue 3: Links Don't Work

**Problem:** Clicking a link does nothing or shows a 404 error.

**Solutions:**

1. **For internal links (jump to sections)**
   - Verify the link uses a `#` symbol: `<a href="#features">`
   - Verify the target section has matching ID: `<section id="features">`

2. **For external links**
   - Test the URL in a new browser tab
   - Make sure the URL is complete (includes `https://`)

3. **For file links**
   - Verify the file exists in the correct location
   - Check the file path is correct
   - Make sure the filename matches exactly (including capitalization)

### Issue 4: Mobile Menu Doesn't Work

**Problem:** The hamburger menu on mobile doesn't open/close.

**Solutions:**

1. **Don't remove the mobile menu JavaScript**
   - The JavaScript code at the bottom (lines 683-720) controls the menu
   - Don't delete or modify this code

2. **Verify HTML structure is intact**
   - Don't remove classes like `mobile-menu`, `mobile-menu-button`
   - Don't remove the `hidden` class from the mobile menu

3. **Test on actual mobile device**
   - Resize your browser window to test mobile view
   - Or open the page on an actual phone

### Issue 5: FAQ Accordion Doesn't Expand/Collapse

**Problem:** Clicking FAQ questions doesn't expand the answers.

**Solutions:**

1. **Don't modify the FAQ JavaScript**
   - The code at lines 708-723 controls the accordion
   - Keep this code intact

2. **Verify HTML structure**
   - Don't remove classes: `faq-item`, `faq-question`, `faq-answer`, `faq-icon`
   - Keep the `hidden` class on the answer div

3. **Check that you're using the correct structure**
   - Each FAQ item must have: question button + answer div
   - The answer div must start with `hidden` class

### Issue 6: Page Looks Different on Mobile

**Problem:** The page displays incorrectly on phones or tablets.

**Solutions:**

1. **Don't remove responsive classes**
   - Classes like `md:text-5xl`, `lg:text-6xl` control mobile responsiveness
   - Keep these in place

2. **Test on different screen sizes**
   - Resize your browser window to test
   - Use browser Developer Tools (F12) → Device Toolbar

3. **Check that viewport meta tag exists**
   - Line 5 should have: `<meta name="viewport" content="width=device-width, initial-scale=1.0">`
   - Don't remove or modify this line

### Issue 7: Images or Icons Don't Show

**Problem:** Images or Font Awesome icons appear as broken or missing.

**Solutions:**

1. **For Font Awesome icons**
   - Verify the CDN link is intact (line 31)
   - Don't remove this line: `<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">`

2. **For custom images**
   - Make sure the image file exists
   - Check the file path is correct
   - Verify the file format is supported (.jpg, .png, .gif, .webp)

3. **Check your internet connection**
   - External resources (CDNs) require internet access
   - If offline, external icons won't load

---

## Best Practices

### 1. Always Back Up Your Files

**Before making changes:**

1. Create a copy of your `index.html` file
   - Right-click the file → Copy
   - Right-click in folder → Paste
   - Rename to `index-backup.html`

2. Use version control (optional but recommended)
   - Use Git to track changes
   - Makes it easy to revert if something breaks

### 2. Make Changes Incrementally

**Don't:**
- Change multiple things at once
- Make big edits without testing

**Do:**
- Change one section at a time
- Test after each change
- Save frequently

### 3. Test Across Browsers

**Test your page in:**
- Chrome
- Firefox
- Safari
- Edge

**Test on multiple devices:**
- Desktop computer
- Tablet
- Mobile phone

### 4. Use a Code Editor

**Recommended editors (free):**
- Visual Studio Code
- Sublime Text
- Notepad++
- Atom

**Avoid:**
- Microsoft Word (adds formatting)
- Regular Notepad (limited features)

### 5. Keep the Structure Consistent

**Maintain consistent:**
- Indentation (2 or 4 spaces)
- Naming conventions
- Color schemes
- Font sizes

### 6. Document Your Changes

**Keep track of:**
- What you changed
- When you changed it
- Why you changed it

**Example comment:**
```html
<!-- Updated hero title on Jan 15, 2025 - Changed from "Heal from Your Accident Injury" to new title -->
<h1>New title here</h1>
```

### 7. Test All Links Regularly

**Monthly checklist:**
- [ ] Test all navigation links
- [ ] Test all external links
- [ ] Test email links
- [ ] Test phone links (if any)
- [ ] Test buttons

### 8. Keep Content Updated

**Update regularly:**
- Patient testimonials (quarterly)
- Statistics (annually)
- Contact information (as needed)
- Hours of operation (as needed)
- Services offered (as needed)

### 9. Monitor Performance

**Check:**
- Page loading speed
- Mobile responsiveness
- SEO rankings
- User engagement

### 10. Security Considerations

**Important:**
- Don't share your source code publicly
- Keep sensitive information (emails, phone numbers) secure
- Use HTTPS for your website
- Keep backups of important files
- Don't hardcode API keys or passwords

---

## Common Customization Examples

### Example 1: Change Primary Color from Blue to Green

**Step 1:** Find all instances of `blue-600`

**Step 2:** Replace with `green-600`

```html
<!-- BEFORE -->
<div class="w-10 h-10 rounded-lg bg-blue-600 flex items-center justify-center">
    <i class="fas fa-heart text-white text-lg"></i>
</div>

<!-- AFTER -->
<div class="w-10 h-10 rounded-lg bg-green-600 flex items-center justify-center">
    <i class="fas fa-heart text-white text-lg"></i>
</div>
```

**Locations to change:**
- Header logo background
- Navigation hover color
- Button backgrounds
- Section accent colors
- Feature card icons

### Example 2: Add a New Testimonial

**Step 1:** Find the testimonials section (line 299)

**Step 2:** Copy an existing testimonial card

**Step 3:** Paste it and update the information

```html
<!-- NEW TESTIMONIAL -->
<div class="card-hover bg-gradient-to-br from-blue-50 to-indigo-50 rounded-xl p-8 border border-blue-100">
    <div class="flex items-center mb-4">
        <div class="w-12 h-12 rounded-full bg-blue-600 flex items-center justify-center text-white font-bold mr-4">
            JD
        </div>
        <div>
            <h4 class="font-bold text-gray-900">John Davis</h4>
            <p class="text-sm text-gray-600">Business Owner</p>
        </div>
    </div>
    <div class="flex items-center mb-4">
        <i class="fas fa-star text-yellow-400"></i>
        <i class="fas fa-star text-yellow-400"></i>
        <i class="fas fa-star text-yellow-400"></i>
        <i class="fas fa-star text-yellow-400"></i>
        <i class="fas fa-star text-yellow-400"></i>
    </div>
    <p class="text-gray-700 leading-relaxed">
        "Great experience from start to finish. The team was professional and caring. Highly recommended!"
    </p>
</div>
```

### Example 3: Update Contact Information

**Step 1:** Find the footer contact section (line 650)

**Step 2:** Update the email address

```html
<!-- BEFORE -->
<li class="flex items-start space-x-3">
    <i class="fas fa-envelope text-blue-400 mt-1 flex-shrink-0"></i>
    <a href="mailto:Frontdesk@oaklandaccidentcare.com" class="text-gray-400 hover:text-blue-400">Frontdesk@oaklandaccidentcare.com</a>
</li>

<!-- AFTER -->
<li class="flex items-start space-x-3">
    <i class="fas fa-envelope text-blue-400 mt-1 flex-shrink-0"></i>
    <a href="mailto:contact@yourclinic.com" class="text-gray-400 hover:text-blue-400">contact@yourclinic.com</a>
</li>
```

### Example 4: Change Button Text

**Find all buttons** using `<a>` tags with `btn-primary` class

**Update the text** inside the `<span>` tag

```html
<!-- BEFORE -->
<a href="https://oaklandaccidentcare.com" class="px-8 py-4 bg-blue-600 text-white text-lg font-bold rounded-lg btn-primary">
    <span>Schedule Your Appointment Today</span>
    <i class="fas fa-arrow-right"></i>
</a>

<!-- AFTER -->
<a href="https://oaklandaccidentcare.com" class="px-8 py-4 bg-blue-600 text-white text-lg font-bold rounded-lg btn-primary">
    <span>Book Your Free Consultation</span>
    <i class="fas fa-arrow-right"></i>
</a>
```

---

## Quick Reference Guide

### File Structure

```
your-project-folder/
├── index.html          (Main landing page)
├── privacy.html        (Privacy policy page)
├── terms.html          (Terms of service page)
├── blog.html           (Optional blog page)
└── README.md           (This file)
```

### Key Sections in index.html

| Section | Line Numbers | Purpose |
|---------|-------------|---------|
| Head/Meta Tags | 1-45 | SEO and page settings |
| Header/Navigation | 47-89 | Top menu and logo |
| Hero Section | 91-147 | Main headline and CTA |
| Features Section | 149-213 | Why choose us cards |
| Benefits Section | 215-295 | Benefit cards |
| Testimonials Section | 297-373 | Customer reviews |
| About Section | 375-406 | Company information |
| CTA Section | 408-430 | Call to action with background |
| FAQ Section | 432-595 | Frequently asked questions |
| Footer | 597-680 | Contact, links, social media |
| JavaScript | 682-721 | Interactive features |

### Tailwind Color Reference

**Primary Colors:**
- `blue-600` (main color)
- `blue-50` (light background)
- `blue-100` (light border)

**Secondary Colors:**
- `emerald-600` (green accent)
- `purple-600` (purple accent)
- `orange-600` (orange accent)

**Neutral Colors:**
- `gray-900` (dark text)
- `gray-700` (medium text)
- `gray-600` (light text)
- `white` (backgrounds)

### Common Tailwind Sizes

**Text Sizes:**
- `text-sm` = 14px
- `text-lg` = 18px
- `text-xl` = 20px
- `text-2xl` = 24px
- `text-3xl` = 30px
- `text-4xl` = 36px
- `text-5xl` = 48px
- `text-6xl` = 60px

**Padding/Margin:**
- `p-4` = 16px padding
- `p-8` = 32px padding
- `mb-4` = 16px margin bottom
- `mt-8` = 32px margin top

---

## Getting Help

### Resources

- **Tailwind CSS Documentation**: https://tailwindcss.com/docs
- **Font Awesome Icons**: https://fontawesome.com/icons
- **HTML Reference**: https://developer.mozilla.org/en-US/docs/Web/HTML
- **CSS Reference**: https://developer.mozilla.org/en-US/docs/Web/CSS

### Common Questions

**Q: How do I add more features cards?**
A: Copy one feature card (lines 162-212) and paste it in the same section. Update the title, description, icon, and bullet points.

**Q: How do I change the page background color?**
A: Find the `<body>` tag (line 39) and change `bg-white` to your desired color.

**Q: How do I add a new section?**
A: Copy an existing section, update the ID, title, and content. Make sure to add a corresponding navigation link.

**Q: How do I make the page faster?**
A: Optimize images, minimize CSS/JavaScript, and use a Content Delivery Network (CDN) for external resources.

**Q: How do I track visitor analytics?**
A: Add Google Analytics or similar service by adding a tracking code to the `<head>` section.

---

## Summary

Congratulations! You now have a comprehensive guide for maintaining and customizing your Oakland Accident Care landing page. 

**Key Takeaways:**

✅ **Updating text** is simple - just find and replace
✅ **Modifying colors** uses Tailwind utility classes
✅ **Fixing links** requires checking hrefs and file paths
✅ **Creating policy pages** follows a simple template
✅ **Always backup** before making changes
✅ **Test thoroughly** across devices and browsers
✅ **Keep your code organized** for future maintenance

**Next Steps:**

1. Back up your current `index.html` file
2. Create `privacy.html` and `terms.html` pages
3. Test all links and functionality
4. Update content with your actual information
5. Customize colors and styling to match your brand
6. Launch your website!

Good luck with your Oakland Accident Care landing page! 🎉