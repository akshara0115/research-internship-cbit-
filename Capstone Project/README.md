### Digital Triage Assistant
Automatically extract and summarize symptoms from a handwritten note for use by front-desk nurses or emergency staff.

This project uses computer vision and natural language processing to streamline medical triage. By digitizing and summarizing symptoms from handwritten notes, it helps healthcare workers quickly identify critical cases.
Features
# Handwriting OCR: 
    Uses pytesseract to recognize handwritten text from images.

# Line Removal: 
    Cleans lined paper using OpenCV morphological transformations for better OCR accuracy.

# Symptom Extraction:
    Applies spaCy NLP to detect health-related terms.

# Summary Generation: 
    Produces a concise symptom list for quick triage decisions.
## Workflow
# 1.Image Preprocessing

Convert to grayscale

Apply Gaussian blur

Remove horizontal lines with adaptive thresholding and morphological operations

# 2.Text Extraction

Recognize text from the cleaned image using Tesseract OCR.

# 3. NLP Analysis

Tokenize and process text using spaCy.

Identify and extract medical symptoms.

# 4. Output

Display original image, processed image, recognized text, and extracted symptom summary.
## Example Use Case
A nurse scans or photographs a patient's handwritten note. The system cleans the image, extracts the symptoms, and generates a quick summary, enabling faster emergency care.
