# UW Research Lab Website

## Getting Started

### Running the Website Locally

1. **Install dependencies:**
   ```bash
   bundle install
   ```

2. **Start the development server:**
   ```bash
   bundle exec jekyll serve --livereload
   ```

3. **View the website:**
   - Open your browser and go to `http://localhost:4000`
   - The site will automatically reload when you make changes

### Managing the People Page

The people page features a modern, compact design with:
- **Circular profile images** (100px) with hover effects
- **Compact card layout** that fits more people per row
- **Thesis topic display** showing each person's research focus
- **Research interest tags** that highlight each person's work
- **Role badges** (Faculty, PhD, Masters) for quick identification
- **Responsive design** that works on all devices

#### Adding New People

1. **Add profile image** to `assets/img/people/` (use square images for best results)
2. **Update `_data/people.yml`** with the person's information:
   ```yaml
   - firstname: "John"
     lastname: "Doe"
     role: "phd"  # faculty, phd, masters, postdoc
     website: "https://johndoe.com"
     pic: "john-doe"  # filename without .jpg
     position: "PhD Student"
     thesis-topic: "Your research topic or thesis title here"
     keywords:
       - "Human-AI Collaboration"
       - "Data Visualization"
       - "Machine Learning"
   ```

3. **Thesis topics** will appear in italics below the person's name and position
4. **Keywords/tags** will automatically appear as colorful badges highlighting research interests

#### Design Features

- **Compact layout** - More people visible at once
- **Smaller images** - 100px circular photos (80px on mobile)
- **Reduced padding** - Cards take up less space
- **Thesis topics** - Clear display of research focus
- **Hover effects** on images and cards
- **Smooth animations** when the page loads
- **Gradient text** for the page title
- **Modern color scheme** with purple/blue gradients
- **Mobile responsive** design

### Stopping the Server

Press `Ctrl+C` in the terminal where the server is running.
