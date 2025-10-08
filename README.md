# JIIT Tools Suite Documentation

A modern, glassmorphic documentation website for the JIIT Tools Suite — a comprehensive collection of web applications and automation tools built for the JIIT student community.

## Overview

This project serves as the central hub and documentation site for all JIIT Tools Suite projects, providing easy access to tools like JPortal, Timetable, Mess Menu, Placement Updates, Sophos Auto-Login, and the Telegram Notification Bot. The site features a modern glassmorphic design with frosted-glass UI elements, backdrop blur effects, and gradient color accents.

## Features

- **Glassmorphic Design**: Modern frosted-glass aesthetic with backdrop blur and subtle transparency
- **Tool Showcase**: Comprehensive listing of all available JIIT tools with descriptions and quick links
- **Responsive Layout**: Mobile-first design that works seamlessly across all device sizes
- **Fast Performance**: Built with Astro for optimal loading speeds and minimal JavaScript
- **Dark Theme**: Eye-friendly dark color scheme with gradient accents

## Tech Stack

- **Astro 5.x**: Static site generator for fast, content-focused websites
- **Tailwind CSS 4.x**: Utility-first CSS framework for styling
- **TypeScript**: Type-safe development experience
- **Bun**: Fast JavaScript runtime and package manager

## Project Structure

```
/
├── public/
│   └── favicon.svg
├── src/
│   ├── assets/
│   │   ├── astro.svg
│   │   └── background.svg
│   ├── components/
│   │   └── Welcome.astro
│   ├── layouts/
│   │   └── Layout.astro          # Main layout with glassmorphic header/footer
│   ├── pages/
│   │   ├── index.astro            # Homepage with hero and tool grid
│   │   └── tools.astro            # Complete tools listing page
│   └── styles/
│       └── global.css             # Glassmorphism utilities and theme
├── astro.config.mjs
├── tailwind.config.js
├── tsconfig.json
└── package.json
```

## Getting Started

### Prerequisites

- Node.js 18+ or Bun 1.0+
- Git

### Installation

1. Clone the repository:

```sh
git clone https://github.com/tashifkhan/JIIT-tools-docs.git
cd JIIT-tools-docs
```

2. Install dependencies:

```sh
bun install
```

Or with npm:

```sh
npm install
```

### Development

Start the development server:

```sh
bun run dev
```

The site will be available at `http://localhost:4321`

### Building for Production

Build the static site:

```sh
bun run build
```

The output will be in the `dist/` directory, ready for deployment.

### Preview Production Build

Preview the production build locally:

```sh
bun run preview
```

## Design System

### Glassmorphism Utilities

The project includes custom CSS utilities in `src/styles/global.css`:

- **`.bg-surface`**: Main background with layered radial gradients
- **`.glass`**: Frosted glass effect with backdrop blur and subtle borders
- **`.glass-card`**: Pre-styled glass card with padding and rounded corners
- **`.badge-glass`**: Small glass badge for tags and labels
- **`.blur-blob`**: Large blurred color elements for depth

### Color Palette

- **Background**: Deep dark blue (`#0f1117`) with gradient overlays
- **Glass**: Semi-transparent white with backdrop blur
- **Accents**: Indigo, pink, and blue gradients
- **Text**: Light grays and whites for optimal contrast

## Featured Tools

The site showcases the following JIIT Tools Suite projects:

1. **JPortal**: React PWA for WebKiosk with Pyadlite PDF parsing (8k+ users)
2. **JIIT Timetable**: Real-time timetables for 6.5k+ students with dynamic display
3. **Mess Menu**: Daily and weekly meal information accessible via timetable portal
4. **Placement & Campus Updates**: Timely opportunities and campus news (4k+ users)
5. **Sophos Auto-Login**: One-click Wi-Fi login scripts for LRC and Hostels (100 users)
6. **Telegram Notification Bot**: Real-time broadcast updates and announcements

## Customization

### Modifying the Glass Effect

Edit the `.glass` utility in `src/styles/global.css`:

```css
.glass {
	background-color: rgba(255, 255, 255, 0.06);
	border: 1px solid rgba(255, 255, 255, 0.14);
	backdrop-filter: saturate(140%) blur(18px);
}
```

### Adding New Tools

Add new tools to the `tools` array in `src/pages/tools.astro`:

```typescript
const tools = [
	{
		name: "Tool Name",
		desc: "Tool description",
		href: "https://tool-url.com",
		tag: "Category",
	},
];
```

## Deployment

This Astro site can be deployed to any static hosting platform:

- **Vercel**: Connect your GitHub repository for automatic deployments
- **Netlify**: Drag and drop the `dist/` folder or connect via Git
- **GitHub Pages**: Use the Astro GitHub Pages action
- **Cloudflare Pages**: Direct Git integration with automatic builds

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

## License

This project is open source and available under the MIT License.

## Author

Built by [@tashifkhan](https://github.com/tashifkhan)

## Links

- **Live Site**: [JIIT Tools Suite](https://tools.tashif.codes) (if deployed)
- **GitHub Organization**: [@tashifkhan](https://github.com/tashifkhan)
- **Telegram Bot**: [@SupersetNotificationBot](https://t.me/SupersetNotificationBot)

## Acknowledgments

- JIIT student community for feedback and support
- Astro team for the excellent static site generator
- Tailwind CSS for the utility-first approach to styling
