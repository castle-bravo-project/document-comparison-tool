# Document Comparison Tool

A powerful, privacy-focused web application for comparing documents and images with advanced diff algorithms.

## Overview

The Document Comparison Tool is a client-side web application that allows users to compare two documents or images side-by-side. It supports multiple file formats (PDF, Word, Text, and Images) and provides detailed comparison results using various diff algorithms. All processing is done locally in the browser, ensuring maximum privacy and security.

## Features

- **Supported Formats**: Compare PDF, Word (.docx, .doc), Text (.txt), and Image (.png, .jpg, .jpeg) files.
- **Multiple Diff Algorithms**:
  - Myers' Algorithm: Line-based comparison for precise differences.
  - Word-based Comparison: Granular word-level diff analysis.
  - Line-based Comparison: High-level line-by-line comparison.
- **Privacy First**: All processing occurs locally in the browser with no data sent to external servers.
- **Interactive UI**: Drag-and-drop file upload, side-by-side comparison view, and detailed statistics (similarity score, additions, deletions, modifications).
- **Customizable Options**: Ignore whitespace during comparison for cleaner results.
- **Report Generation**: Generate and download a text-based comparison report.
- **Responsive Design**: Built with Tailwind CSS for a modern, responsive interface.

## Installation

No installation is required! The Document Comparison Tool is a single-page web application that runs entirely in the browser.

1. Clone or download the repository:
   ```bash
   git clone https://github.com/yourusername/document-comparison-tool.git
   ```
2. Open `index.html` in a modern web browser (Chrome, Firefox, Edge, etc.).
3. Start comparing documents immediately.

## Usage

1. **Upload Files**:
   - Drag and drop files into the designated areas or click to browse.
   - Select an original document and a comparison document (supports PDF, Word, Text, or Images).
2. **Configure Comparison**:
   - Choose a diff algorithm (Myers, Word-based, or Line-based) from the dropdown.
   - Optionally enable "Ignore whitespace" for cleaner results.
3. **Compare**:
   - Click the "Compare Documents" button to process and display results.
   - View similarity score, additions, deletions, and modifications in the results section.
   - Inspect the side-by-side comparison with color-coded differences:
     - **Green**: Additions
     - **Red**: Deletions
     - **Yellow**: Modifications
     - **Gray**: Unchanged
4. **Generate Report**:
   - Click "Generate Comparison Report" to download a text file summarizing the results.
5. **Clear All**: Reset the tool by clicking the "Clear All" button.

## Dependencies

The tool uses the following libraries, loaded via CDN:
- **PDF.js** (v3.11.174): For PDF file parsing.
- **Mammoth.js** (v1.4.2): For Word document extraction.
- **JSZip** (v3.10.1): For handling Word document processing.
- **Tailwind CSS**: For responsive styling.

No additional setup is required, as all dependencies are included via CDN links.

## Privacy & Security

- **Local Processing**: All document processing happens in the browser, ensuring no files are uploaded to external servers.
- **Data Cleanup**: Temporary data is cleared automatically after comparison and on page unload.
- **No Tracking**: The tool does not use analytics or tracking mechanisms.
- **Secure Design**: Built with privacy as a priority, ensuring your documents remain confidential.

## Development

To modify or extend the tool:

1. **File Structure**:
   - `index.html`: The main application file containing HTML, CSS, and JavaScript.
2. **Customization**:
   - Modify the Tailwind CSS classes in the `<style>` section for styling changes.
   - Extend the diff algorithms in the `<script>` section by adding new comparison methods.
3. **Testing**:
   - Test with various file formats to ensure compatibility.
   - Use browser developer tools to debug JavaScript and inspect performance.
4. **Contributing**:
   - Fork the repository, make changes, and submit a pull request.
   - Follow the [Contributing Guidelines](#contributing) below.

## Contributing

We welcome contributions! To contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature`).
3. Commit your changes (`git commit -m "Add your feature"`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Open a pull request with a detailed description of your changes.

Please ensure your code follows the existing style and includes appropriate tests.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Built with ❤️ using open-source libraries: PDF.js, Mammoth.js, JSZip, and Tailwind CSS.
- Inspired by the need for privacy-focused document comparison tools.

---

For issues or feature requests, please open an issue on the GitHub repository.
