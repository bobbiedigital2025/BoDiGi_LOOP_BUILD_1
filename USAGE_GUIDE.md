# BoDiGi PDF Editor - Usage Guide

## Getting Started

### Step 1: Open the PDF Editor

Open `pdf-editor.html` in your web browser. You can do this by:

**Option A: Direct File Open**
- Navigate to the file in your file system
- Right-click and select "Open with" → your preferred browser
- Or double-click the file (if your system is configured to open HTML files in a browser)

**Option B: Local Web Server** (Recommended for best performance)
```bash
# Using Python 3
cd /path/to/BoDiGi_LOOP_BUILD_1
python3 -m http.server 8000

# Then open in browser: http://localhost:8000/pdf-editor.html
```

### Step 2: Load a PDF

1. Click the **"📁 Open PDF"** button in the toolbar
2. Select a PDF file from your computer
3. The PDF will load and display in the editor

**Note**: A sample test PDF (`test-sample.pdf`) is included in the repository for testing purposes.

### Step 3: Edit Your PDF

#### Adding Text
1. Click the **"✏️ Add Text"** button
2. In the sidebar, configure:
   - **Text Content**: Enter the text you want to add
   - **Font Size**: Choose size between 8-72px
   - **Text Color**: Pick any color
3. Click anywhere on the PDF to place your text
4. Repeat to add multiple text elements

#### Drawing Rectangles
1. Click the **"⬜ Add Rectangle"** button
2. In the sidebar, configure:
   - **Border Color**: Choose outline color
   - **Fill Color**: Choose fill color
   - **Border Width**: Set thickness (1-10px)
3. Click and drag on the PDF to draw a rectangle
4. Release to finalize the shape

### Step 4: Save Your Work

1. Click the **"💾 Save PDF"** button
2. Your edited PDF will download as `edited-document.pdf`
3. All your annotations are permanently saved in the PDF

## Tips & Best Practices

### Text Annotation Tips
- Use larger font sizes (18-24px) for headers and important notes
- Use darker colors for better readability
- Keep text concise and clear
- Test text placement before adding many annotations

### Shape Drawing Tips
- Use transparent fill colors (or white) for highlighting areas without covering content
- Use bright border colors (like red or yellow) to draw attention
- Adjust border width based on the size of your rectangle
- Draw slowly and precisely for better control

### Multi-Page Documents
- Use the **Previous** and **Next** buttons to navigate between pages
- Each page maintains its own annotations
- Clear annotations works per-page only

### Workflow Suggestions

**For Forms:**
1. Open the form PDF
2. Use text mode to fill in fields
3. Save the completed form

**For Reviews:**
1. Open the document to review
2. Use rectangles to highlight sections
3. Use text to add comments or notes
4. Save the annotated version

**For Signing:**
1. Open the document
2. Add text with your name/signature
3. Add date using text annotation
4. Save the signed document

## Common Use Cases

### Business Documents
- Fill out forms that aren't digitally editable
- Add company stamps or seals
- Sign contracts and agreements
- Add notes to proposals

### Educational Materials
- Annotate study guides
- Add explanations to diagrams
- Highlight important sections
- Create custom worksheets

### Personal Documents
- Fill out government forms
- Add notes to receipts
- Sign lease agreements
- Annotate manuals

## Keyboard Shortcuts

Currently, the editor uses mouse interactions. Keyboard shortcuts coming in future versions.

## Browser Compatibility

The PDF editor works best in modern browsers:
- ✅ **Chrome/Edge**: Full support, best performance
- ✅ **Firefox**: Full support
- ✅ **Safari**: Full support (macOS/iOS)
- ⚠️ **Internet Explorer**: Not supported

## Internet Requirements

**First Load**: Internet connection required to load PDF.js and pdf-lib libraries from CDN

**After Libraries Load**: Can work offline if libraries are cached

**For Offline Use**: Download PDF.js and pdf-lib libraries locally and update script tags in the HTML file

## Troubleshooting

### PDF Won't Load
**Problem**: File won't open
**Solutions**:
- Verify the file is a valid PDF (not corrupted)
- Check file isn't password-protected
- Try a different PDF file
- Check browser console for error messages

### Annotations Disappear
**Problem**: Added items don't show up
**Solutions**:
- Make sure you've clicked the mode button (Add Text/Add Rectangle)
- Check you're editing the correct page
- Try refreshing and reloading the PDF

### Can't Save PDF
**Problem**: Save button doesn't work
**Solutions**:
- Check if pop-ups are blocked
- Try a different browser
- Verify you have write permissions to download folder
- Check browser console for errors

### Performance Issues
**Problem**: Editor is slow or laggy
**Solutions**:
- Close unnecessary browser tabs
- Try a smaller PDF file
- Reduce the number of annotations
- Use a different browser

## Advanced Features (Coming Soon)

Future updates may include:
- Undo/Redo functionality
- Image insertion
- Line and arrow drawing
- Text highlighting
- Digital signatures
- PDF merging
- Page deletion/reordering
- Zoom controls

## Need Help?

If you encounter issues:
1. Check this guide first
2. Review the main [PDF_EDITOR_README.md](PDF_EDITOR_README.md)
3. Check browser console for error messages
4. Try the included test-sample.pdf to verify basic functionality
5. Open an issue on GitHub with details about your problem

## Example Workflow

Here's a complete example of editing a document:

1. **Open** pdf-editor.html in Chrome
2. **Click** "Open PDF" button
3. **Select** test-sample.pdf from the repository
4. **Click** "Add Text" button
5. **Type** "APPROVED" in the text content field
6. **Change** text color to green (#00ff00)
7. **Set** font size to 24
8. **Click** on the PDF where you want to place the text
9. **Click** "Add Rectangle" button
10. **Change** border color to red
11. **Draw** a rectangle around important content
12. **Click** "Save PDF" button
13. **Check** your downloads folder for edited-document.pdf

That's it! Your PDF is now edited and saved.
