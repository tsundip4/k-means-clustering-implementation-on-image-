Overview
This project demonstrates image compression using the K-Means clustering algorithm from the scikit-learn library.
The technique reduces the number of colors in an image by grouping similar pixel colors into a smaller set of representative colors (clusters).

Technologies Used
Python
NumPy
Matplotlib
scikit-learn (KMeans)

Project Structure
The notebook contains the following steps:

Import Libraries
  NumPy, Matplotlib, and KMeans from scikit-learn.
Load and Display Image
  Read an image (sanp.jpg) from the sample_data directory.
  Display the original image using Matplotlib.
Image Analysis
  Print image dimensions (height, width, channels).
  Display data type and pixel value range.
Pixel Extraction
Reshape the image into a 2D array of pixels (each row = RGB values).
  K-Means Clustering
Define the number of clusters (k=16).
  Fit K-Means on the pixel data.
  Replace each pixel with its nearest cluster center.
  Convert compressed pixels back to image shape.
  
Results
  Display the original and compressed images side-by-side.
  Print the final cluster centers (representative colors).

Key Features
  Reduces image color palette to k colors.
  Uses K-Means clustering for efficient color quantization.
  Compares original and compressed images visually.
  Outputs cluster centers (RGB values) used for compression.

Example Output
Original image shape: (3624, 2295, 3)
Compressed image uses only 16 colors.
Cluster centers are printed as RGB values.

Notes
Ensure the image file (sanp.jpg) is placed in the sample_data directory.
Adjust k to change the level of compression (higher k = more colors = better quality).
The compressed image is saved as a uint8 array with pixel values rounded to nearest integers.

Applications
Image size reduction for web optimization.
Color quantization for artistic effects.
Preprocessing for image analysis tasks.

