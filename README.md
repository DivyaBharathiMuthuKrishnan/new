PDF Text Extraction for Experiment Documentation
Project Overview
This project automates the extraction of structured data from scientific experiment PDFs. By leveraging text extraction techniques such as PyPDF2, Tesseract OCR, and Groq LLM, the system is capable of processing complex PDFs with varying layouts. It focuses on extracting key information like Experiment Title, Procedure, Materials Used, and Observations, organizing it into a structured format for further analysis or reporting.

Features
Text Extraction: Extracts important sections of scientific experiments such as titles, procedures, materials used, and more.
Layout Handling: Capable of processing multi-column, table-based, or image-based PDFs using advanced extraction methods.
Data Cleaning: Removes unnecessary characters and noise from extracted text using Regular Expressions.
Structured Output: Saves the extracted data into a structured Excel file for easy analysis.
Dataset
Source: Scientific experiment PDFs provided by users.
Key Features:
Experiment Title, Procedure, Materials Used, Observations, Conclusion.
The dataset is dynamic and depends on the PDF files being processed.
System Workflow
Data Collection: Users provide PDFs containing scientific experiment details.
Text Extraction:
If the PDF contains text-based content, PyPDF2 extracts the text.
For image-based PDFs, Tesseract OCR is used for extraction.
Text Preprocessing:
Noise Removal: Remove extraneous characters such as special symbols, hyphens, etc., using Regular Expressions.
Layout Handling: Groq LLM is used for processing complex layouts and multi-column content.
Text Segmentation: The extracted text is split into logical sections like Title, Procedure, Materials, etc.
Data Organization: The extracted data is structured and saved into an Excel file.
Evaluation: The system compares the extracted data with the original PDF for validation and accuracy.
Libraries Used
Text Extraction:
PyPDF2, Tesseract OCR, Groq LLM.
Data Processing:
Pandas, NumPy, Scikit-learn.
Text Cleaning:
Regular Expressions.
Visualization:
Matplotlib, Seaborn.
System Requirements
Hardware:
Processor: Intel Core i7/i9 or AMD Ryzen 7/9.
RAM: Minimum 8GB (recommended 16GB).
Storage: 256GB SSD (minimum), 512GB SSD (recommended).
Software:
IDE: Google Colab (GPU-enabled).
Language: Python 3.x.
Installation and Usage
Clone the repository:


git clone https://github.com/your-repo-name/pdf-text-extraction.git
Install dependencies:
pip install -r requirements.txt
Run the Flask app:
Access the application:

Open a web browser and go to http://127.0.0.1:5000 to upload a PDF and extract experiments.
Download Extracted Data:

After processing, you can download the structured data in an Excel format directly from the results page.
Future Work
Enhanced OCR Integration: Improve OCR accuracy for better extraction from scanned PDFs, especially in non-standard fonts.
Automatic Table Extraction: Implement methods to handle and extract tables more effectively.
Support for Other Formats: Extend the system to handle other formats like Word or HTML for broader compatibility.
Contributing
Feel free to open issues or submit pull requests for bug fixes or feature improvements. Your contributions are welcome!
