# 📚 How to Deploy with GitHub Pages

GitHub Pages is a free hosting service that lets you publish websites directly from your GitHub repository. Perfect for showcasing your projects, portfolios, and assignments.

---

## 🎯 **What is GitHub Pages?**

GitHub Pages automatically builds and serves your website from your repository. It's:
- **Free** - No cost for public repositories
- **Easy** - Just push your code and it's live
- **Fast** - Global CDN for quick loading
- **Custom domains** - Use your own domain name
- **HTTPS** - Secure by default

---

## 🚀 **Quick Start Guide**

### **Step 1: Prepare Your Repository**
1. **Create a new repository** or use an existing one
2. **Add your website files** (HTML, CSS, JS, images)
3. **Commit and push** your files to GitHub

### **Step 2: Enable GitHub Pages**
1. Go to your repository on GitHub

![Main Repository Page](./assets/how-to-github-pages/01-main-repository-page-on-github.png)

2. Click **Settings** tab

3. Scroll down to **Pages** section

![Pages Section in Settings](./assets/how-to-github-pages/03-pages-section-in-settings-sidebar.png)

4. Under **Source**, select **Deploy from a branch**
5. Choose **main** branch and **/ (root)** folder

![Source Dropdown and Branch Selection](./assets/how-to-github-pages/04-source-dropdown-with-deploy-from-branch-selected-and-main-branch-root-folder.png)

6. Click **Save**

### **Step 3: Use your GitHub Pages website under the Settings of the Edit Repo details**
- Your site will be available at: `https://{username}.github.io/{repository-name}`
- It may take a few minutes to deploy initially

- While you are waiting, Designate your Pages site as your official website for your repo.

1. Go back to the "Code" tab on the main repo site, and click the Gear Icon to the right.

![Settings Tab Highlighted](./assets/how-to-github-pages/02-settings-tab-highlighted-in-repository-sidebar.png)

2. 

![Pages Section in Settings](./assets/how-to-github-pages/03-pages-section-in-settings-sidebar.png)
![Confirm Sidebar Selection Complete](./assets/how-to-github-pages/07-confirm-sidebar-selection-complete-and-page-ready-on-checkmark.png)

---

## 📁 **Repository Structure**

### **For Simple Websites:**
```
your-repo/
├── index.html          # Main page
├── style.css           # Styles
├── script.js           # JavaScript
├── images/             # Image folder
│   └── logo.png
└── README.md           # Project documentation
```

### **For Project Subfolders:**
```
your-repo/
├── project1/
│   ├── index.html
│   └── style.css
├── project2/
│   ├── index.html
│   └── script.js
└── README.md
```

---

## ⚙️ **Optional: Custom 404 Page**

Create a `404.html` file in your repository root for a custom error page:
```html
<!DOCTYPE html>
<html>
<head>
    <title>Page Not Found</title>
</head>
<body>
    <h1>404 - Page Not Found</h1>
    <p>Sorry, the page you're looking for doesn't exist.</p>
    <a href="/">Go Home</a>
</body>
</html>
```

---

## 🛠️ **Common Use Cases**

### **Portfolio Website**
- Showcase your projects
- Include contact information
- Add resume/CV
- Link to GitHub repositories

### **Project Documentation**
- API documentation
- User guides
- Technical specifications
- Tutorials and examples

### **Assignment Submissions**
- Live demos of your work
- Interactive projects
- Code examples with explanations
- Visual presentations

### **Blog or Personal Site**
- Write about your learning journey
- Share coding tips and tricks
- Document your projects
- Connect with the developer community

---

## 📝 **Best Practices**

### **File Organization**
- Use descriptive file names
- Keep images optimized (compress before uploading)
- Organize CSS and JS in separate files
- Use semantic HTML structure

### **Performance**
- Optimize images (use WebP format when possible)
- Minify CSS and JavaScript for production
- Use relative paths for internal links
- Test your site on different devices

### **SEO and Accessibility**
- Include proper meta tags
- Use semantic HTML elements
- Add alt text to images
- Ensure good color contrast
- Test with screen readers

