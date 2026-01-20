PDF Form Filler (CSV → PDF)
Browser-based tool to automatically fill PDF forms from CSV (and other spreadsheet exports). Upload a fillable PDF and a data file, map fields once, then generate a batch of completed PDFs in seconds—no manual copy-paste, no server, everything runs client-side.


Features
* Automatic mapping between CSV columns and PDF form fields, with manual overrides when needed.  
* Batch generation of filled PDFs: one row in your data produces one completed PDF.  
* 100% client-side: files are processed in your browser; nothing is uploaded to a server.  
* Drag-and-drop interface for both the PDF template and the CSV file.  
* Useful for HR forms, applications, contracts, certificates, and other repetitive PDFs.  
How it works
1. Prepare a fillable PDF Your PDF must have real form fields (AcroForm). If your document is just a static or scanned PDF, first add form fields using a PDF editor such as Adobe Acrobat or similar tools.  
2. Prepare your CSV or spreadsheet export Each row represents one completed PDF.   Each column represents a field you want to fill (for example: first_name, last_name, dob, email, is_member).   Boolean fields (checkboxes) can use values like Yes/No, True/False, or 1/0, depending on how your template is configured.  
3. Upload and map fields Open the app in your browser and upload the PDF template. Upload your CSV (or other spreadsheet export converted to CSV).   The app suggests mappings between CSV columns and PDF fields based on their names; you can review and adjust these mappings before running the batch.  
4. Generate and download PDFs Run the batch fill process to generate one filled PDF per row in your data file.   Download the results individually or all at once (for example as a ZIP archive, depending on the implementation).  
Usage
1. Open the hosted app URL in a modern browser (for example, via GitHub Pages or another static host).  
2. Drag and drop your fillable PDF form into the PDF upload area.
3. Drag and drop your CSV file into the data upload area.
4. Confirm or adjust the automatically suggested field mappings.  
5. Start the batch fill process and wait for the generation to complete.
6. Download the generated PDFs and distribute them as needed.  
This tool is intended for small-to-medium batches (hundreds to low thousands of rows), with actual limits depending on your browser and machine, since all processing happens locally.


Development
This is a static front-end project:
* All logic runs client-side in JavaScript; there is no backend component.  
* You can clone the repository and open index.html directly in a modern browser to run it locally.  
Typical workflow:
1. Clone the repository or download it as a ZIP.
2. Open index.html in your browser to test changes.
3. Commit and push updates to the main branch to redeploy (for example, through GitHub Pages).  
If you want to extend the project, you can:
* Integrate or swap in a different PDF library for form filling and field handling.  
* Add additional parsers for Excel or Google Sheets exports in the browser and convert them to CSV automatically.  
* Improve error messages, validation, and performance for large files and edge cases.  
Limitations
* Requires PDFs with form fields; scanned or static PDFs without fields are not supported by default.  
* Performance, maximum file size, and maximum row count depend on the user’s browser and hardware, because everything runs locally.  
* Complex PDFs with many pages or heavy graphics may process more slowly or hit memory limits in some environments.  
License
This project is released under the MIT License. You are free to use, modify, and distribute it within your team or organization, subject to the terms of the MIT License.
