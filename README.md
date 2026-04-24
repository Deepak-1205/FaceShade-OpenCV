# FaceShade OpenCV

FaceShade OpenCV is a fun and creative computer vision project that adds stylish sunglasses to passport-size photos using image processing techniques. It transforms ordinary images into visually appealing outputs using simple and efficient methods.

---

## Features

- Detects faces in an image automatically  
- Adds a properly aligned sunglasses overlay  
- Works best with passport-size or single-face images  
- Easily customizable with different sunglasses styles  
- Fast and lightweight implementation  

---

## Technologies Used

- Python  
- OpenCV – for face detection and image processing  
- NumPy – for array manipulation  

---
## How It Works

The project uses basic computer vision techniques to detect a face and place a sunglasses overlay accurately.

1. **Load Input Image**  
   The program reads the input image from the `images/` folder using OpenCV.

2. **Face Detection**  
   A Haar Cascade classifier is used to detect the face region in the image.

3. **Locate Eye/Face Region**  
   The detected face coordinates are used to estimate where the sunglasses should be placed.

4. **Load Sunglasses Image**  
   A transparent PNG image of sunglasses is loaded from the `assets/` folder.

5. **Resize the Sunglasses**  
   The sunglasses image is resized based on the width of the detected face for proper alignment.

6. **Overlay the Sunglasses**  
   The resized sunglasses are placed on the face using image blending techniques (handling transparency).

7. **Save Output Image**  
   The final image is saved in the `output/` folder.
