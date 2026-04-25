# FaceShade OpenCV


**Name:** Deepak S  
**Register Number:** 212224230053 


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
   <img src="https://github.com/user-attachments/assets/026161a5-436b-4e78-a368-120764563c93" width="500"/>

2. **Face Detection**  
   A Haar Cascade classifier is used to detect the face region in the image.

3. **Locate Eye/Face Region**  
   The detected face coordinates are used to estimate where the sunglasses should be placed.

4. **Load Sunglasses Image**  
   A transparent PNG image of sunglasses is loaded from the `assets/` folder.  
   <img src="https://github.com/user-attachments/assets/2e0f7e4a-1f91-4466-9950-f4d77d6f1e27" width="500"/>

5. **Resize the Sunglasses**  
   The sunglasses image is resized based on the width of the detected face for proper alignment.

6. **Overlay the Sunglasses**  
   The resized sunglasses are placed on the face using image blending techniques (handling transparency).  
   <img src="https://github.com/user-attachments/assets/1a228207-c254-40f8-b224-4a9b164096a4" width="500"/>

7. **Save Output Image**  
   The final image is saved in the `output/` folder.  
   <img src="https://github.com/user-attachments/assets/543b8d5a-da26-4b3d-9049-b453f9cb12aa" width="500"/>

---

## Result

The project successfully overlays sunglasses onto the detected face, producing a clean and visually enhanced result. The use of alpha blending ensures smooth integration, making the output appear natural and well-aligned.
