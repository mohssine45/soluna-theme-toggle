# Orbit Theme Toggle

A lightweight, dependency-free animated sun/moon theme toggle built with **HTML + CSS only**.

## Demo

Open [`demo/index.html`](./demo/index.html) locally, or publish the `demo` folder with GitHub Pages.

## Features

- Pure HTML + CSS
- No JavaScript
- No dependencies
- Lightweight and easy to customize
- Smooth sun/moon transition
- Orbiting dots animation
- Keyboard focus support
- `prefers-reduced-motion` support
- Customizable accent color
- Framework-agnostic

## Quick Start

Copy the HTML from [`src/orbit-theme-toggle.html`](./src/orbit-theme-toggle.html) and the CSS from [`src/orbit-theme-toggle.css`](./src/orbit-theme-toggle.css) into your project.

The toggle intentionally does **not** control your application's theme. It only provides the UI state. Your application can listen to the checkbox state and apply its own dark-mode logic.

## Customize

Change the accent color with the CSS custom property:

```css
.ts-toggle-wrapper {
  --ts-color: #6f2da8;
}
```

You can also change the size by adjusting `.ts-toggle`.

## NPM

The package exposes the stylesheet and HTML template:

```bash
npm install orbit-theme-toggle
```

Import the stylesheet:

```js
import "orbit-theme-toggle/style.css";
```

The HTML template is available at:

```text
orbit-theme-toggle/template.html
```

## Important: Theme Logic

Orbit Theme Toggle is intentionally presentation-only. It does not assume whether your application uses:

- `class="dark"`
- `data-theme="dark"`
- React state
- Vue state
- another theme system

This keeps the component reusable across different projects.

## Accessibility

The component uses a native checkbox for its state and supports keyboard focus. Users who prefer reduced motion receive a non-animated transition.

For production applications, keep the accessible label meaningful for the context in which the component is used.

## Browser Support

Uses standard HTML, SVG, CSS transitions, CSS custom properties, and `prefers-reduced-motion`.

## License

MIT © Mz Design
