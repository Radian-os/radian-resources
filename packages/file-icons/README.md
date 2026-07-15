# File Icons

<p align="center">
  <strong>Consistent, elegant SVG file-type icons for file list views, upload areas, and documents.</strong>
</p>

This package hosts a set of modern and minimalist SVG file type icons (such as PDF, ZIP, code files, documents, and spreadsheets). These are perfect for displaying in file upload status indicators, attachment lists, and document repositories.

---

## 🚀 CDN Usage (Zero Install)

You do not need to install this package. Hotlink the SVG icons directly via the jsDelivr global CDN using the file extension or file class name:

```text
https://cdn.jsdelivr.net/gh/Radian-os/radian-resources@main/packages/file-icons/src/{icon-name}.svg
```

*Replace `{icon-name}` with the filename matching the extension (e.g., `pdf.svg`, `zip.svg`, `image.svg`, `code.svg`).*

---

## 🛠️ Code Example (React / Next.js)

To display a file-type icon inside an attachment list:

```tsx
import Image from 'next/image';

interface AttachmentProps {
  fileName: string;
  fileExtension: string; // e.g., 'pdf', 'zip'
}

export default function FileAttachment({ fileName, fileExtension }: AttachmentProps) {
  return (
    <div className="flex items-center gap-3 p-3 border rounded-lg">
      <Image 
        src={`https://cdn.jsdelivr.net/gh/Radian-os/radian-resources@main/packages/file-icons/src/${fileExtension.toLowerCase()}.svg`}
        alt={`${fileExtension} icon`}
        width={32}
        height={32}
        className="h-8 w-8"
      />
      <span className="text-sm font-medium">{fileName}</span>
    </div>
  );
}
```

### HTML Example
```html
<img src="https://cdn.jsdelivr.net/gh/Radian-os/radian-resources@main/packages/file-icons/src/pdf.svg" alt="PDF File" width="32" height="32" />
```

