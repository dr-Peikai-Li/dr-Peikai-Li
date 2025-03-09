# Dr. Peikai Li - Academic Website

This repository contains the source code for Dr. Peikai Li's academic website, showcasing research, publications, teaching, and professional activities in organizational psychology and leadership.

## Website Structure

The website consists of the following main pages:

- `index.html` - Homepage with profile, research overview, and featured publications
- `research.html` - Detailed information about research areas, projects, and methodologies
- `publications.html` - Complete list of publications with filters and links to full texts
- `teaching.html` - Teaching experience, courses, and workshops
- `cv.html` - Full academic curriculum vitae
- `contact.html` - Contact information and inquiry form

## Setting Up Your GitHub Pages Website

### 1. Fork or Clone This Repository

Start by forking this repository to your own GitHub account or clone it to create a new repository.

### 2. Repository Settings

- Rename your repository to `yourusername.github.io` (replace "yourusername" with your actual GitHub username)
- Go to the repository Settings → Pages
- Under "Source", select "main" branch
- Click "Save"

### 3. Customization

#### Profile Photo

1. Add your profile photo to the `assets/images/` directory
2. Update the image path in `index.html`:
   ```html
   <img src="assets/images/your-photo.jpg" alt="Your Name">
   ```

#### CV PDF

1. Add your CV PDF to the `assets/files/` directory
2. Update the link in `cv.html`:
   ```html
   <a href="assets/files/your-cv.pdf" class="btn btn-large" download>
   ```

#### Contact Information

Update your contact information in:
- `index.html` - Social media links
- `contact.html` - Email, phone, address, etc.

#### Content Updates

Each HTML file is well-structured with clear section divisions, making it easy to update specific content areas:

- Update personal information, education, experience in relevant sections
- Modify or add publications in the publications page
- Update research projects and interests on the research page
- Add or remove courses and workshops on the teaching page

### 4. Customizing Colors and Styles

The main color scheme and styles can be customized in the `assets/css/style.css` file:

```css
:root {
  --primary-color: #2c3e50;      /* Main text and header color */
  --secondary-color: #3498db;    /* Links and accents */
  --accent-color: #e74c3c;       /* Highlight color */
  --text-color: #333333;         /* Body text */
  --light-text: #666666;         /* Secondary text */
  --background-color: #ffffff;   /* Main background */
  --light-background: #f5f7fa;   /* Secondary background */
  --border-color: #e1e1e1;       /* Borders and dividers */
  --link-color: #2980b9;         /* Link text */
  --link-hover: #3498db;         /* Link hover color */
  --font-main: 'Source Sans Pro', Arial, sans-serif;  /* Main text font */
  --font-heading: 'Playfair Display', Georgia, serif; /* Heading font */
}
```

Change these values to adjust the color scheme throughout the site.

## File Structure

```
yourusername.github.io/
├── index.html               # Homepage
├── research.html            # Research page
├── publications.html        # Publications page
├── teaching.html            # Teaching page
├── cv.html                  # CV page
├── contact.html             # Contact page
├── assets/
│   ├── css/
│   │   └── style.css        # Main stylesheet
│   ├── js/
│   │   └── main.js          # JavaScript functionality
│   ├── images/
│   │   └── profile.jpg      # Profile photo
│   └── files/
│       └── CV-Peikai-Li.pdf # Downloadable CV
└── README.md                # This file
```

## Adding Google Analytics (Optional)

To add Google Analytics tracking to your site, add the following code just before the closing `</head>` tag in each HTML file:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=YOUR-GA-ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'YOUR-GA-ID');
</script>
```

Replace `YOUR-GA-ID` with your actual Google Analytics tracking ID.

## Adding a Custom Domain (Optional)

1. Purchase a domain name from a domain registrar
2. In your GitHub repository, go to Settings → Pages
3. Under "Custom domain", enter your domain name and click "Save"
4. Set up DNS records with your domain registrar:
   - Type: A, Name: @, Value: 185.199.108.153
   - Type: A, Name: @, Value: 185.199.109.153
   - Type: A, Name: @, Value: 185.199.110.153
   - Type: A, Name: @, Value: 185.199.111.153
   - Type: CNAME, Name: www, Value: yourusername.github.io

## Maintenance

- Regularly update your publications, projects, and news
- Keep your CV current
- Check for broken links periodically
- Update your profile photo when needed

## Support

If you encounter any issues with the template, please open an issue on GitHub or contact the original developer.

## License

This template is available for personal and academic use. Please keep the attribution to the original creator in the footer.
