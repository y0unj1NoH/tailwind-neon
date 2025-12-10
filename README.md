# ✨ Tailwind Neon

Beautiful neon glow utilities for **Tailwind CSS v4** —
Text Glow, Box Glow, Outline Glow, and Glow Animations.

Fully CSS-based. Zero-JS. Lightweight.

---

## 🚀 Installation

```sh
npm install tailwind-neon
```

---

## 🔧 Usage (Tailwind v4)

Simply import the stylesheet in your global CSS:

```css
@import "tailwind-neon";
```

Tailwind will automatically register all utilities through `@layer utilities`.

---

## ✨ What’s Included

| Category               | Utilities                                                   |
| ---------------------- | ----------------------------------------------------------- |
| **Text Glow**          | `text-glow-xs`, `text-glow-sm`, `text-glow`, `text-glow-lg` |
| **Box Glow**           | `glow-xs`, `glow-sm`, `glow`, `glow-lg`                     |
| **Outline Glow**       | `glow-outline`, `glow-outline-lg`                           |
| **Animations**         | `animate-glow-pulse`, `animate-glow-flicker`                |
| **Custom Glow Colors** | Supports CSS variables:<br>`--glow-color`, `--text-glow-color`, `--outline-glow-color` |

---

## 🔥 Text Glow

```html
<p class="text-glow text-cyan-400">Default Glow</p>
<p class="text-glow-sm text-pink-400">Small Glow</p>
<p class="text-glow-lg text-purple-400">Large Glow</p>
```

---

## 🔷 Box Glow

```html
<button class="px-4 py-2 rounded bg-cyan-400 text-white glow glow-cyan-400">
  Neon Button
</button>
```

Variants: `glow-xs`, `glow-sm`, `glow`, `glow-lg`

---

## 🟩 Outline Glow

```html
<button class="px-4 py-2 rounded glow-outline text-cyan-300">
  Outline Glow
</button>
```

---

## 🎨 Custom Glow Colors

Glow colors can be customized in multiple ways.
**Text Glow** defaults to using the element’s **text color (`currentColor`)**, so you can simply use Tailwind text utilities:

```html
<p class="text-glow text-green-400">Uses Tailwind's text-green-400 as the glow color</p>
```

For Box Glow and Outline Glow, or when you want independent control, use one of the following options:

---

### **Option 1: Inline override**

```html
<p class="text-glow" style="--text-glow-color: #39ff14;">
  Custom Green Text Glow
</p>
```

---

### **Option 2: Theme utility (Tailwind v4)**

```css
@theme {
  .neon-green {
    --glow-color: #39ff14;
  }
}
```

**Usage:**

```html
<button class="px-4 py-2 rounded bg-cyan-400 text-white glow glow-neon-green">
    glow
</button>
```
---

## ✨ Glow Animations

```html
<p class="text-glow animate-glow-pulse text-cyan-300">Pulse</p>
<p class="text-glow animate-glow-flicker text-cyan-400">Flicker</p>
```

---

## 📚 Demo

A full demo is included in this package and can be viewed locally:

```
demo/index.html
```

Open this file directly in your browser to preview all glow utilities, animations, and examples.

(Once GitHub Pages is enabled, an online demo will also be available.)

---

## 🧩 Features

* Beautiful neon glow utilities (xs/sm/default/lg)
* Text glow, box glow, outline glow
* Pulse & flicker animations
* Tailwind v4 native (`@layer utilities`)
* Zero-JS, lightweight


## 📄 License

MIT
