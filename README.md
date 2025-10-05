# Universal Content Preprocessor 🤖

A powerful, all-in-one tool designed to convert, clean, and process various file formats, making them ready for analysis by AI platforms like Google's NotebookLM.



## ✨ About The Project

This application was built to solve a common problem: getting content from various sources (like PDFs, Word documents, ebooks, and spreadsheets) into a clean, digestible format for AI models. It provides a simple web interface to handle complex preprocessing tasks, from OCR and table extraction to intelligent document splitting.

---

## 🚀 Features

This tool supports a wide range of processing workflows depending on the file type.

#### **📄 General Conversions**
* **Word, Markdown, Text (.docx, .md, .txt):** Convert to either a clean `.pdf` or `.txt` file.
* **PowerPoint (.pptx):** Extract all textual content into a single `.txt` file.
* **Excel, CSV (.xlsx, .csv):** Convert spreadsheet data into a clean, structured `.pdf` document that preserves the table layout.

#### **📑 Advanced PDF Toolkit**
When a PDF is uploaded, you can choose from a suite of powerful tools:
* **OCR:** Convert scanned, image-based PDFs into fully searchable documents.
* **Table Extraction:** Automatically detect and extract tables into separate `.csv` files.
* **Image Extraction:** Pull all embedded images from the PDF and save them as separate files.
* **Smart Splitting:** Intelligently split the PDF by chapter or section headings, with the ability to group multiple chapters into a single file.
* **Header/Footer Cleaning:** Automatically remove repetitive page numbers, titles, and other noise while preserving important footnotes and sources, saving the result as a clean `.txt` file.

#### **📚 Ebook (EPUB) Tools**
* **Chapter Splitting:** Split an `.epub` file into multiple, smaller PDF documents.
* **Smart Naming:** Automatically name the output files based on their chapter titles.
* **Chapter Grouping:** Use a simple slider to define how many chapters to include in each split file.

---

## 🛠️ Built With

This project is built with Python and leverages a number of powerful open-source libraries:

* **Framework:** [Streamlit](https://streamlit.io/)
* **Document Conversion:** [Pandoc](https://pandoc.org/)
* **PDF Processing:** [PyMuPDF](https://github.com/pymupdf/PyMuPDF)
* **OCR:** [Tesseract](https://github.com/tesseract-ocr/tesseract) & [pytesseract](https://github.com/madmaze/pytesseract)
* **Table Extraction:** [Camelot](https://camelot-py.readthedocs.io/en/master/)
* **Data Handling:** [Pandas](https://pandas.pydata.org/)
* **Office Files:** [python-pptx](https://python-pptx.readthedocs.io/en/latest/), [openpyxl](https://openpyxl.readthedocs.io/en/stable/)

---

## ⚙️ Getting Started (Running Locally)

To get a local copy up and running, follow these simple steps.

### **Prerequisites**
* Python 3.8 or higher installed on your system.
* The system dependencies listed in `packages.txt` (for Linux/macOS).

### **Installation & Execution**
1.  Clone the repository:
    ```sh
    git clone [https://github.com/your_username/your_repository_name.git](https://github.com/your_username/your_repository_name.git)
    ```
2.  Navigate to the project directory:
    ```sh
    cd your_repository_name
    ```
3.  Install the required Python packages:
    ```sh
    pip install -r requirements.txt
    ```
4.  Run the Streamlit app:
    ```sh
    streamlit run app.py
    ```
The application should automatically open in your web browser.

---

## 💡 Future Improvements

* Transcribe audio and video files.
* Add support for converting HTML files or live URLs.
* Integrate more advanced data extraction features.
