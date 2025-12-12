# Personal Portfolio Website

A clean, responsive personal portfolio website built with React, Tailwind CSS, and TypeScript.

## Features

- **Hero Section**: Name, title, and professional tagline with social links
- **About Section**: Professional summary and profile
- **Experience Timeline**: Interactive timeline with companies, roles, dates, and achievements
- **Project Cards**: Showcasing key projects with technologies and metrics
- **Skills Section**: Categorized skill badges with certifications
- **Education Section**: Academic background
- **Contact Form**: Functional form for visitor inquiries
- **Dark Mode**: Toggle between light and dark themes (persisted in localStorage)
- **Fully Responsive**: Mobile-first design that works on all devices

## Tech Stack

- **Frontend**: React, TypeScript, Tailwind CSS
- **UI Components**: shadcn/ui
- **Backend**: Express.js
- **Form Validation**: Zod + React Hook Form
- **Icons**: Lucide React, React Icons

## Project Structure

```
├── client/
│   ├── src/
│   │   ├── components/       # React components
│   │   │   ├── Navigation.tsx
│   │   │   ├── Hero.tsx
│   │   │   ├── About.tsx
│   │   │   ├── Experience.tsx
│   │   │   ├── Projects.tsx
│   │   │   ├── Skills.tsx
│   │   │   ├── Education.tsx
│   │   │   ├── Contact.tsx
│   │   │   └── Footer.tsx
│   │   ├── lib/
│   │   │   ├── portfolio-data.ts   # <-- UPDATE YOUR CONTENT HERE
│   │   │   └── theme-provider.tsx
│   │   ├── App.tsx
│   │   └── index.css
│   └── index.html
├── server/
│   └── routes.ts             # Contact form API
└── README.md
```

## How to Update Your Content

### 1. Personal Information & All Sections

Edit `client/src/lib/portfolio-data.ts`:

```typescript
export const portfolioData = {
  personal: {
    name: "Your Name",
    title: "Your Title",
    tagline: "Your professional tagline",
    email: "your@email.com",
    phone: "+1 234 567 890",
    location: "Your City, Country",
    linkedin: "https://linkedin.com/in/yourprofile",
    github: "https://github.com/yourusername",
  },
  
  about: { ... },
  experience: [ ... ],
  projects: [ ... ],
  skills: { ... },
  education: [ ... ],
  certifications: [ ... ],
};
```

### 2. Adding a Profile Photo

Replace the placeholder in `About.tsx` with an actual image:

```tsx
<img 
  src="/your-photo.jpg" 
  alt="Your Name" 
  className="w-48 h-48 md:w-64 md:h-64 rounded-2xl object-cover"
/>
```

### 3. Customize Colors

Edit `client/src/index.css` to change the accent color (currently a professional blue):

```css
--primary: 217 91% 35%;  /* Hue Saturation% Lightness% */
```

### 4. SEO & Meta Tags

Update `client/index.html` with your own meta information:

```html
<meta name="description" content="Your description" />
<title>Your Name | Portfolio</title>
```

## Development

```bash
# Install dependencies
npm install

# Start development server
npm run dev
```

The app runs on `http://localhost:5000`

## Deployment

This project is ready to deploy on Replit:

1. Click the "Deploy" button in Replit
2. Your portfolio will be live at `your-repl-name.replit.app`

For custom domains, configure in Replit's deployment settings.

## Contact Form

Messages submitted through the contact form are:
1. Validated using Zod schema
2. Stored in memory (for basic use)
3. Logged to the console

For production, consider:
- Adding email notifications (e.g., Resend, SendGrid)
- Storing messages in a database
- Adding spam protection (reCAPTCHA)

## License

MIT License - feel free to use this template for your own portfolio!
