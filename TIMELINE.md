# 🗓️ 12-Week Development Curriculum Timeline

## 🌟 Weekly Breakdown

### Week 1-2: Web Foundations
**Lesson 1: HTML Essentials**
- **Key Concepts**:
  - Document structure (`<!DOCTYPE>`, `<html>`, `<head>`, `<body>`)
  - Semantic tags (`<header>`, `<article>`, `<section>`)
  - Forms and validation (`<input>`, `<textarea>`, `required` attribute)
- **Assignment**: Personal portfolio page with:
  - 3 sections (About, Projects, Contact)
  - Functional contact form
- **Prep for Next**: Experiment with inline CSS styles

**Lesson 2: CSS Mastery**
- **Key Concepts**:
  - CSS specificity hierarchy
  - Flexbox layouts (flex-direction, justify-content)
  - CSS variables and custom properties
- **Assignment**: Style portfolio page with:
  - Consistent color scheme using CSS variables
  - Responsive navigation bar
- **Prep for Next**: Add `onclick` handlers to navigation buttons

---

### Week 3-4: Core Programming Concepts
**Lesson 3: JavaScript Basics**
- **Key Concepts**:
  - DOM manipulation (`querySelector`, `addEventListener`)
  - Basic data types and type coercion
  - JSON format and storage
- **Assignment**:
  ```javascript
  // Add interactive features to portfolio:
  document.getElementById('theme-toggle').addEventListener('click', () => {
    document.body.classList.toggle('dark-mode');
  });
  ```
- **Prep for Next**: Explore `fetch()` API with sample endpoints

**Lesson 4: Modern JavaScript**
- **Key Concepts**:
  - ES6+ features (arrow functions, destructuring)
  - Async/await patterns
  - Local storage API
- **Assignment**: Build a:
  - Weather widget using OpenWeather API
  - Persistent theme selector using localStorage
- **Prep for Next**: Install TypeScript compiler (`tsc --init`)

---

### Week 5-6: Frontend Specialization
**Lesson 5: Responsive Design**
- **Key Concepts**:
  - Media query breakpoints
  - CSS Grid template areas
  - Mobile-first vs desktop-first approaches
- **Assignment**: Convert portfolio to:
  - 3-column desktop layout
  - Single-column mobile layout
- **Prep for Next**: Create basic `.ts` file with type annotations

**Lesson 6: TypeScript Transition**
- **Key Concepts**:
  - Type inference vs explicit typing
  - TS config options (`strict`, `noImplicitAny`)
  - Interface declarations
- **Assignment**:
  ```typescript
  interface Project {
    title: string;
    description: string;
    url: URL;
  }
  // Convert portfolio data to TypeScript objects
  ```
- **Prep for Next**: Explore Express.js routing documentation

---

### Week 7-8: Node.js Backend
**Lesson 7: Server Fundamentals**
- **Key Concepts**:
  - Node module system
  - REST API principles
  - Express middleware
- **Assignment**:
  ```javascript
  // Basic Express server
  const express = require('express');
  const app = express();
  app.get('/api/projects', (req, res) => {
    res.json(portfolioProjects);
  });
  ```
- **Prep for Next**: Set up MongoDB Atlas account

**Lesson 8: Database Integration**
- **Key Concepts**:
  - Schema design
  - Mongoose ODM
  - CRUD operations
- **Assignment**: Connect portfolio to:
  - MongoDB database for projects
  - Contact form submissions collection
- **Prep for Next**: Python syntax comparison exercises

---

### Week 9-10: Python Backend
**Lesson 9: Python Basics**
- **Key Concepts**:
  - Virtual environments (`venv`)
  - PEP8 guidelines
  - List comprehensions
- **Assignment**: Port weather widget to:
  - Python CLI version
  - File-based data storage
- **Prep for Next**: Explore Flask quickstart guide

**Lesson 10: Python Web Frameworks**
- **Key Concepts**:
  - Flask vs Django comparison
  - WSGI servers
  - ORM basics
- **Assignment**: Build Python version of:
  - Portfolio API endpoint
  - Database connection layer
- **Prep for Next**: Research JWT authentication

---

### Week 11-12: Full-Stack Integration
**Lesson 11: Authentication**
- **Key Concepts**:
  - JWT token flow
  - Password hashing (bcrypt)
  - Protected routes
- **Assignment**: Add to portfolio:
  - User registration/login
  - Admin project management panel
- **Prep for Next**: Explore deployment platforms

**Lesson 12: Deployment**
- **Key Concepts**:
  - Containerization basics
  - CI/CD pipelines
  - Monitoring and logging
- **Assignment**: Deploy full-stack app to:
  - Vercel (frontend)
  - Heroku (backend)
  - MongoDB Atlas (database)
  
---

## 🏁 Final Milestones
- **Week 6**: First full-stack prototype (HTML/CSS + Node)
- **Week 9**: Python-backed alternative implementation
- **Week 12**: Production-ready deployed application

[➡️ Proceed to Assignments](https://github.com/wanjuifavour/Beginner-Web-Crash-Course.git/assignments) | 
[❓ Get Help](https://github.com/wanjuifavour/Beginner-Web-Crash-Course.git/discussions)

> **Note**: This timeline assumes 4-6 hours of weekly practice outside lessons. Adjust pace as needed!