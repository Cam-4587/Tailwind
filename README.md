# Tailwind CSS Learning Playground

A comprehensive workspace to learn and experiment with Tailwind CSS concepts.

## Features

This playground includes interactive examples of:

- **Layout**: Flexbox, Grid, Spacing (padding & margin)
- **UI Components**: Buttons, Cards, Badges, Form Elements
- **Effects**: Shadows, Transitions, Scale, Gradients, Opacity, Transforms
- **Typography**: Headings, Font Sizes, Font Weights, Letter Spacing

## Quick Start (CDN)
The `index.html` file uses Tailwind CSS via CDN, so you can open it directly in a browser without any build setup.

Simply open `index.html` in your browser to see all the examples.

### Local Development (Build)

If you want to use the custom configuration and build process:

1. Install dependencies:
```bash
npm install
```

2. Run the development server with watch mode:
```bash
npm run dev
```

3. Build for production:
```bash
npm run build
```

## File Structure

```
.
├── index.html              # Main playground with all examples
├── tailwind.config.js      # Tailwind configuration with custom theme
├── package.json            # Project dependencies
├── src/
│   ├── input.css          # Custom CSS with component layers
│   └── output.css         # Generated CSS (when built)
└── README.md              # This file
```

## Key Tailwind Concepts Demonstrated

### Utility Classes
- Color utilities: `text-gray-600`, `bg-indigo-500`
- Spacing: `p-6`, `m-4`, `space-x-4`, `gap-6`
- Display: `flex`, `grid`, `block`, `hidden`
- Sizing: `w-full`, `h-16`, `max-w-7xl`

### Responsive Design
- Breakpoints: `md:`, `lg:` prefixes for responsive classes
- Example: `grid-cols-1 md:grid-cols-2 lg:grid-cols-3`

### State Variants
- Hover: `hover:bg-indigo-700`
- Focus: `focus:ring-2 focus:ring-indigo-500`
- Transitions: `transition duration-300`

### Component Patterns
- Reusable component classes in `src/input.css` using `@layer components`
- Examples: `.btn-primary`, `.card`, `.badge`

## Tailwind CSS Resources

- [Official Documentation](https://tailwindcss.com/docs)
- [Component Examples](https://tailwindcss.com/components)
- [Interactive Color Picker](https://tailwindcss.com/docs/customizing-colors)
- [Plugin System](https://tailwindcss.com/docs/plugins)

## Customization

Edit `tailwind.config.js` to:
- Add custom colors, spacing, and other values
- Extend the default theme
- Configure plugins
- Set up custom animations and keyframes

Edit `src/input.css` to:
- Add custom component classes
- Define utilities
- Import external fonts and styles

## Tips for Learning

1. **Inspect Elements**: Use your browser's developer tools to inspect elements and see which Tailwind classes are applied
2. **Use the Playground**: Modify the classes in `index.html` to see how changes affect the layout
3. **Read the Docs**: Reference the official Tailwind documentation when learning new utilities
4. **Experiment**: Try combining different classes to create unique designs
5. **Mobile First**: Always consider responsive design by starting with mobile classes and adding breakpoints

---

Happy learning with Tailwind CSS! 🎨

## FAQ about the uptime script

**Why have you added this script?**

It will help us to calculate how many running workspaces there are at any one time, which greatly helps us with cost and capacity planning. It will help us decide on the future direction of our cloud-based IDE strategy.

**How will this affect me?**

For everyday usage of Gitpod, it doesn’t have any effect at all. The script only captures the following data:

- An ID that is randomly generated each time the workspace is started.
- The current date and time
- The workspace status of “started” or “running”, which is sent every 5 minutes.

It is not possible for us or anyone else to trace the random ID back to an individual, and no personal data is being captured. It will not slow down the workspace or affect your work.

**So….?**

We want to tell you this so that we are being completely transparent about the data we collect and what we do with it.

**Can I opt out?**

Yes, you can. Since no personally identifiable information is being captured, we'd appreciate it if you let the script run; however if you are unhappy with the idea, simply run the following commands from the terminal window after creating the workspace, and this will remove the uptime script:

```
pkill uptime.sh
rm .vscode/uptime.sh
```

**Anything more?**

Yes! We'd strongly encourage you to look at the source code of the `uptime.sh` file so that you know what it's doing. As future software developers, it will be great practice to see how these shell scripts work.

---

Happy coding!
