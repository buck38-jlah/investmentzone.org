# Investment Zone Website

A modern, professional investment-focused website built with React, TypeScript, and Tailwind CSS. Perfect for investment firms, financial advisors, and wealth management companies.

## 🌟 Features

- **Modern Design**: Clean, professional aesthetic with dark theme and blue/cyan accents
- **Responsive Layout**: Fully responsive design that works on all devices
- **Smooth Animations**: GSAP-powered scroll animations and hover effects
- **Interactive Components**: Service cards, testimonial carousel, and more
- **Fast Performance**: Optimized build with Vite
- **SEO Ready**: Proper meta tags and semantic HTML structure

## 📁 Project Structure

```
├── public/              # Static assets (images)
├── src/
│   ├── sections/        # Website sections/components
│   │   ├── Navigation.tsx
│   │   ├── Hero.tsx
│   │   ├── About.tsx
│   │   ├── Services.tsx
│   │   ├── WhyChoose.tsx
│   │   ├── Testimonials.tsx
│   │   ├── Blog.tsx
│   │   ├── CTA.tsx
│   │   └── Footer.tsx
│   ├── App.tsx          # Main application component
│   ├── index.css        # Global styles
│   └── main.tsx         # Entry point
├── dist/                # Production build output
└── README.md
```

## 🚀 Getting Started

### Prerequisites

- Node.js 18+ and npm/yarn
- Git

### Installation

1. **Clone or download this repository**
   ```bash
   git clone <your-repo-url>
   cd investment-zone-website
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   npm run dev
   ```
   The website will be available at `http://localhost:5173`

4. **Build for production**
   ```bash
   npm run build
   ```
   The built files will be in the `dist/` directory.

## 📋 GitHub Pages Deployment

### Method 1: Deploy from GitHub.com (Recommended for beginners)

1. **Create a new repository on GitHub**
   - Go to [github.com/new](https://github.com/new)
   - Name your repository (e.g., `investment-zone-website`)
   - Make it public
   - Don't initialize with README (you already have one)

2. **Upload your files**
   - After creating the repo, click "uploading an existing file"
   - Upload the contents of your project folder (not the folder itself)
   - Commit the files

3. **Enable GitHub Pages**
   - Go to Settings → Pages in your repository
   - Source: Deploy from a branch
   - Branch: main
   - Folder: / (root)
   - Click Save

4. **Wait for deployment**
   - GitHub will build and deploy your site
   - Check the Pages section for your live URL
   - It should look like: `https://yourusername.github.io/investment-zone-website/`

### Method 2: Using Git Command Line

1. **Initialize git and commit**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   ```

2. **Create repository and push**
   ```bash
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
   git branch -M main
   git push -u origin main
   ```

3. **Enable GitHub Pages** (follow steps 3-4 from Method 1)

### Method 3: Deploy dist folder (for custom domains)

1. **Build the project**
   ```bash
   npm run build
   ```

2. **Create a new branch for deployment**
   ```bash
   git add dist -f
   git commit -m "Add dist folder"
   git subtree push --prefix dist origin gh-pages
   ```

3. **Enable GitHub Pages**
   - Go to Settings → Pages
   - Source: Deploy from a branch
   - Branch: gh-pages
   - Folder: / (root)

## 🌐 Custom Domain Setup (investmentzone.org)

1. **Add CNAME file**
   - Create a file named `CNAME` in the `public` folder
   - Add your domain: `investmentzone.org`
   - Rebuild: `npm run build`

2. **Configure DNS**
   - Go to your domain registrar's DNS settings
   - Add these A records pointing to GitHub's servers:
     ```
     185.199.108.153
     185.199.109.153
     185.199.110.153
     185.199.111.153
     ```
   - Or add a CNAME record: `www` → `yourusername.github.io.`

3. **Enable HTTPS**
   - In GitHub Pages settings, check "Enforce HTTPS"

4. **Wait for DNS propagation** (up to 48 hours)

## 🎨 Customization

### Colors
Edit `src/index.css` to customize the color scheme:

```css
:root {
  --primary-blue: #0036ff;
  --dark-bg: #000e22;
  --darker-blue: #001429;
  --light-blue: #0055ff;
  --accent-cyan: #00cfff;
  --accent-purple: #6932ff;
}
```

### Content
Each section is a separate component in `src/sections/`. Update:
- Text content and headings
- Images (replace files in `public/` folder)
- Stats and testimonials
- Links and contact information

### Images
Replace images in the `public/` folder with your own:
- `hero-image.jpg` - Main hero section image
- `about-image.jpg` - About section image
- `service-1.jpg` to `service-4.jpg` - Service cards
- `testimonial-1.jpg` to `testimonial-4.jpg` - Client testimonials
- `blog-1.jpg` to `blog-3.jpg` - Blog post images
- `cta-bg.jpg` - Call-to-action background
- `why-choose.jpg` - Why choose us section image

**Recommended image sizes:**
- Hero: 1920x1080px (16:9 ratio)
- About: 800x1000px (4:5 ratio)
- Services: 800x600px (4:3 ratio)
- Testimonials: 200x200px (1:1 ratio)
- Blog: 800x600px (4:3 ratio)
- CTA Background: 1920x1080px (16:9 ratio)

## 🔧 Technologies Used

- **React 18** - UI Library
- **TypeScript** - Type safety
- **Vite** - Build tool
- **Tailwind CSS** - Utility-first CSS framework
- **GSAP** - Animation library
- **Lucide React** - Icon library
- **shadcn/ui** - UI components

## 📱 Responsive Breakpoints

- Mobile: < 768px
- Tablet: 768px - 1024px
- Desktop: > 1024px
- Large Desktop: > 1280px

## 🎯 Sections Included

1. **Navigation** - Sticky header with smooth scroll
2. **Hero** - Main banner with stats and CTA
3. **About** - Company overview with floating stats
4. **Services** - Interactive service cards with hover effects
5. **Why Choose Us** - Split-screen layout with feature highlights
6. **Testimonials** - 3D card carousel
7. **Blog** - Latest insights grid
8. **CTA** - Call-to-action with parallax background
9. **Footer** - Complete footer with links and newsletter

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Support

If you have any questions or need help with deployment:
- Check the [GitHub Pages documentation](https://docs.github.com/en/pages)
- Open an issue in your repository
- Contact your web developer

---

**Built with ❤️ for Investment Zone**
