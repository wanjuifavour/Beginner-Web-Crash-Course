# 📚 HTML5 Cheatsheet - Lesson 1

*A comprehensive reference guide for HTML fundamentals*

---

## 🏗️ Basic Document Structure

Every HTML document starts with this foundation:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Page description for SEO">
    <title>My First Page</title>
</head>
<body>
    <!-- Your content goes here -->
</body>
</html>
```

### What each part does:
- `<!DOCTYPE html>`: Tells browser this is HTML5
- `<html lang="en">`: Root element with language specification
- `<head>`: Contains metadata (not visible on page)
- `<body>`: Contains all visible content

---

## 📝 Text Content & Formatting

### Headings (Hierarchy Matters!)
```html
<h1>Main Page Title</h1>        <!-- Only one per page -->
<h2>Major Section</h2>          <!-- Multiple allowed -->
<h3>Subsection</h3>             
<h4>Sub-subsection</h4>
<h5>Minor heading</h5>
<h6>Smallest heading</h6>
```

### Paragraphs & Text Emphasis
```html
<p>This is a paragraph of text. It can contain 
   <strong>important content</strong> and 
   <em>emphasized text</em>.</p>

<p>Line breaks happen automatically, but you can force one<br>
   with the br tag if needed.</p>

<blockquote>
    "This is a quote from someone important."
</blockquote>
```

### Text Formatting Tags
```html
<strong>Bold/Important</strong>      <!-- Semantic importance -->
<b>Bold styling only</b>             <!-- Visual only -->
<em>Italicized/Emphasized</em>       <!-- Semantic emphasis -->
<i>Italic styling only</i>           <!-- Visual only -->
<mark>Highlighted text</mark>        <!-- Like highlighter -->
<small>Fine print</small>            <!-- Smaller text -->
<del>Deleted text</del>              <!-- Strikethrough -->
<ins>Inserted text</ins>             <!-- Underlined -->
```

---

## 📋 Lists

### Unordered Lists (Bullet Points)
```html
<ul>
    <li>First item</li>
    <li>Second item</li>
    <li>Third item with <strong>emphasis</strong></li>
</ul>
```

### Ordered Lists (Numbered)
```html
<ol>
    <li>Step one</li>
    <li>Step two</li>
    <li>Step three</li>
</ol>

<!-- Custom starting number -->
<ol start="5">
    <li>This will be number 5</li>
    <li>This will be number 6</li>
</ol>
```

### Nested Lists
```html
<ul>
    <li>Main item
        <ul>
            <li>Sub-item one</li>
            <li>Sub-item two</li>
        </ul>
    </li>
    <li>Another main item</li>
</ul>
```

### Description Lists
```html
<dl>
    <dt>HTML</dt>
    <dd>HyperText Markup Language</dd>
    <dt>CSS</dt>
    <dd>Cascading Style Sheets</dd>
</dl>
```

---

## 🔗 Links & Navigation

### Basic Links
```html
<!-- External link -->
<a href="https://example.com" target="_blank" rel="noopener">
    Visit Example.com
</a>

<!-- Internal link -->
<a href="about.html">About Us</a>

<!-- Link to section on same page -->
<a href="#contact">Go to Contact Section</a>

<!-- Email link -->
<a href="mailto:hello@example.com">Send Email</a>

<!-- Phone link -->
<a href="tel:+1234567890">Call Us</a>
```

### Link Best Practices
- Always include `rel="noopener"` for external links with `target="_blank"`
- Use descriptive link text (avoid "click here")
- Include `title` attribute for additional context

---

## 🖼️ Images & Media

### Images
```html
<!-- Basic image -->
<img src="images/photo.jpg" alt="Description of image">

<!-- Responsive image with multiple sizes -->
<img src="images/photo.jpg" 
     alt="Description of image"
     width="300" 
     height="200"
     loading="lazy">

<!-- Image as link -->
<a href="full-size.jpg">
    <img src="thumbnail.jpg" alt="Click to see full size">
</a>
```

### Figure with Caption
```html
<figure>
    <img src="chart.png" alt="Sales data for Q4">
    <figcaption>Q4 Sales Performance Chart</figcaption>
