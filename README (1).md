# Intensity Level Slicing using OpenCV

This project demonstrates **Intensity Level Slicing**, an image-processing technique used to highlight a specific range of pixel intensity values in a grayscale image.

The implementation uses Python, OpenCV, NumPy, and Matplotlib.

## Project Overview

Intensity level slicing emphasizes pixels within a selected intensity range while either suppressing or preserving the remaining parts of an image.

This notebook uses the following intensity range:

- Minimum intensity: `100`
- Maximum intensity: `200`

Two results are generated:

1. **Slicing Without Background** — pixels within the selected range are highlighted, while pixels outside the range are suppressed.
2. **Slicing With Background** — the original grayscale image is preserved, while pixels within the selected range are highlighted.

## Technologies Used

- Python
- OpenCV (`cv2`)
- NumPy
- Matplotlib
- Google Colab / Jupyter Notebook

## Project Structure

```text
Intensity-Level-Slicing/
├── cv_lab_5.ipynb
├── roolno21.jfif
└── README.md
```

Make sure the input image is included in the repository and matches the filename used in the notebook.

## Installation

Install the required libraries:

```bash
pip install opencv-python numpy matplotlib
```

## How to Run

1. Clone or download this repository.
2. Open `cv_lab_5.ipynb` in Jupyter Notebook or Google Colab.
3. Ensure that `roolno21.jfif` is available at the path expected by the notebook.
4. Run all cells.

The notebook uses this image path:

```python
img = cv2.imread("/content/roolno21.jfif", 0)
```

For local execution, update the path to the location of your image.

## Method

The image is loaded in grayscale, and each pixel is checked against the selected intensity range.

```python
r_min = 100
r_max = 200
```

Pixels whose intensity falls between 100 and 200 are highlighted in the processed outputs.

### Slicing Without Background

Only pixels in the selected intensity range are displayed; pixels outside the range are suppressed.

### Slicing With Background

The original grayscale image is preserved, and pixels in the selected intensity range are highlighted.

## Output

The notebook displays:

- Original grayscale image
- Intensity slicing without background
- Intensity slicing with background

These outputs allow visual comparison of the two slicing approaches.

## Learning Objectives

- Read images using OpenCV
- Work with grayscale pixel intensities
- Understand intensity level slicing
- Perform pixel-by-pixel image processing
- Generate and visualize processed images with Matplotlib

## Possible Improvements

- Let users select the intensity range interactively
- Display a histogram of pixel intensities
- Support multiple input images
- Save processed images to files
- Add a graphical user interface

## Author

Your Name
