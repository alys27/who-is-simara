# Personal Portfolio Website (Jekyll)

A personal portfolio website prepared for the SITE 1101 – Principles of Information Systems course.

**✨This website was built using Jekyll (for a 10% bonus)**

## 📋 Description

This website was developed using the Jekyll static site generator, along with HTML, CSS, and JavaScript. The site features a responsive design, ensuring proper display and usability on mobile, tablet, and desktop devices.

## 🚀 Features

- ✅ Home Page (profile photo and introduction text)
- ✅ About Page (background, qualifications, activities)
- ✅ Projects Page (Project 1 and other projects)
- ✅ Contact Page
- ✅ Navigation bar and Footer
- ✅ GitHub and Codecademy icon links
- ✅ Responsive design (mobile and tablet support)
- ✅ Clean and modular code structure
- ✅ Jekyll static site generator (10% bonus)

## 📁 Structure

```
alys27.github.io/
├── _config.yml          # Jekyll configuration
├── _layouts/
│   └── default.html     # Main layout
├── _includes/
│   ├── header.html      # Navigation bar
│   └── footer.html      # Footer
├── index.html           # Home page
├── about.html           # About page
├── projects.html        # Projects page
├── contact.html         # Contact page
├── css/
│   └── style.css        # Main CSS file
├── js/
│   └── main.js          # JavaScript file
├── images/              # Images folder
│   ├── profile.jpg      # Profile image
│   ├── project1.jpg     # Project 1 image
│   ├── project2.jpg     # Project 2 image
│   └── project3.jpg     # Project 3 image
├── Gemfile              # Ruby dependencies
└── README.md            # This file

```

## 🔧 Installation

### For Local Development

1. Install Ruby və Bundler:
   - Windows: [RubyInstaller](https://rubyinstaller.org/)
   - macOS: `brew install ruby`
   - Linux: `sudo apt-get install ruby-full`

2. Clone the Repository:
```bash
git clone https://github.com/alys27/alys27.github.io.git
cd alys27.github.io
```

3. Install Dependencies:
```bash
bundle install
```

4. Start the Jekyll server:
```bash
bundle exec jekyll serve
```

5. Open in your browser: `http://localhost:4000`

### Hosting on GitHub Pages

GitHub Pages automatically builds Jekyll sites. Simply:

1. Push the repository to GitHub
2. Go to Settings > Pages and select Jekyll
3. Your website will be alive!

## 📝 Configuration

To use the website, update the information in the `_config.yml` file:

```yaml
author: "Simara Aliyeva"
email: "your.email@example.com"
github_username: "alys27"
codecademy_username: "alyss27"
repository: "site1101-portfolio"
```

## 🌐 GitHub Pages

To host the website on GitHub Pages:

1. Go to your GitHub repository
2. Navigate to Settings > Pages
3. Under Source, select Deploy from a branch
4. Choose branch: `main` and folder `/ (root)`
5. Click Save
6. GitHub Pages will automatically build the site using Jekyll
7. After a few minutes, your website will be available at `https://alys27.github.io`

## 📄 License

This project was created for educational purposes.

## 👤 Author

Simara Aliyeva - SITE 1101 CS Student

## 🔗 Links

- [GitHub Profile](https://github.com/alys27)
- [Codecademy Profile](https://www.codecademy.com/profiles/alyss27)
- [Website Repository](https://github.com/alys27/alys27.github.io)

## 🎯 Advantages of Jekyll

- ✅ Modular code structure (layouts and includes)
- ✅ Automatic site generation
- ✅ Native GitHub Pages support
- ✅ Markdown support
- ✅ Liquid template engine
- ✅ Plugin system