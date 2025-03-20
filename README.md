# QR Code Label Generator for Paperless-ngx ASN

A web-based tool for generating printable QR code labels for Paperless-ngx ASN (Archival Serial Numbers). Based on the original implementation by Tobias Maier, this tool has been enhanced and improved to provide more precise control over layout and print quality.

## Features

- Generation of QR codes for ASN numbers with customizable prefixes
- Precise control over page margins and label spacing
- Target/Actual value comparison for exact print adjustments
- Configurable text formatting (font family, size, weight)
- Visual A4 page preview with margin indicators
- Save and load configurations
- Print-optimized output
- Responsive design
- No installation required - runs in browser

## Technical Details

- Label size: 25.35mm × 10mm
- QR code size: 9mm × 9mm
- Page format: A4 (210mm × 297mm)
- Labels per page: 7 × 27 = 189 labels
- Default page margins:
  - Top: 13.14mm
  - Bottom: 13.7mm
  - Left: 8.4mm
  - Right: 8.5mm

## Usage

1. Open `index.html` in your web browser

2. Configure QR code settings:
   - Start number: First ASN number
   - ASN prefix: Prefix for your ASN numbers (e.g., "ASN")
   - Leading zeros: Number of digits for numbering
   - Display prefix: Show/hide prefix in label
   - Show borders: Show/hide label borders

3. Adjust page margins:
   - Target and actual values adjustable for all margins
   - Visual warnings for overlaps
   - Automatic scaling calculation

4. Set label dimensions:
   - Width and height of labels
   - Horizontal and vertical spacing
   - Real-time preview of changes

5. Configure text formatting:
   - Font family (default: Arial)
   - Font size (default: 11pt)
   - Font weight
   - QR code spacing

6. Save/Load configuration:
   - Click "Save Configuration" to export
   - Use "Load Configuration" to import
   - "Reset to Default" for standard settings

7. Preview and print:
   - "Update Labels" to refresh preview
   - "Print Labels" for print-optimized output

## Troubleshooting

- Detailed calculation information displayed for margin overlaps
- Scaling factors help with precise adjustments
- Verify actual print dimensions with a ruler
- Adjust actual values accordingly

## Dependencies

- [Alpine.js](https://alpinejs.dev/) - For reactive functionality
- [Tailwind CSS](https://tailwindcss.com/) - For styling
- [QR Server API](https://goqr.me/api/) - For QR code generation

## License

MIT License - See LICENSE file for details

## Author

Enhanced version by Murat Güven
GitHub Repository: [muguu](https://github.com/muguu/ASN-QR-Code-label-generator)

Based on the original implementation by Tobias Maier
