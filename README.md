# Color_normalisation


# Stain Normalization for PanNuke Dataset

This repository contains a Python script for normalizing tissue stains in images from the PanNuke dataset. The normalization is performed using differnt stain normalization techniques on 19 different tissue types.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Metrics](#metrics)
- [License](#license)
- [Contributing](#contributing)

## Installation

To run the code in this repository, you will need the following Python packages:

- `numpy`
- `Pillow`
- `requests`
- `opencv-python`
- `scikit-image`
- `tiatoolbox`

You can install the required packages using pip:

```bash
pip install numpy Pillow requests opencv-python scikit-image tiatoolbox
```

## Usage

1. **Prepare your input data**:

   - Place the images you want to normalize in the `input_folder` directory. The code currently processes images in `.png` format.

2. **Set the parameters**:

   In the script, update the paths for the input folder, output folder, and reference image URL. For example:

   ```python
   input_folder = "/path/to/your/input/folder"
   output_folder = "/path/to/your/output/folder"
   reference_image_url = "https://your.reference.image.url"
   ```

3. **Run the normalization**:

   Execute the Jupyter Notebook. The script will normalize the stains in the images and save the results in the specified output folder.

## Metrics

The following metrics are calculated for each normalized image:

- **Pearson Correlation Coefficient (PCC)**: Measures the correlation between color channels of the original and normalized images.
- **AMCE-alpha (Eα)**: Assesses the difference in mean alpha (Red channel) between target and processed images.
- **AMCE-beta (Eβ)**: Assesses the difference in mean beta (Blue channel) between target and processed images.
- **Relative Square Error (RSE)**: Measures the relative error between original and normalized images.
- **Peak Signal-to-Noise Ratio (PSNR)**: Evaluates the quality of the normalized image.
- **Structural Similarity Index (SSIM)**: Compares the structural similarity between original and normalized images.



## Contributing

Contributions are welcome! If you have suggestions for improvements or would like to add features, please fork the repository and submit a pull request.

---

Feel free to replace the placeholder values (like `yourusername` and `repository-name`) with your actual GitHub username and repository name. Let me know if you need any further assistance!
