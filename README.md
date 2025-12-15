# ASCII Art Generator

A modern web app that converts images into ASCII art with customizable settings and export options. Built with Next.js, TypeScript, and Tailwind CSS.

## Features

- 🖼️ **Image Upload** - Drag & drop, file picker, or URL input
- 🎨 **Live Preview** - Real-time ASCII art preview as you adjust settings
- 📏 **Flexible Settings**:
  - Output width (50-200 characters)
  - Multiple character sets (Dense, Medium, Sparse, Blocks, Simple)
  - Color modes (Grayscale or Colored)
  - Contrast and brightness controls
- 🔍 **Zoom Controls** - Adjustable font size for preview (4px-24px)
- 💾 **Export Options**:
  - TXT (plain text)
  - HTML (with styling)
  - SVG (vector format)
  - Copy to clipboard
- ⌨️ **Keyboard Shortcuts** - Ctrl+S to save
- 🌙 **Dark Mode** - Automatic dark mode support
- 📱 **Responsive Design** - Works on desktop and mobile

## Getting Started

### Prerequisites

- Node.js 18+ and npm/yarn/pnpm

### Installation

1. Clone or download this repository
2. Install dependencies:

```bash
npm install
# or
yarn install
# or
pnpm install
```

3. Run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
```

4. Open [http://localhost:3000](http://localhost:3000) in your browser

## Project Structure

```
ascii-art-generator/
├── app/
│   ├── layout.tsx          # Root layout with metadata
│   ├── page.tsx            # Main page with all components
│   └── globals.css         # Global styles + Tailwind
├── components/
│   ├── ImageUploader.tsx   # Image upload component
│   ├── AsciiPreview.tsx    # Live preview component
│   ├── Controls.tsx        # Settings panel
│   └── ExportButtons.tsx   # Export/download buttons
├── lib/
│   ├── asciiConverter.ts   # Core conversion algorithm
│   └── characterSets.ts   # Character set definitions
└── types/
    └── index.ts            # TypeScript type definitions
```

## Tech Stack

- **Next.js 14** - React framework with App Router
- **TypeScript** - Type safety
- **Tailwind CSS** - Utility-first CSS framework
- **Canvas API** - Image processing
- **File API** - Upload and download handling

## How to Use

1. **Upload an Image**: Drag & drop an image, click to select a file, or enter an image URL
2. **Adjust Settings**: Tweak the width, character set, color mode, contrast, and brightness
3. **Preview**: The ASCII art updates automatically as you change settings
4. **Export**: Download the result as TXT, HTML, or SVG, or copy to clipboard

## Character Sets

- **Dense**: `@%#*+=-:. ` - For high detail
- **Medium**: Full character set for balanced results (default)
- **Sparse**: `.:-=+*#%@` - For minimalist results
- **Blocks**: `█▓▒░ ` - Block/retro style
- **Simple**: `.# ` - Very simple

## Keyboard Shortcuts

- `Ctrl+S` / `Cmd+S` - Download as TXT

## Building for Production

```bash
npm run build
npm start
```

Production output is in the `.next/` folder.

## License

MIT License - feel free to use for personal or commercial projects.

## Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request.

---

Made with ❤️ using Next.js
