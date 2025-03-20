# QR Code Label Generator for Paperless-ngx ASN

A web-based tool for generating printable QR code labels for Paperless-ngx ASN (Archival Serial Numbers). Based on the original implementation by Tobias Maier, this tool has been enhanced and improved to provide more precise control over layout and print quality. While originally designed for ASN labels, it can now be used to create QR code labels of various sizes for any purpose, supporting multiple page formats and orientations.

## Features

- Generation of QR codes for ASN numbers with customizable prefixes
- Precise control over page margins and label spacing
- Target/Actual value comparison for exact print adjustments
- Multiple page format support (A4, A5, US Letter, Legal)
- Portrait and landscape orientation
- Configurable text formatting (font family, size, weight)
- Visual page preview with margin indicators
- Save and load configurations
- Print-optimized output
- Responsive design
- No installation required - runs in browser
- Flexible label sizing for various applications

## Technical Details

- Default label size: 25.35mm × 10mm (customizable)
- QR code size: 9mm × 9mm
- Supported page formats:
  - A4 (210mm × 297mm)
  - A5 (148mm × 210mm)
  - US Letter (215.9mm × 279.4mm)
  - US Legal (215.9mm × 355.6mm)
- Default labels per page: 7 × 27 = 189 labels (adjustable based on format)
- Default page margins:
  - Top: 13.14mm
  - Bottom: 13.7mm
  - Left: 8.4mm
  - Right: 8.5mm

## Understanding Target and Actual Values and Scaling

The generator uses a sophisticated target and actual value system to ensure precise label printing:

### Target Values
- These are your desired measurements, which can come from:
  - Manufacturer specifications for your label sheets
  - Your own requirements for custom labels
  - Standard label dimensions
- Example: If your label sheet specifies 25.4mm × 10mm labels, these are your target values

### Actual Values
- These are the real measurements from your test prints
- How to determine:
  1. Use target values for initial test print
  2. Measure the actual printed dimensions with a precise ruler
  3. Enter these measurements as actual values
  4. The generator will automatically calculate scaling factors

### Automatic Scaling
The system automatically calculates scaling factors to compensate for printer variations:
- Horizontal scaling: Adjusts for width differences
- Vertical scaling: Adjusts for height differences
- These calculations ensure that your labels will print at the correct size

### Example Workflow
1. Initial Setup:
   - Enter target values from your label sheet specifications
   - Set actual values equal to target values initially
   - Make a test print

2. Measurement and Adjustment:
   - Measure the printed labels carefully
   - Enter the measured dimensions as actual values
   - The system will calculate scaling factors
   - Make another test print to verify

3. Fine-tuning:
   - If needed, adjust actual values further
   - Each printer may need slightly different values
   - Save your configuration once perfect

### Tips for Accurate Measurements
- Use a high-quality ruler or caliper
- Measure multiple labels and take the average
- Consider both width and height
- Check spacing between labels
- Verify margins on all sides

## Usage

1. Open `index.html` in your web browser

2. Select page format and orientation:
   - Choose between A4, A5, US Letter, or Legal format
   - Select portrait or landscape orientation
   - Page dimensions are automatically updated

3. Configure QR code settings:
   - Start number: First ASN number
   - ASN prefix: Prefix for your ASN numbers (e.g., "ASN")
   - Leading zeros: Number of digits for numbering
   - Display prefix: Show/hide prefix in label
   - Show borders: Show/hide label borders

4. Adjust page margins:
   - Target and actual values adjustable for all margins
   - Visual warnings for overlaps
   - Automatic scaling calculation

5. Set label dimensions:
   - Width and height of labels (customizable for different label types)
   - Horizontal and vertical spacing
   - Real-time preview of changes
   - Automatic calculation of labels per page

6. Configure text formatting:
   - Font family (default: Arial)
   - Font size (default: 11pt)
   - Font weight
   - QR code spacing

7. Save/Load configuration:
   - Click "Save Configuration" to export
   - Use "Load Configuration" to import
   - "Reset to Default" for standard settings

8. Preview and print:
   - "Update Labels" to refresh preview
   - "Print Labels" for print-optimized output

## Label Customization Examples

The generator can be adapted for various label types:

- Small inventory labels (e.g., 20mm × 10mm)
- Large shipping labels (e.g., 50mm × 30mm)
- Square labels for product tracking
- Custom-sized labels for specific applications

Simply adjust the label dimensions and spacing to match your specific requirements.

## Troubleshooting

- Detailed calculation information displayed for margin overlaps
- Scaling factors help with precise adjustments
- Verify actual print dimensions with a ruler
- Adjust actual values accordingly
- Check page format settings if labels appear incorrectly sized

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
