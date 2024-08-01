# Google Image Downloader and Enhancer

This repository contains a Python script for downloading images from Google based on specified keywords and enhancing them using the Real-ESRGAN library.

## Contents

- `image.ipynb`: The main Jupyter Notebook file containing the code for downloading and enhancing images.

## Features

- **Download Images:** Download images from Google based on specified keywords.
- **Image Enhancement:** Utilize Real-ESRGAN for enhancing the downloaded images.

## Setup

1. **Clone Real-ESRGAN and Install Dependencies**

   The notebook starts by cloning the Real-ESRGAN repository and installing the necessary dependencies:

   ```python
   !git clone https://github.com/xinntao/Real-ESRGAN.git
   %cd Real-ESRGAN
   !pip install basicsr facexlib gfpgan
   !pip install -r requirements.txt
   ```

2. **Upload Files**

   The notebook uses Google Colab's file upload functionality:

   ```python
   from google.colab import files
   files.upload()
   ```

3. **Download and Enhance Images**

   A function is defined to download images from Google and enhance them:

   ```python
   def download_images(keywords, num_images, download_path, name):
       # Function implementation
   ```

## Usage

1. **Open the `image.ipynb` Notebook**

   Open the notebook in Google Colab or your preferred Jupyter environment.

2. **Run the Cells**

   Run the cells sequentially to set up the environment, upload files, and download images. Customize the keywords and other parameters as needed.

3. **Example Usage**

   ```python
   keywords = ["cat", "cute"]
   num_images = 10
   download_path = "./images"
   name = "cat_images"
   
   download_images(keywords, num_images, download_path, name)
   ```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [Real-ESRGAN](https://github.com/xinntao/Real-ESRGAN) by Xintao Wang and other contributors.

