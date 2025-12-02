# Kanban Notes

A lightweight, drag-and-drop kanban board application built with vanilla JavaScript. Organize your notes and tasks into customizable columns with an elegant interface.

## Features

- **Drag and Drop**: Reorder items within columns and move items between columns
- **Column Management**:
  - Add unlimited columns
  - Rename columns by clicking on the title
  - Reorder columns by dragging
  - Delete columns when no longer needed
- **Item Management**:
  - Add notes/tasks to any column
  - Edit items by clicking on them
  - Delete items with the × button
  - Support for multi-line text content
- **Import/Export**:
  - Export your board to markdown format
  - Import from markdown to restore or share boards
  - Supports Upnote app import format
  - Download as `.md` file or copy to clipboard
- **Data Persistence**: Deleted notes are archived to localStorage with timestamps
- **Responsive Design**: Clean, modern interface with smooth animations

## Getting Started

Simply open `index.html` in a web browser. No build process or dependencies required.

```bash
# Clone the repository
git clone <repository-url>
cd kanban-notes

# Open in browser
open index.html  # macOS
xdg-open index.html  # Linux
start index.html  # Windows
```

## Usage

### Adding Columns

Click the **+ Add Column** button at the top of the page. The new column title will be automatically selected for editing.

### Adding Items

1. Type your note in the input field at the bottom of any column
2. Press **Enter** or click the **+** button

### Editing

- **Column titles**: Click on the column title to edit
- **Items**: Click on any item to edit its text
- Press **Enter** to save changes
- Press **Escape** to cancel editing

### Drag and Drop

- **Items**: Click and drag any item to reorder within a column or move to another column
- **Columns**: Click and drag the ☰ handle to reorder columns

### Import/Export

#### Export
1. Click the **Export** button
2. Choose to either:
   - **Copy to Clipboard**: Copy the markdown directly
   - **Download**: Save as `notes.active.md`

#### Import
1. Click the **Import** button
2. Paste your markdown content
3. Click **Import** to load

**Note**: Importing replaces current notes. Your previous notes are automatically archived to `notes.deleted.md` (localStorage).

## Markdown Format

The application uses a simple markdown format for import/export:

```markdown
## Column Name

Item 1 text here

Item 2 text here

---

## Another Column

Item 3 text here
```

- Column headings use `##`
- Items are separated by blank lines
- Columns are separated by `---`

## File Structure

```
kanban-notes/
├── index.html           # Complete application (HTML, CSS, JS)
├── notes.active.md      # Current active notes
├── notes.deleted.md     # Archive of deleted notes
├── notes.example.md     # Example notes for reference
└── README.md            # This file
```

## Example Data

The application loads with example notes from Robinson Crusoe organized into three columns:
- Provisions & Supplies
- Shelter & Fortification
- Daily Labours

## Browser Compatibility

Works in all modern browsers that support:
- HTML5 Drag and Drop API
- ES6 JavaScript
- CSS3 animations
- localStorage

## License

[Add your license here]

## Contributing

Contributions are welcome! Feel free to submit issues or pull requests.
