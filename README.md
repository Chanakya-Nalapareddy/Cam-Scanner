# Cam-Scanner


# Cam-Scanner

**Authors:** Chanakya Nalapareddy, Nosherwan Babar  
**Date:** 12/11/2024

---

## 📌 Program Description

This program implements a comprehensive pipeline for detecting and rectifying a document from an input image using computer vision techniques. The key steps include:

1. Preprocessing the image  
2. Applying Gaussian smoothing  
3. Performing edge detection using the Canny algorithm  
4. Detecting lines using the Hough Transform  
5. Finding intersections to identify the document corners  
6. Computing a homography matrix for rectification  
7. Generating a rectified (warped) version of the document

---

## 🚀 Features

### 1. All-in-One Script
- Entire code is contained in a single `.m` file.
- No external dependencies.

### 2. Custom Implementations
- Includes custom functions for Hough Transform, smoothing, and homography.

### 3. Easy Setup
- Just change the image path and run.

---

## 🛠️ Instructions to Run

### Requirements
- MATLAB (R2018b or later recommended)

### Input Image
- Place your image (e.g., `test_image.jpg`) in the same folder as the script.
- Make sure the image has a clear view of the document.

### Running the Script
Open MATLAB and run the following:
```matlab
>> run('your_script_name.m')
```
Replace `your_script_name.m` with the actual file name.

### Modify the File Path
At the start of the script, change the image filename if needed:
```matlab
img = imread('your_image_file.jpg');
```

---

## 📤 Output

The script displays and saves:

- Grayscale image  
- Edge-detected image  
- Hough accumulator  
- Lines overlay  
- Document corners  
- Rectified output

Saved files include:

- `resized_image.jpg`  
- `final_filtered_detected_image.png`  
- `rectified_image.jpg`

---

## 📌 Notes

- Use high-quality images with distinct document edges for best results.  
- If detection fails, try adjusting the Canny thresholds or Hough settings.

---