### **Security**
- Never commit sensitive information (API keys, passwords)
- Use HTTPS (enabled by default)
- Validate user inputs if using forms
- Keep dependencies updated

---

## 🔧 **Troubleshooting**

### **Site Not Loading**
- Check if Pages is enabled in repository settings
- Verify your `index.html` file exists
- Wait a few minutes for deployment
- Check the Actions tab for build errors

📸 *Screenshot Placeholder - Show the GitHub Actions tab with build status*

### **Styling Issues**
- Use relative paths for CSS and images
- Check browser console for 404 errors
- Ensure CSS files are properly linked
- Test locally before deploying

📸 *Screenshot Placeholder - Show browser DevTools console with 404 errors*

### **Custom Domain Problems**
- Verify DNS settings with your provider
- Check CNAME file is in repository root
- Wait up to 24 hours for DNS propagation
- Ensure domain is properly configured

---

## 📚 **Advanced Features (Optional)**

### **Jekyll Integration**
GitHub Pages supports Jekyll for static site generation:
1. Create `_config.yml` file
2. Use Jekyll templates and layouts
3. Write content in Markdown
4. Automatic build and deployment

📸 *Screenshot Placeholder - Show Jekyll site structure with _config.yml and _posts folder*

---

## 🎨 **Example Projects**

### **Simple Portfolio**
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>John Developer</h1>
        <nav>
            <a href="#about">About</a>
            <a href="#projects">Projects</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>
    <main>
        <section id="about">
            <h2>About Me</h2>
            <p>I'm a passionate web developer...</p>
        </section>
        <section id="projects">
            <h2>My Projects</h2>
            <div class="project-grid">
                <!-- Project cards here -->
            </div>
        </section>
    </main>
</body>
</html>
```

📸 *Screenshot Placeholder - Show the portfolio website rendered in a browser*

### **Project Showcase**
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chatbot Project</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>
    <div class="container">
        <h1>AI Chatbot Project</h1>
        <p>Built with HTML, CSS, JavaScript, and Hugging Face API</p>
        <div class="row">
            <div class="col-md-6">
                <h3>Features</h3>
                <ul>
                    <li>Real-time AI responses</li>
                    <li>Bootstrap styling</li>
                    <li>Input validation</li>
                </ul>
            </div>
            <div class="col-md-6">
                <h3>Technologies</h3>
                <ul>
                    <li>HTML5</li>
                    <li>CSS3</li>
                    <li>JavaScript</li>
                    <li>Bootstrap</li>
                </ul>
            </div>
        </div>
    </div>
</body>
</html>
```

📸 *Screenshot Placeholder - Show the Bootstrap-styled project showcase page*

---

## 🔗 **Useful Resources**

### **Documentation**
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [GitHub Actions for Pages](https://github.com/peaceiris/actions-gh-pages)

### **Tools**
- [GitHub Pages Generator](https://pages.github.com/)
- [Jekyll Themes](http://jekyllthemes.org/)
- [GitHub Pages Checker](https://github.com/igrigorik/github-pages-gem)

### **Tutorials**
- [GitHub Pages Tutorial](https://guides.github.com/features/pages/)
- [Custom Domain Setup](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)
- [Jekyll Quick Start](https://jekyllrb.com/docs/)

---

## 💡 **Pro Tips**

1. **Use relative paths** for all internal links
2. **Test locally** before pushing to GitHub
3. **Keep your repository organized** with clear file structure
4. **Use meaningful commit messages** for better project history
5. **Add a README.md** to explain your project

---

## 🎯 **Quick Checklist**

Before deploying your site:
- [ ] All files are committed and pushed to GitHub
- [ ] `index.html` exists in the root directory
- [ ] All images and assets use relative paths
- [ ] No sensitive information (API keys, passwords) in code
- [ ] Site works locally in a browser
- [ ] GitHub Pages is enabled in repository settings

---

*Happy deploying! 🚀*
