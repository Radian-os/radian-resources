# Country Flags

<p align="center">
  <strong>Beautiful, optimized SVG country flags for locale selectors, phone inputs, and dashboard tables.</strong>
</p>

This package provides a comprehensive collection of clean, pixel-perfect SVG world flags. Optimized for fast rendering, these flags are ideal for building multi-lingual UI selectors, checkout flows, and user profile information.

---

## 🚀 CDN Usage (Zero Install)

You do not need to install this package. Hotlink the SVG flags directly via the jsDelivr global CDN using the ISO 3166-1 alpha-2 country code:

```text
https://cdn.jsdelivr.net/gh/Radian-os/radian-resources@main/packages/country-flags/src/{country-code}.svg
```

*Replace `{country-code}` with the lowercase two-letter code of the country (e.g., `us.svg`, `gb.svg`, `ca.svg`, `jp.svg`).*

---

## 🛠️ Code Example (React / Next.js)

To display a flag alongside a country name or select input:

```tsx
import Image from 'next/image';

interface CountrySelectorProps {
  countryCode: string; // e.g., 'us', 'jp', 'de'
  countryName: string;
}

export default function CountryFlag({ countryCode, countryName }: CountrySelectorProps) {
  return (
    <div className="flex items-center gap-2">
      <Image 
        src={`https://cdn.jsdelivr.net/gh/Radian-os/radian-resources@main/packages/country-flags/src/${countryCode.toLowerCase()}.svg`}
        alt={`${countryName} flag`}
        width={24}
        height={16}
        className="rounded-sm object-cover"
      />
      <span>{countryName}</span>
    </div>
  );
}
```

### HTML Example
```html
<img src="https://cdn.jsdelivr.net/gh/Radian-os/radian-resources@main/packages/country-flags/src/us.svg" alt="United States" width="24" height="16" />
```

