# Histogram Equalization for Image Enhancement

## Overview

This project demonstrates the implementation of **Histogram Equalization (HE)** for grayscale image enhancement as part of a Computer Vision assignment.

Histogram Equalization is a widely used image processing technique that improves image contrast by redistributing pixel intensity values over a wider range. This method is particularly useful when an image contains low contrast and most intensity values are concentrated within a limited interval.

The project applies Histogram Equalization to a grayscale image (`cat.jpg`), visualizes the original and equalized histograms, and analyzes the effects of the transformation on image quality and contrast.

---

## Objectives

* Load and analyze a grayscale image.
* Compute the image histogram.
* Calculate the Probability Density Function (PDF).
* Compute the Cumulative Distribution Function (CDF).
* Generate a lookup table for Histogram Equalization.
* Apply the transformation to obtain an enhanced image.
* Compare the original and equalized images using histogram analysis.

---

## Technologies Used

* Python
* NumPy
* OpenCV
* Matplotlib

---

## Processing Pipeline

1. Load the input image.
2. Extract a grayscale channel.
3. Compute the original histogram.
4. Normalize the histogram to obtain the PDF.
5. Calculate the CDF.
6. Build the lookup table using the Histogram Equalization formula.
7. Transform the image using the lookup table.
8. Generate and visualize the equalized image.
9. Compute and plot the equalized histogram.
10. Analyze and compare the results.

---

## Results

### Original Image

* Pixel intensities are concentrated within a limited range.
* Low contrast reduces the visibility of image details.
* Histogram contains strong peaks in specific intensity intervals.

### Equalized Image

* Pixel intensities are distributed more uniformly.
* Overall image contrast is improved.
* Details in dark and bright regions become more visible.
* Histogram becomes more spread across the intensity range.

---

## Discussion

Histogram Equalization successfully increases image contrast and improves visibility of details. However, global Histogram Equalization may over-enhance some regions and introduce unnatural brightness changes in certain images.

For more balanced local contrast enhancement, adaptive methods such as **CLAHE (Contrast Limited Adaptive Histogram Equalization)** can be considered.

---


