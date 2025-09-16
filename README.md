# Constitution Maker

A simple, powerful tool for creating, editing, and generating constitutions in HTML and PDF formats. Based on the CEGSA (Computer Engineering Student Association) constitution structure.

## 🖼️ Screenshots

### Main Interface
<img width="1184" height="459" alt="Screenshot 2025-09-15 at 10 45 34 PM" src="https://github.com/user-attachments/assets/47846800-c8e4-4aa2-9a27-c21f5dcf8ee1" />

### Generated Constitution with Table of Contents
<img width="1000" height="663" alt="Screenshot 2025-09-15 at 10 48 06 PM" src="https://github.com/user-attachments/assets/501378ba-4c0a-4367-b531-0451964cdde6" />

## 📄 How to Save as PDF (Most Important!)

**This is the #1 feature you'll use:**

1. **Open** `constitution-generator.html` in your web browser
2. **Edit** your constitution content as needed
3. **Click "Export PDF"** button
4. **Print dialog opens** - Look for the **"Destination"** dropdown
5. **Change destination** from your printer to **"Save as PDF"**
6. **⚠️ IMPORTANT**: In the print dialog, **uncheck "Headers and footers"** to remove the file path
7. **Click "Save"** and choose where to save your PDF file
8. **Done!** You now have a professional PDF constitution

> 💡 **Tip**: The PDF will have perfect formatting with Roman numerals, bullet points, and proper legal document styling. Unchecking "Headers and footers" removes the file path but keeps all the content formatting.

## Features

- **PDF Generation**: High-quality PDF output using browser's built-in print-to-PDF
- **Web-based Interface**: Easy-to-use HTML interface for creating and editing constitutions
- **Real Constitution Template**: Pre-loaded with actual CEGSA constitution structure
- **Professional Formatting**: Proper legal document formatting with Roman numerals and bullet points
- **Multi-language Support**: Built-in support for English, Spanish, French, German, and Italian
- **JSON Export/Import**: Easy data portability and version control
- **Print-friendly**: Optimized for both screen and print viewing

## Quick Start

1. **Download** the files to your computer
2. **Open** `constitution-generator.html` in your web browser
3. **Start editing** your constitution immediately!

## Usage

### Basic Usage

1. **Open** `constitution-generator.html` in your browser
2. **Edit the constitution**:
   - Change the title, organization name, or adoption date
   - Modify any article or section text
   - Add new articles using the "Add Article" button
3. **Export your constitution**:
   - **HTML format** - For web viewing and sharing
   - **PDF format** - For printing and official use (via browser print)
   - **JSON format** - For backup and version control
4. **Import existing data** - Use "Import JSON" to load `constitution-cegsa.json` or other constitution files

### PDF Generation

**Already covered above** - This is the most important feature! See the "How to Save as PDF" section at the top of this README.

### Multi-language Support

- Select from supported languages in the dropdown
- All interface elements and document structure adapt to the selected language
- Easy to add new languages by extending the translation object

## Constitution Data Structure

```json
{
  "title": "Constitution of the Example Organization",
  "organization": "Example Organization",
  "adoptionDate": "2024-01-01",
  "language": "en",
  "preamble": "We, the members...",
  "articles": [
    {
      "number": 1,
      "title": "Article Title",
      "sections": [
        {
          "number": 1,
          "text": "Section text here."
        }
      ]
    }
  ],
  "amendments": [
    {
      "text": "Amendment text",
      "date": "2024-01-01"
    }
  ],
  "signatures": [
    {
      "name": "President",
      "title": "President"
    }
  ]
}
```

## Customization

### Adding New Languages

1. Edit the `translations` object in `constitution-generator.html`
2. Add your language code and translations:

```javascript
const translations = {
  // ... existing languages
  'your-lang': {
    preamble: "Your Translation",
    article: "Your Translation",
    section: "Your Translation",
    amendments: "Your Translation",
    signatures: "Your Translation",
    adopted: "Your Translation"
  }
};
```

### Custom Styling

- Modify the CSS in `constitution-generator.html` for both web and print styling
- Use print media queries for print-specific styling
- All styling is contained in the single HTML file

## File Structure

```
constitution-maker/
├── constitution-generator.html    # Main web interface (works offline)
├── constitution-cegsa.json       # Real CEGSA constitution data
├── README.md                     # This documentation
└── CEGSA Constitution.docx.pdf   # Original source document
```

## Browser Compatibility

- Modern browsers with ES6+ support
- Chrome, Firefox, Safari, Edge
- Mobile-friendly responsive design
- Works offline - no internet connection required

## No Dependencies Required

- **Pure HTML/CSS/JavaScript** - No server or external libraries needed
- **Works offline** - Open the HTML file directly in any browser
- **Cross-platform** - Works on Windows, Mac, Linux, mobile devices



