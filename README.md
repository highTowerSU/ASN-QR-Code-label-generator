# QR Code Label Generator for Paperless-ngx ASN

A web-based tool to generate printable QR code labels for Paperless-ngx ASN (Archival Serial Numbers). This tool helps you create and print labels with QR codes that can be easily scanned and processed by Paperless-ngx.

## Features

- Generate QR codes for ASN numbers with customizable prefixes
- Configurable page margins for different printer setups
- Adjustable label spacing
- Visual preview of A4 page layout
- Print-ready output
- No installation required - runs in browser
- Mobile-responsive design

## Usage

1. Open `index.html` in your web browser
2. Configure your settings:
   - **QR Code Settings:**
     - Start Number: First ASN number to generate
     - ASN Prefix: Prefix for your ASN numbers (e.g., "ASN")
     - Display Prefix: Toggle prefix visibility
     - Show Label Borders: Toggle border visibility
   - **Page Margins:** Adjust margins in millimeters
   - **Label Spacing:** Set gaps between labels
3. Click "Update Labels" to preview
4. Click "Print Labels" to print

## Technical Details

- Label Size: 25.4mm × 10mm
- QR Code Size: 9mm × 9mm
- Page Format: A4 (210mm × 297mm)
- Labels per Page: 7 × 27 = 189 labels

## Dependencies

- [Alpine.js](https://alpinejs.dev/) - For reactive functionality
- [Tailwind CSS](https://tailwindcss.com/) - For styling
- [QR Server API](https://goqr.me/api/) - For QR code generation

## License

MIT License - See LICENSE file for details

## Author

Original implementation by Tobias Maier
GitHub Repository: [muguu](https://github.com/muguu/ASN-QR-Code-label-generator)
