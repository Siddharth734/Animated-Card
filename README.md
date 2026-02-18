# Animated Card Component

A small but significant piece of something bigger.

Built with HTML & SCSS. No JavaScript. No dependencies.

---

## Stack

- HTML
- SCSS (compiled to CSS)
- Custom font: `Tapestry-Regular.ttf`

## Structure

```
card-component/
├── index.html
├── style.scss
├── style.css
└── Tapestry-Regular.ttf
```

## How it works

A `.box` card sits centered on a dark background. The conic gradient border is always present but the animation is **paused by default** — on hover it resumes, the border becomes visible (`border-width: 0.2rem`), text turns orange, and a glow appears.

The spinning border uses `@property --rotate` (a Houdini CSS property) to make the angle animatable inside a `conic-gradient`.

```html
<div class="box">
  <img src="your-image.png" alt="">
  <h1>Title</h1>
  <p>Description</p>
</div>
```

## Customization

Tweak directly in `style.scss`:

```scss
// Animation speed
animation: rotator 5s infinite linear;

// Accent color
rgb(233, 134, 21)

// Card max width
max-width: 20rem;

// Border thickness on hover
border-width: 0.2rem;
```

---

MIT License