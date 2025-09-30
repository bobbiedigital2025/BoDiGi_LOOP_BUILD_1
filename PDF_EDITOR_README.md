# BoDiGi PDF Editor

A professional, browser-based PDF editor designed for small businesses. Edit, annotate, and enhance your PDF documents without any server-side processing - everything runs securely in your browser.

## Features

### 📄 PDF Viewing
- High-quality PDF rendering using PDF.js
- Multi-page navigation
- Responsive design for all screen sizes
- Clean and intuitive interface

### ✏️ Text Annotation
- Add custom text anywhere on your PDF
- Adjustable font size (8-72px)
- Customizable text color
- Click-to-place text functionality

### 🎨 Shape Drawing
- Draw rectangles with click and drag
- Customizable border colors
- Adjustable fill colors
- Variable border width

### 💾 Export & Save
- Save edited PDFs with all modifications
- Export to standard PDF format
- All annotations preserved in final document

## Quick Start

### Method 1: Direct Browser Access
1. Open `pdf-editor.html` in any modern web browser
2. Click "Open PDF" to load your PDF file
3. Use the toolbar to add annotations
4. Click "Save PDF" to download your edited document

### Method 2: Local Web Server
```bash
# Using Python 3
python3 -m http.server 8000

# Using Node.js
npx http-server

# Then open http://localhost:8000/pdf-editor.html
```

## How to Use

### Opening a PDF
1. Click the **"Open PDF"** button in the toolbar
2. Select a PDF file from your computer
3. The PDF will load and display in the editor

### Adding Text
1. Click the **"Add Text"** button in the toolbar
2. Configure text properties in the sidebar:
   - Enter your text content
   - Set font size
   - Choose text color
3. Click anywhere on the PDF to place your text
4. Repeat to add multiple text elements

### Drawing Rectangles
1. Click the **"Add Rectangle"** button in the toolbar
2. Configure shape properties in the sidebar:
   - Choose border color
   - Select fill color
   - Set border width
3. Click and drag on the PDF to draw a rectangle
4. Release to finalize the shape

### Navigating Pages
- Use **Previous** and **Next** buttons below the canvas
- Page counter shows current page and total pages

### Saving Your Work
1. Click the **"Save PDF"** button in the toolbar
2. Your edited PDF will download automatically as `edited-document.pdf`
3. All annotations are permanently saved in the PDF

### Clearing Annotations
- Click **"Clear All"** to remove all annotations from the current page
- A confirmation dialog will appear before clearing

## Technical Details

### Technologies Used
- **PDF.js** (v3.11.174) - Mozilla's PDF rendering library
- **pdf-lib** (v1.17.1) - PDF creation and modification library
- **HTML5 Canvas** - For rendering and interactive drawing
- **Vanilla JavaScript** - No framework dependencies

### Browser Compatibility
- ✅ Chrome 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Edge 90+

### Security & Privacy
- **100% Client-Side Processing** - No data is sent to any server
- **Local File Handling** - Files never leave your computer
- **No Account Required** - Use immediately without sign-up
- **No Data Collection** - Complete privacy guaranteed

## Customization

### Changing Default Colors
Edit the HTML file and modify these default values:
```javascript
// Text color (line ~XXX)
<input type="color" id="text-color" value="#000000">

// Border color
<input type="color" id="border-color" value="#667eea">

// Fill color
<input type="color" id="fill-color" value="#ffffff">
```

### Adjusting Scale/Zoom
Modify the scale variable in the JavaScript section:
```javascript
let scale = 1.5; // Change to 1.0 for smaller, 2.0 for larger
```

### Customizing Styles
The CSS is embedded in the `<style>` section. Modify colors, fonts, and layouts as needed:
```css
/* Example: Change primary color */
.btn-primary {
    background: #667eea; /* Change this hex color */
}
```

## Use Cases

### For Small Businesses
- Add business stamps or seals to documents
- Fill in forms that aren't editable
- Add notes and comments to contracts
- Highlight important sections with colored boxes

### For Professionals
- Review and annotate client documents
- Add signatures or initials
- Create custom forms
- Add explanatory notes to presentations

### For Students
- Annotate study materials
- Add notes to research papers
- Highlight important passages
- Create custom worksheets

## Troubleshooting

### PDF Won't Load
- Ensure the file is a valid PDF
- Try a different browser
- Check if the file is password-protected (not supported)
- Verify the file isn't corrupted

### Annotations Don't Save
- Make sure you click "Save PDF" after adding annotations
- Check browser console for JavaScript errors
- Ensure pop-ups aren't blocked in your browser

### Performance Issues
- Large PDFs may take time to load
- Close unnecessary browser tabs
- Try reducing the scale/zoom level
- Consider splitting very large PDFs

### Canvas Not Responding
- Refresh the page and reload the PDF
- Check if JavaScript is enabled
- Try a different browser
- Ensure you've clicked a mode button (Add Text/Add Rectangle)

## Future Enhancements

Potential features for future versions:
- [ ] Drawing tools (lines, circles, arrows)
- [ ] Image insertion
- [ ] Text highlighting
- [ ] Signature pad
- [ ] Undo/redo functionality
- [ ] Multiple page editing
- [ ] PDF merging
- [ ] Page rotation
- [ ] Zoom controls
- [ ] Dark mode

## License

This PDF editor is part of the BoDiGi_LOOP_BUILD_1 project and is provided as-is for small business use.

## Support

For issues, questions, or suggestions, please open an issue on the GitHub repository.

## Credits

Built with:
- PDF.js by Mozilla
- pdf-lib by Andrew Dillon
- Modern HTML5/CSS3/JavaScript

---

**BoDiGi PDF Editor** - Making PDF editing simple and accessible for everyone.
