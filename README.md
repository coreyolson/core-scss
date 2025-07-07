# core.scss

![Version](https://img.shields.io/github/v/tag/coreyolson/core-scss?label=version)
![License](https://img.shields.io/github/license/coreyolson/core-scss)
![Style](https://img.shields.io/badge/style-SCSS-blue)

**core.scss** is a minimal, reusable SCSS starter for consistent layout, spacing, and typography across projects. It provides the essentials. No colors, no branding, just a clean functional scss starter to build from.

---

## Features

- 📐 **Layout** – Flex-based grid with rows and responsive columns
- 📏 **Spacing** – Margin & padding helpers (`m0–m3`, `p0–p3`, `x`, `y`, etc.)
- 📝 **Typography** – Scalable heading sizes and text sizing utilities
- 🧲 **Utilities** – Visibility classes, truncate, wrap, width, z-index, etc.
- 🖨️ **Print Styles** – Clean print-friendly output
- 💡 **Unopinionated** – No themes or color schemes

---

## Example

```html
<div class="container">
  <div class="row">
    <div class="col-6 p1">
      <h1 class="text-xl">Title</h1>
    </div>
    <div class="col-6 p1 text-right">
      <p class="text-sm wrap">Responsive layout with spacing helpers.</p>
    </div>
  </div>
</div>
```

---

## Overview

| Category       | Classes                                                  |
|----------------|----------------------------------------------------------|
| **Spacing**    | `m0–m3`, `p0–p3`, `mx`, `my`, `px`, `py`                 |
| **Grid**       | `.container`, `.row`, `.col-1` to `.col-12`              |
| **Text Size**  | `text-xs`, `text-sm`, `text-lg`, `text-xl`               |
| **Text Weight**| `text-light`, `text-normal`, `text-bold`                 |
| **Text Flow**  | `wrap`, `nowrap`, `break`, `truncate`                    |
| **Text Color** | `.muted`                                                 |
| **Link**       | `.link-plain`                                            |
| **Alignment**  | `text-left`, `text-center`, `text-right`                 |
| **Flex**       | `flex`, `justify-*`, `items-center`                      |
| **Display**    | `block`, `inline`, `inline-block`, `hidden`              |
| **Lists**      | `.list-plain`                                            |
| **Visibility** | `hide-sm`, `show-md`, etc.                               |
| **Z-Index**    | `z-0`, `z-10`, `z-20`, `z-30`, `z-auto`                  |
| **Width**      | `w-25`, `w-50`, `w-75`, `w-100`                          |
| **Print**      | `.no-print`, `.print-only`                               |

---

## Installation

Install via NPM:

```bash
npm install core-scss
```

Then in your SCSS:

```scss
@use "core-scss/src/index" as *;
```

> Note: Sass does **not** yet resolve the package entry by `package.json`.  
> Be sure to include the full path (`/src/index`) and **omit** the underscore + extension.

If using the Sass CLI, include the node_modules path:

```bash
sass --load-path=node_modules src/scss/style.scss public/css/style.css
```

---

## License
This project is licensed under the MIT License.