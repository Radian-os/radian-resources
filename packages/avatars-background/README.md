# UI Avatars Backgrounds

<p align="center">
  <strong>High-quality, pre-optimized backgrounds for your UI avatars.</strong>
</p>

This package contains **58 diverse, high-quality backgrounds** tailored for developers and UI/UX designers to combine with transparent UI avatars. It includes solid colors (CLR), gradients (Grad), and image-based (IMG) backgrounds.

---

## 🚀 CDN Usage (Zero Install)

You do not need to install this package to use the backgrounds. You can hotlink them directly in your app via the jsDelivr global CDN using the following URL structure:

```text
https://cdn.jsdelivr.net/gh/Radian-os/radian-resources@main/packages/avatars-background/src/{filename}
```

*Replace `{filename}` with one of the available background filenames (e.g., `CLR-Amber.png`, `Grad-Blue.png`, `IMG-Cyan.png`).*

---

## 🛠️ Code Example (Next.js)

To display these backgrounds efficiently in a React/Next.js environment, use the Next.js `<Image />` component:

```tsx
import Image from 'next/image';

export default function RadianAvatarBackground() {
  return (
    <Image 
      src="https://cdn.jsdelivr.net/gh/Radian-os/radian-resources@main/packages/avatars-background/src/Grad-Blue.png"
      alt="Radian UI Avatar Background"
      width={48}
      height={48}
      className="rounded-full object-cover"
    />
  );
}
```

### Next.js Image Optimization Configuration
To permit Next.js to fetch and optimize these images from the CDN, add the following configuration to your `next.config.js` or `next.config.mjs`:

```javascript
/** @type {import('next').NextConfig} */
const nextConfig = {
  images: {
    remotePatterns: [
      {
        protocol: 'https',
        hostname: 'cdn.jsdelivr.net',
        port: '',
        pathname: '/gh/Radian-os/radian-resources/**',
      },
    ],
  },
};

module.exports = nextConfig;
```
