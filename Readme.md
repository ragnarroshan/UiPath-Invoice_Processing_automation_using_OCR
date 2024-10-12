## Exercise_13-Invoice_Processing_automation_using_OCR

## Aim:

To automate the extraction of specific data (Invoice Number, Date, and Total Amount) from an invoice PDF using OCR and store the extracted information in an Excel file.

## Equipments Required:

UiPath Studio<br>
Invoice PDF file<br>
Excel file for storing extracted data<br>

#### Installed UiPath packages:

UiPath.PDF.Activities<br>
UiPath.IntelligentOCR.Activities<br>
UiPath.Excel.Activities<br>

## Procedure:

### Install UiPath and Required Packages:

Download and install UiPath Studio.<br>
Create a new project and install the necessary packages (PDF, OCR, Excel).<br>

### Read the Invoice PDF with OCR:

Use the Read PDF with OCR activity to extract text from the PDF.<br>
Choose an OCR engine like Tesseract to process the document.<br>

### Extract Specific Data Using Regex:

Add the Matches activity to extract the Invoice Number, Date, and Total Amount using regular expressions:<br>
Invoice Number: INV-\d+<br>
Date: \d{2}/\d{2}/\d{4}<br>
Total Amount: \₹?\d+(,\d{3})\*(\.\d{2})?<br>
Store the extracted values in variables.<br>

### Write Data to Excel:

Use the Excel Application Scope activity to open or create an Excel file.<br>
Write the extracted data (Invoice Number, Date, Total Amount) into specific cells using Write Cell activity.<br>

### Run and Test:

Run the workflow and verify that the data has been extracted correctly and saved into the Excel file.

## UiPath WorkFlow:
![alt text](<img/Screenshot 2024-10-12 201545.png>)
![alt text](<img/Screenshot 2024-10-12 202115.png>)
![alt text](<img/Screenshot 2024-10-12 203238.png>)
![alt text](<img/Screenshot 2024-10-12 203929.png>)
![alt text](<img/Screenshot 2024-10-12 204423.png>)
![alt text](<img/Screenshot 2024-10-12 204452.png>)
![alt text](<img/Screenshot 2024-10-12 204606.png>)
![alt text](<img/Screenshot 2024-10-12 205632.png>)
![alt text](<img/Screenshot 2024-10-12 205752.png>)
![alt text](<img/Screenshot 2024-10-12 205924.png>)
![alt text](<img/Screenshot 2024-10-12 210327.png>)

## Result:

The automation successfully extracts the Invoice Number, Date, and Total Amount from the PDF and enters them into an Excel file, demonstrating efficient invoice processing using OCR.
