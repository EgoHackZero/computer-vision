# Computer Vision Course

A comprehensive collection of Jupyter notebooks covering fundamental concepts and techniques in computer vision and image processing. This repository contains hands-on tutorials and exercises for learning computer vision from the ground up.

## Overview

This repository includes practical implementations of various computer vision techniques using Python, NumPy, Matplotlib, Scikit-image, and SciPy. Each notebook focuses on specific topics with clear explanations, code examples, and visualizations.

## Contents

### Notebooks

1. **00_numpy_recap.ipynb** - NumPy fundamentals and array operations
2. **01_image_processing.ipynb** - Basic image processing operations
   - Loading images from files, URLs, and libraries
   - RGB to grayscale conversion
   - Image transformations (rotation, resizing, scaling)
   - Channel manipulation
3. **02_image_quality_processing.ipynb** - Image quality enhancement techniques
4. **03_image_segmentation.ipynb** - Image segmentation methods
5. **04_textures.ipynb** - Texture analysis and processing
6. **05_image_convolution.ipynb** - Convolution operations and filters
7. **try.ipynb** - Experimental notebook for testing

### Data

- `_data/` - Directory containing sample images and datasets
- `textury_train/` - Training textures dataset
- `image.jpg`, `sonet.png` - Sample images

## Requirements

### Dependencies

```python
numpy
matplotlib
scipy
scikit-image
Pillow
requests
```

### Installation

```bash
pip install numpy matplotlib scipy scikit-image Pillow requests
```

Or using conda:

```bash
conda install numpy matplotlib scipy scikit-image pillow requests
```

## Usage

1. Clone this repository:
```bash
git clone https://github.com/EgoHackZero/computer-vision.git
cd computer-vision
```

2. Install the required dependencies (see Installation section above)

3. Launch Jupyter Notebook:
```bash
jupyter notebook
```

4. Open any notebook and run the cells sequentially

## Topics Covered

### Image Fundamentals
- Understanding images as NumPy arrays
- RGB and grayscale color spaces
- Image loading from various sources (local files, URLs, libraries)

### Image Processing
- Color space conversions
- Image transformations (rotation, scaling, resizing)
- Channel manipulation and separation
- Random noise generation

### Advanced Techniques
- Image quality enhancement
- Segmentation methods
- Texture analysis
- Convolution and filtering

## Examples

### Loading and Processing Images

```python
from skimage import io, data
from skimage.color import rgb2gray
import matplotlib.pyplot as plt

# Load image from library
image = data.astronaut()

# Convert to grayscale
gray_image = rgb2gray(image)

# Display
plt.imshow(gray_image, cmap='gray')
plt.show()
```

## Project Structure

```
computer-vision/
│
├── _data/                      # Sample images and datasets
├── textury_train/             # Texture training data
├── 00_numpy_recap.ipynb       # NumPy basics
├── 01_image_processing.ipynb  # Basic image processing
├── 02_image_quality_processing.ipynb
├── 03_image_segmentation.ipynb
├── 04_textures.ipynb
├── 05_image_convolution.ipynb
├── try.ipynb                  # Experimental notebook
├── LICENSE                    # Project license
└── README.md                  # This file
```

## Learning Path

For beginners, it's recommended to follow the notebooks in numerical order:

1. Start with `00_numpy_recap.ipynb` to refresh NumPy skills
2. Progress through `01_image_processing.ipynb` for fundamentals
3. Continue with subsequent notebooks for advanced topics

## Contributing

Contributions are welcome! If you'd like to add new examples, fix bugs, or improve documentation:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

Copyright (c) 2025 EgoHackZero. All rights reserved.

## Author

**EgoHackZero**

## Acknowledgments

- Scikit-image library for image processing tools
- NumPy and SciPy communities for numerical computing foundations
- All contributors and learners using this repository

## Resources

- [Scikit-image Documentation](https://scikit-image.org/)
- [NumPy Documentation](https://numpy.org/doc/)
- [Matplotlib Documentation](https://matplotlib.org/)
- [Computer Vision Fundamentals](https://en.wikipedia.org/wiki/Computer_vision)

## Support

For questions, issues, or suggestions, please open an issue in the GitHub repository.

---

**Note**: This repository is intended for educational purposes and learning computer vision concepts.
