# **Sanskrit Text Bounding Box Creation**

## Objective
To create **bounding boxes around each line of Sanskrit text** in the provided image file and save each individual line as a separate JPEG image.

## Steps 

## Image Preprocessing

- Load the provided **Sanskrit text image**.
- Convert the image to grayscale (if necessary) for better text detection.
- Apply any necessary image enhancement techniques (e.g., noise reduction, sharpening) to improve text clarity.

## Text Detection

- Use an appropriate text detection algorithm or library (e.g., OpenCV, Tesseract OCR, Pytesseract) to identify the text regions within the image.
- Extract the bounding boxes for each detected text region.
## Line Segmentation

- Analyze the extracted bounding boxes to identify individual lines of text.
- Apply techniques like horizontal projection profiles or morphological operations to separate lines based on their vertical spacing.
## Bounding Box Creation

- For each identified line, **create a bounding box that tightly encloses the text region**.
- Adjust the bounding box dimensions if necessary to ensure the text is fully contained.
## Image Cropping and Saving:

- Crop the original image using the calculated bounding box coordinates to extract the individual lines.
- Save each cropped line as a separate JPEG image with appropriate naming conventions (e.g., **"line1.jpg"**, "**line2.jpg**", etc.).
## Dependencies:

- Python
- OpenCV (or other image processing library)
- Text detection library (e.g., **Tesseract OCR, Pytesseract**)

## Usage:

- Clone this repository.
- Install the required dependencies using **pip install -r requirements.txt**.
- Place the Sanskrit text image file in the images directory.
- Run the **main.py** script to perform the bounding box creation and image saving.
- The output images will be saved in the output directory.
