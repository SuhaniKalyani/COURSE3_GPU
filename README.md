# Batch Image Processing with Gaussian Filtering

This project provides a robust solution for batch processing images by applying a 5x5 Gaussian blur. It's designed to handle a large number of `.tif` and `.tiff` images efficiently, making it suitable for enterprise-level image processing workflows. The primary function is to denoise grayscale images by smoothing them with a Gaussian filter.

While developed in the context of the "CUDA at Scale for the Enterprise" course, this implementation is CPU-based, utilizing OpenCV. It serves as a foundational version that can be extended for GPU acceleration with technologies like CUDA or NPP.

## Features

-   **Batch Processing**: Process multiple `.tif` and `.tiff` images from a specified input directory.
-   **Gaussian Blurring**: Applies a 5x5 Gaussian filter to reduce noise and detail in images.
-   **Grayscale Conversion**: Automatically converts images to grayscale before processing.
-   **Error Handling**: Includes checks for valid image loading.
-   **Organized Output**: Saves processed images to a separate directory with a `_gaussian` suffix to avoid overwriting original files.

## Project Structure

```
gpu_suhani_course3/
├── input_images/       # Directory for your input .tif and .tiff images
├── output_images/      # Processed images will be saved here
├── main.py             # The main script for processing images
├── HOW_TO_RUN.md       # Detailed instructions for setup and execution
└── README.md           # This file
```

## Quick Start

For detailed setup and execution instructions, please refer to [HOW_TO_RUN.md](HOW_TO_RUN.md).

### 1. Clone the Repository
```bash
git clone <repository-url>
cd gpu_suhani_course3
```

### 2. Set up Environment and Install Dependencies
Follow the instructions in [HOW_TO_RUN.md](HOW_TO_RUN.md) to set up a virtual environment and install the required packages (`numpy` and `opencv-python-headless`).

### 3. Run the Script
```bash
python main.py
```
Input images from `input_images/` will be processed, and the output will be saved in `output_images/`. For example, `image1.tiff` will be saved as `image1_gaussian.tiff`.