</figure>
```

---

## 📋 Forms & User Input

### Complete Contact Form Example
```html
<form action="/submit-contact" method="POST">
    <!-- Text inputs -->
    <div>
        <label for="fullname">Full Name *</label>
        <input type="text" id="fullname" name="fullname" required>
    </div>
    
    <!-- Email input -->
    <div>
        <label for="email">Email Address *</label>
        <input type="email" id="email" name="email" required>
    </div>
    
    <!-- Phone input -->
    <div>
        <label for="phone">Phone Number</label>
        <input type="tel" id="phone" name="phone">
    </div>
    
    <!-- Select dropdown -->
    <div>
        <label for="subject">Subject</label>
        <select id="subject" name="subject" required>
            <option value="">Choose a topic...</option>
            <option value="general">General Inquiry</option>
            <option value="support">Technical Support</option>
            <option value="sales">Sales Question</option>
        </select>
    </div>
    
    <!-- Radio buttons -->
    <fieldset>
        <legend>Preferred Contact Method</legend>
        <input type="radio" id="contact-email" name="contact-method" value="email" checked>
        <label for="contact-email">Email</label>
        
        <input type="radio" id="contact-phone" name="contact-method" value="phone">
        <label for="contact-phone">Phone</label>
    </fieldset>
    
    <!-- Checkboxes -->
    <div>
        <input type="checkbox" id="newsletter" name="newsletter" value="yes">
        <label for="newsletter">Subscribe to newsletter</label>
    </div>
    
    <!-- Textarea -->
    <div>
        <label for="message">Message *</label>
        <textarea id="message" name="message" rows="5" cols="50" 
                  placeholder="Tell us how we can help..." required></textarea>
    </div>
    
    <!-- Submit button -->
    <button type="submit">Send Message</button>
    <button type="reset">Clear Form</button>
</form>
```

### Form Input Types
```html
<input type="text">        <!-- Plain text -->
<input type="email">       <!-- Email validation -->
<input type="password">    <!-- Hidden text -->
<input type="number">      <!-- Numeric input -->
<input type="tel">         <!-- Phone number -->
<input type="url">         <!-- Website URL -->
<input type="date">        <!-- Date picker -->
<input type="time">        <!-- Time picker -->
<input type="file">        <!-- File upload -->
<input type="hidden">      <!-- Hidden data -->
<input type="search">      <!-- Search box -->
```

---

## 🏗️ Semantic HTML Structure

### Modern Page Layout
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Semantic HTML Example</title>
</head>
<body>
    <!-- Site header -->
    <header>
        <h1>Website Name</h1>
        <nav>
            <ul>
                <li><a href="/">Home</a></li>
                <li><a href="/about">About</a></li>
                <li><a href="/contact">Contact</a></li>
            </ul>
        </nav>
    </header>
    
    <!-- Main content area -->
    <main>
        <!-- Individual article/blog post -->
        <article>
            <header>
                <h2>Article Title</h2>
                <p>Published on <time datetime="2024-01-15">January 15, 2024</time></p>
            </header>
            <p>Article content goes here...</p>
            <footer>
                <p>Tags: <a href="/tag/html">HTML</a>, <a href="/tag/tutorial">Tutorial</a></p>
            </footer>
        </article>
        
        <!-- Grouped content section -->
        <section>
            <h2>Related Articles</h2>
            <article>...</article>
            <article>...</article>
        </section>
    </main>
    
    <!-- Sidebar content -->
    <aside>
        <h3>About the Author</h3>
        <p>Bio information...</p>
        
        <h3>Recent Posts</h3>
        <ul>
            <li><a href="/post1">Post 1</a></li>
            <li><a href="/post2">Post 2</a></li>
        </ul>
    </aside>
    
    <!-- Site footer -->
    <footer>
        <p>&copy; 2024 Your Website. All rights reserved.</p>
        <address>
            Contact: <a href="mailto:info@example.com">info@example.com</a>
        </address>
    </footer>
</body>
</html>
```

### When to Use Each Semantic Tag
- `<header>`: Site/section headers, not just page top
- `<nav>`: Primary navigation menus
- `<main>`: Main content area (only one per page)
- `<article>`: Standalone content (blog posts, news articles)
- `<section>`: Grouped related content with a heading
- `<aside>`: Sidebar content, related info
- `<footer>`: Site/section footers, copyright info

---

## 📊 Tables

### Basic Table Structure
```html
<table>
    <caption>Student Grades</caption>
    <thead>
        <tr>
            <th>Name</th>
            <th>Math</th>
            <th>Science</th>
            <th>Average</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Alice</td>
            <td>95</td>
            <td>88</td>
            <td>91.5</td>
        </tr>
        <tr>
            <td>Bob</td>
            <td>78</td>
            <td>92</td>
            <td>85</td>
        </tr>
    </tbody>
    <tfoot>
        <tr>
            <td>Class Average</td>
            <td>86.5</td>
            <td>90</td>
            <td>88.25</td>
        </tr>
    </tfoot>
</table>
```

---

## 🎯 Common Attributes Reference

