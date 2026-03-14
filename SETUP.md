# HTML Symbols & Entities - Local Setup

## Quick Start

### Prerequisites
- Node.js 14+ installed on your machine
- npm or yarn package manager

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/ais95/HTML-Symbols-Entities.git
   cd HTML-Symbols-Entities
   ```

2. **Install dependencies (optional - no external deps required):**
   ```bash
   npm install
   ```

3. **Start the development server:**
   ```bash
   npm run dev
   ```

4. **Open in browser:**
   - Navigate to `http://localhost:3000`
   - The app will automatically reload when files change

## Features

- **Dynamic Search** - Search HTML entities by name, Unicode, hex, or HTML code
- **Copy to Clipboard** - Click any code snippet to copy it instantly
- **80+ Entities** - Covers currency, math symbols, arrows, and special characters
- **Responsive Design** - Works on desktop, tablet, and mobile
- **No Build Step** - Runs directly with Node.js, no build tools needed

## Development

The project structure is simple:
```
├── index.html      # Main application (Vue 3 + app code)
├── style.css       # All styles
├── server.js       # Development server
├── package.json    # Project metadata
└── README.md       # Project info
```

### Hot Reload
Just edit `index.html` or `style.css` and refresh your browser. The server serves files directly without any build process.

### Adding More Entities
Edit the `entities` array in `index.html` to add more HTML symbols. Each entity needs:
- `id` - Unique identifier
- `character` - The symbol itself
- `name` - Description
- `unicode` - Unicode format (e.g., U+000A9)
- `hex` - Hex HTML code (e.g., &#xa9;)
- `decimal` - Decimal HTML code (e.g., &#169;)
- `htmlEntity` - Named entity (e.g., &copy;)

## Troubleshooting

**Port already in use?**
```bash
PORT=3001 npm run dev
```

**Permission denied error?**
```bash
chmod +x server.js
npm run dev
```

**Module not found?**
Make sure Node.js is installed:
```bash
node --version
npm --version
```
