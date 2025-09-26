# Image Denoising with Non-Local Means

## Description

This project explores image denoising using the **Non-Local Means (NLM) filter** with Gaussian noise at varying intensities. The repository includes:

1. **Gaussian Noise Addition**: Different noise levels are added to images using standard deviation variations.
2. **Denoising**: The images are denoised using the NLM filter implemented both on **CPU** and **GPU** (using CUDA).
3. **Performance Comparison**: The runtime of the CPU and GPU implementations is compared, showing significant speedup on the GPU.
4. **Quality Evaluation**: The denoising quality is evaluated using **PSNR** and **SSIM** metrics.

## Requirements

- Python 3.x
- OpenCV
- NumPy
- Matplotlib
- PyTorch (for GPU implementation)
- scikit-image (for metrics)

Install required packages using:

```bash
pip install opencv-python matplotlib numpy pytorch scikit-image
```

## Files

- **material**: Contains sample images such as `bird.jpg`, `vegetables.jpg`, and `woman.jpg` for noise addition and denoising.
- **image processing**: Includes methods for adding Gaussian noise, denoising, and evaluating quality metrics.

## How to Use

1. Run the notebook `Image_Denoising_with_Non_Local_Means.ipynb` in a Jupyter environment.
2. The notebook will load the images, add Gaussian noise, apply denoising using both CPU and GPU, and evaluate the denoising performance.
3. The results, including PSNR and SSIM values, are plotted for comparison.

## Results

The GPU-based implementation offers **approximately 17x faster** processing time compared to the CPU implementation, demonstrating the effectiveness of GPU acceleration for image processing tasks.