| Attribute    | Elements         | Purpose                          | Example                           |
|--------------|------------------|----------------------------------|-----------------------------------|
| `class`      | All              | CSS styling hook                 | `class="highlight"`               |
| `id`         | All              | Unique identifier                | `id="main-content"`               |
| `href`       | `<a>`, `<link>`  | Link destination                 | `href="page.html"`                |
| `src`        | `<img>`, `<script>` | Resource source                | `src="image.jpg"`                 |
| `alt`        | `<img>`          | Accessibility description        | `alt="Logo"`                      |
| `title`      | All              | Tooltip text                     | `title="Click for more info"`     |
| `type`       | `<input>`        | Input field type                | `type="email"`                    |
| `name`       | Form elements    | Form data identifier            | `name="username"`                 |
| `value`      | Form elements    | Default/current value           | `value="Submit"`                  |
| `required`   | Form elements    | Required field validation       | `required`                        |
| `placeholder`| `<input>`, `<textarea>` | Hint text                  | `placeholder="Enter email"`       |
| `target`     | `<a>`            | Link opening behavior           | `target="_blank"`                 |
| `rel`        | `<a>`, `<link>`  | Relationship description        | `rel="noopener"`                  |
| `loading`    | `<img>`          | Loading behavior                | `loading="lazy"`                  |

---

## ✅ HTML Best Practices

### Code Quality
1. **Always include `<!DOCTYPE html>`** - Ensures standards mode
2. **Use lowercase for all tags and attributes** - `<div class="main">` not `<DIV CLASS="main">`
3. **Quote all attribute values** - `class="container"` not `class=container`
4. **Close all tags properly** - Every opening tag needs a closing tag
5. **Use proper indentation** - 2 or 4 spaces consistently
6. **One `<h1>` per page** - Multiple `<h2>`-`<h6>` are fine

### Accessibility
1. **Always include `alt` text for images** - Screen readers need this
2. **Use proper form labels** - Associate every input with a label
3. **Maintain heading hierarchy** - Don't skip from `<h1>` to `<h3>`
4. **Use semantic HTML** - `<button>` instead of `<div onclick>`
5. **Ensure sufficient color contrast** - Text must be readable
6. **Make interactive elements keyboard accessible**

### SEO & Performance
1. **Write descriptive `<title>` tags** - Unique for each page
2. **Include meta descriptions** - `<meta name="description" content="...">`
3. **Use heading tags for structure** - Not just for styling
4. **Optimize images** - Compress and use appropriate formats
5. **Use lazy loading for images** - `loading="lazy"`
6. **Minimize HTTP requests** - Combine CSS/JS files when possible

### Modern HTML
1. **Use semantic elements** - `<main>`, `<article>`, `<section>`, etc.
2. **Avoid deprecated tags** - No `<center>`, `<font>`, `<marquee>`
3. **Use CSS for styling** - Keep presentation separate from content
4. **Make it responsive** - Include viewport meta tag
5. **Validate your HTML** - Use W3C validator regularly

---

## 🔍 Validation & Testing Checklist

### Before Publishing
- [ ] HTML validates without errors ([W3C Validator](https://validator.w3.org/))
- [ ] All images have meaningful `alt` text
- [ ] Form elements have associated labels
- [ ] Links open in new tabs have `rel="noopener"`
- [ ] Page has proper heading hierarchy (`h1` → `h2` → `h3`)
- [ ] No deprecated HTML tags used
- [ ] Semantic elements used appropriately
- [ ] Meta tags included (`charset`, `viewport`, `description`)
- [ ] Page title is descriptive and unique
- [ ] All links work correctly
- [ ] Forms submit properly
- [ ] Page is readable without CSS

### Accessibility Check
- [ ] Can navigate with keyboard only
- [ ] Screen reader compatible
- [ ] Images convey their purpose through alt text
- [ ] Color is not the only way to convey information
- [ ] Text has sufficient contrast ratio
- [ ] Interactive elements are clearly identifiable

---

## 🛠️ Useful Tools & Resources

### Validation & Testing
- [W3C HTML Validator](https://validator.w3.org/) - Check HTML syntax
- [WAVE Web Accessibility Evaluator](https://wave.webaim.org/) - Accessibility testing
- [HTML5 Outliner](https://gsnedders.html5.org/outliner/) - Document structure
- Browser Developer Tools - Built-in testing

### References
- [MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/HTML) - Comprehensive HTML reference  
- [HTML5 Specification](https://html.spec.whatwg.org/) - Official standard
- [Can I Use](https://caniuse.com/) - Browser compatibility checker

### Code Editors
- VS Code with HTML extensions
- Sublime Text
- Atom
- WebStorm/PhpStorm

---

## 💡 Pro Tips

### Productivity Shortcuts
- Use **Emmet abbreviations**: Type `ul>li*3` and press Tab to create a 3-item list
- **Live reload**: Use tools like Live Server to see changes instantly
- **Code snippets**: Create templates for common HTML structures
- **Auto-formatting**: Set up your editor to format HTML automatically

### Common Mistakes to Avoid
1. **Forgetting to close tags** - Use an editor that highlights this
2. **Using `<br>` for spacing** - Use CSS margins instead
3. **Nesting block elements incorrectly** - `<p>` can't contain `<div>`
4. **Missing alt attributes** - Screen readers need these
5. **Using tables for layout** - Tables are for tabular data only
6. **Inline styles** - Keep CSS separate from HTML

---

*📖 Remember: Good HTML is semantic, accessible, and maintainable. Focus on meaning over appearance - let CSS handle the styling!*