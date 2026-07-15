# Brand Logos

<p align="center">
  <strong>Scalable, modern SVG brand logos and social icons for integration lists and UI controls.</strong>
</p>

This package contains high-quality, lightweight brand and product logo SVGs for standard web integrations, authentication providers (Google, GitHub, Apple, etc.), and tech stacks.

---

## 🚀 CDN Usage (Zero Install)

You do not need to install this package. You can hotlink and embed the SVGs directly into your applications using the jsDelivr global CDN:

```text
https://cdn.jsdelivr.net/gh/Radian-os/radian-resources@main/packages/brand-logos/src/{logo-name}.svg
```

*Replace `{logo-name}` with the brand filename (e.g., `radian.svg`, `github.svg`, `google.svg`).*

---

## 🛠️ Code Example (React / Next.js)

To display these SVG brand logos directly in your web applications, you can use standard image tags or remote HTML loading:

```tsx
import Image from 'next/image';

export default function BrandLogo() {
  return (
    <Image 
      src="https://cdn.jsdelivr.net/gh/Radian-os/radian-resources@main/packages/brand-logos/src/radian.svg"
      alt="Radian Logo"
      width={32}
      height={32}
      className="h-8 w-8"
    />
  );
}
```

### HTML Example
```html
<img src="https://cdn.jsdelivr.net/gh/Radian-os/radian-resources@main/packages/brand-logos/src/radian.svg" alt="Radian Logo" width="32" height="32" />
```

