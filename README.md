# Constitution Maker

A simple, powerful tool for creating, editing, and generating constitutions in HTML and PDF formats. Based on the real CEGSA (Computer Engineering Student Association) constitution structure.

## 📄 How to Save as PDF (Most Important!)

**This is the #1 feature you'll use:**

1. **Open** `constitution-generator.html` in your web browser
2. **Edit** your constitution content as needed
3. **Click "Export PDF"** button
4. **Print dialog opens** - Look for the **"Destination"** dropdown
5. **Change destination** from your printer to **"Save as PDF"**
6. **Click "Save"** and choose where to save your PDF file
7. **Done!** You now have a professional PDF constitution

> 💡 **Tip**: The PDF will have perfect formatting with Roman numerals, bullet points, and proper legal document styling.

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

## Example Use Cases

- **Student Organizations**: Create constitutions for clubs and societies
- **Non-profit Organizations**: Draft governing documents
- **Community Groups**: Establish rules and procedures
- **Professional Associations**: Create membership guidelines
- **International Organizations**: Multi-language constitution support

## Tips for Best Results

1. **Use clear, concise language** in your constitution text
2. **Test PDF generation** with your specific content
3. **Save JSON backups** regularly during editing
4. **Use templates** as starting points for common organization types
5. **Review formatting** in both HTML and PDF outputs
6. **Consider legal review** for important constitutions

