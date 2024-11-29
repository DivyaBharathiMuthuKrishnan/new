# *PDF Text Extraction for Experiment Documentation*

## *Project Overview*
This project automates the extraction of structured data from scientific experiment PDFs. By leveraging text extraction techniques such as **PyPDF2**, **Tesseract OCR**, and **Groq LLM**, the system is capable of processing complex PDFs with varying layouts. It focuses on extracting key information like **Experiment Title**, **Procedure**, **Materials Used**, and **Observations**, organizing it into a structured format for further analysis or reporting.

---

## *Features*
- **Text Extraction**: Extracts important sections of scientific experiments such as titles, procedures, materials used, and more.  
- **Layout Handling**: Capable of processing multi-column, table-based, or image-based PDFs using advanced extraction methods.  
- **Data Cleaning**: Removes unnecessary characters and noise from extracted text using **Regular Expressions**.  
- **Structured Output**: Saves the extracted data into a structured **Excel file** for easy analysis.  

---

## *Dataset*
- **Source**: Scientific experiment PDFs provided by users.  
- **Key Features**:
  - **Experiment Title**, **Procedure**, **Materials Used**, **Observations**, **Conclusion**.  
  - The dataset is dynamic and depends on the PDF files being processed.  

---

## *System Workflow*
1. **Data Collection**: Users provide PDFs containing scientific experiment details.  
2. **Text Extraction**:  
   - If the PDF contains text-based content, **PyPDF2** extracts the text.  
   - For image-based PDFs, **Tesseract OCR** is used for extraction.  
3. **Text Preprocessing**:  
   - **Noise Removal**: Remove extraneous characters such as special symbols, hyphens, etc., using **Regular Expressions**.  
   - **Layout Handling**: **Groq LLM** is used for processing complex layouts and multi-column content.  
   - **Text Segmentation**: The extracted text is split into logical sections like **Title**, **Procedure**, **Materials**, etc.  
4. **Data Organization**: The extracted data is structured and saved into an **Excel file**.  
5. **Evaluation**: The system compares the extracted data with the original PDF for validation and accuracy.

---

## *Key Results*

| **Method**             | **Accuracy** | **Efficiency**  | **Interpretation**                                                            |
|------------------------|--------------|-----------------|-------------------------------------------------------------------------------|
| **PyPDF2**             | High         | Moderate        | Best suited for simple, text-based PDFs but struggles with complex layouts.   |
| **Tesseract OCR**      | Moderate     | High            | Effective for image-based PDFs, but OCR accuracy depends on image quality.    |
| **Groq LLM**           | Very High    | Moderate        | Excellent for handling complex layouts with context-aware extraction.         |
| **Regular Expressions**| Very High    | High            | Efficient for cleaning and formatting extracted text.                          |

---

## *Libraries Used*
1. **Text Extraction**:  
   - PyPDF2, Tesseract OCR, Groq LLM.  
2. **Data Processing**:  
   - Pandas, NumPy, Scikit-learn.  
3. **Text Cleaning**:  
   - Regular Expressions.  
4. **Visualization**:  
   - Matplotlib, Seaborn.  

---

## *System Requirements*

### **Hardware**:  
- **Processor**: Intel Core i7/i9 or AMD Ryzen 7/9.  
- **RAM**: Minimum 8GB (recommended 16GB).  
- **Storage**: 256GB SSD (minimum), 512GB SSD (recommended).  

### **Software**:  
- **IDE**: Google Colab (GPU-enabled).  
- **Language**: Python 3.x.  

---

## *Installation and Usage*

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-repo-name/pdf-text-extraction.git

