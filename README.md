# Pytesseract_OCR

This project demonstrates a comprehensive Optical Character Recognition (OCR) pipeline using Python. The project includes preprocessing of images, OCR extraction using Tesseract, and further processing to extract specific entities from the OCR results.

## Project Structure

- `preprocessing.ipynb`: Notebook for image preprocessing.
- `ocr_index.ipynb`: Notebook for OCR extraction.
- `separate_footnote.ipynb`: Notebook for separating footnotes and further processing.
- 'pytesseract.ipynb` : use tesseract to perform ocr 

## Installation

To set up the environment and install the necessary dependencies, follow these steps:

1. Clone the repository:

    ```bash
    https://github.com/AfifaNoor/Pytesseract_OCR.git
    cd ocr-processing-project
    ```

2. Create a virtual environment and activate it:

    ```bash
    python -m venv myenv
    source myenv/bin/activate  # On Windows use `myenv\Scripts\activate`
    ```

3. Install the required packages:

    ```bash
    pip install -r requirements.txt
    ```

## Requirements

- Python 3.7+
- Tesseract-OCR
- OpenCV
- Pillow

To install Tesseract-OCR, follow the instructions on the [official Tesseract GitHub page](https://github.com/tesseract-ocr/tesseract).

## Usage

### Preprocessing

The `preprocessing.ipynb` notebook covers the steps for image preprocessing:

1. Reading the image.
2. Converting the image to grayscale.
3. Applying Gaussian blur.
4. Thresholding the image.
5. Dilation to enhance contours.

### OCR Extraction

The `ocr_index.ipynb` notebook covers the steps for OCR extraction:

1. Loading the preprocessed image.
2. Extracting text using Tesseract.
3. Processing the extracted text to identify entities.

### Separate Footnote

The `separate_footnote.ipynb` notebook covers the steps for further processing:

1. Identifying and separating footnotes from the main text.
2. Extracting specific entities and information.

### Running the Notebooks

To run the notebooks, use Jupyter Notebook or Jupyter Lab:

```bash
jupyter notebook
