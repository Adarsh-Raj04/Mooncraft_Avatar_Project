# Moonraft Avatar Project
[![GitHub forks](https://img.shields.io/github/forks/Adarsh-Raj04/Mooncraft_Avatar_Project)](https://github.com/Adarsh-Raj04/Mooncraft_Avatar_Project/network)
[![GitHub stars](https://img.shields.io/github/stars/Adarsh-Raj04/Mooncraft_Avatar_Project)](https://github.com/Adarsh-Raj04/Mooncraft_Avatar_Project/stargazers)
[![GitHub forks and stars](https://img.shields.io/github/stars/Adarsh-Raj04/Mooncraft_Avatar_Project.svg?style=social&label=Forks%20%26%20Stars)](https://github.com/Adarsh-Raj04/Mooncraft_Avatar_Project)



This project is designed to create cartoon like avatar from an input image using OpenCV and Python. The script takes an input image, applies several image processing techniques, and generates a cartoon-like avatar of the image.

## Prerequisites

Before running the script, make sure you have the following dependencies installed:

- OpenCV (`cv2`)
- NumPy (`numpy`)
- Matplotlib (`matplotlib`)

You can install these dependencies using `pip`:

```bash
pip install opencv-python numpy matplotlib
```
Getting Started
Clone this repository or download the script to your local machine.

Place the image you want to cartoonify in the same directory as the script, or specify the file path when calling the read_file function by modifying the filename variable.

Run the script:

```bash
python project.py
```
How the Script Works
Load and Display the Image: The script starts by reading and displaying the input image.

Edge Mask Generation: An edge mask is generated using the edge_mask function. This mask highlights the edges in the image, which is a crucial step in creating a cartoon effect.

Color Quantization: The color_quantization function reduces the number of colors in the image. This step simplifies the image's color palette, making it look more like a cartoon.

Noise Reduction: A bilateral filter is applied to the quantized image to reduce noise and smooth out the colors.

Combine Edge Mask with Quantized Image: The edge mask is combined with the quantized image to create the final cartoon-like effect.

Display Results: The script displays the cartoon avatar image as well as the original image for comparison.

Customization
You can customize the avatar creation process by adjusting the following parameters:

line_size and blur_value in the edge_mask function: These parameters control the thickness of the edges in the cartoon effect.
k in the color_quantization function: This parameter determines the number of colors in the simplified color palette. You can experiment with different values to achieve different cartoon styles.
Parameters in the cv2.bilateralFilter function: You can modify d, sigmaColor, and sigmaSpace to adjust the noise reduction and color smoothing.
Example
Here's an example of how to use the script:



# Load and display the image
```bash
filename = "./input.jpg" #change it with the required file path.

img = read_file(filename)
```


# create cartoon like avatar the image and display the result
```bash
avatar()
```

License
This project is licensed under the MIT License. Feel free to use and modify the code for your own projects.
