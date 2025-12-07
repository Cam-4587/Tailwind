# Tailwind CSS Setup

This project is set up with Tailwind CSS v4 for rapid UI development.

## Packages Installed

The following packages have been installed to enable Tailwind CSS:

- **tailwindcss** (^4.1.17) - The core Tailwind CSS framework
- **@tailwindcss/postcss** (latest) - PostCSS plugin for Tailwind CSS v4
- **postcss** (^8.5.6) - CSS transformation tool
- **autoprefixer** (^10.4.22) - Adds vendor prefixes automatically
- **postcss-cli** (latest) - Command-line interface for PostCSS

## Project Structure

- `input.css` - Source CSS file with Tailwind directives
- `output.css` - Generated CSS file (excluded from git)
- `postcss.config.js` - PostCSS configuration
- `index.html` - Example HTML file demonstrating Tailwind CSS classes

## Usage

### Building CSS

To build your CSS file once:

```bash
npm run build:css
```

### Watch Mode

To automatically rebuild CSS when `input.css` changes:

```bash
npm run watch:css
```

### Using Tailwind in Your HTML

1. Link to the generated `output.css` file in your HTML:

```html
<link rel="stylesheet" href="output.css">
```

2. Use Tailwind utility classes in your HTML:

```html
<div class="bg-blue-500 text-white p-4 rounded">
  Hello Tailwind!
</div>
```

## Customization

### Adding Custom Styles

You can add custom CSS to `input.css`:

```css
@import "tailwindcss";

/* Your custom styles here */
.my-custom-class {
  /* custom styles */
}
```

## Development Server

To view your HTML file with live reload, you can use:

```bash
python3 -m http.server
```

Then open your browser to the provided URL.

## Learn More

- [Tailwind CSS Documentation](https://tailwindcss.com/docs)
- [Tailwind CSS v4 Documentation](https://tailwindcss.com/docs/v4)
