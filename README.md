# Eigenfaces-Project

# Eigenfaces Using SVD & PCA

This project explores the use of Singular Value Decomposition (SVD) and Principal Component Analysis (PCA) in creating Eigenfaces, a technique used for facial recognition. Eigenfaces are a set of eigenvectors that represent the principal components of a dataset of facial images, allowing for dimensionality reduction while retaining essential features for recognition.

## Project Overview

Eigenfaces provide a way to represent a high-dimensional facial image space in a lower dimension. This project demonstrates how to compute Eigenfaces using SVD and PCA, applying these techniques to a dataset of facial images for tasks such as image reconstruction and classification.

### Key Objectives:
- Understand the concept of Eigenfaces and how they are used in facial recognition.
- Explore the relationship between SVD and PCA in the context of Eigenfaces.
- Implement the computation of Eigenfaces using a dataset of facial images.
- Demonstrate facial image reconstruction and classification using Eigenfaces.

## Methodology

1. **Background**: Eigenfaces are eigenvectors used in facial recognition problems, introduced by Sirovich and Kirby in 1987. They describe a set of bases derived using PCA and SVD to project facial images from a higher-dimensional space to a lower dimension.

2. **SVD and PCA**:
   - **SVD**: Singular Value Decomposition is used to compress images by truncating SVD matrices to lower dimensions, prioritizing components based on their singular values.
   - **PCA**: Principal Component Analysis reduces the number of variables while retaining essential information. The top eigenvectors are used to create Eigenfaces, which allow for comparison and recognition of facial features.

3. **Computing Eigenfaces**:
   - Obtain a set of facial images, ensuring they are the same size and centered.
   - Compute the mean face and subtract it from all images to normalize the dataset.
   - Perform SVD on the dataset to derive the principal components (eigenvectors).
   - Use the top eigenvectors to form the Eigenfaces, representing key facial features.

4. **Example Application**:
   - Images from the Yale Faces B dataset were used, consisting of 38 participants with varying lighting conditions.
   - Facial images were projected into principal components, and Eigenfaces were used for image reconstruction and classification.

## Results

- **Facial Reconstruction**: Linear combinations of the computed Eigenfaces were used to reconstruct images of participants, demonstrating the ability to capture and recreate facial features.
- **Image Classification**: Faces were projected into principal component space, enabling comparison and classification of facial images.

## Takeaways

- Eigenfaces provide an effective technique for facial recognition by breaking down facial features into a set of images that capture the essential features.
- **SVD** is a factorization technique that is more numerically stable but computationally expensive.
- **PCA** is a linear combination technique that is computationally efficient but less numerically stable.
- The Eigenfaces method has a higher success rate in facial recognition compared to other methods due to its ease and speed.

