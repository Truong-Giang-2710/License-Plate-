License Plate Recognization by using C# interface and EmguCV 

🔗 Project Links
- 📂 Source Code: https://drive.google.com/drive/folders/1imPfXzgRijyD2YVEARGf_d4dBTx0hHIb?usp=sharing
- 📺 Demo Video:  https://youtu.be/RZke8umycUk?si=BoDBp5Y-mwPv_SO2

📌 Overview
This project was "completely coded by me" from scratch, including interface design, image processing, and OCR logic. It is a C# Windows Forms application that uses **EmguCV (a .NET wrapper for OpenCV)** and **Tesseract OCR** to perform automatic and manual recognition of vehicle license plates.

This system is suitable for **vehicle access management** in various real-life scenarios with a recognition accuracy of 90%.
- 🏢 Company parking lots  
- 🏫 School or university campuses  
- 🏠 Residential areas or smart gates  
- 🅿️ Public parking systems  
 
🔧 Features
 🚗 Auto Recognition
- Real-time camera feed.
- Automatically detects and reads license plates when visible in front of the camera.
- Extracted license plate characters are displayed on screen using Tesseract OCR.
- Captured license plate images are saved automatically in the "./AutoCaptured/" folder.

I coded this project which is a Windows desktop application for license plate recognition using EmguCV (a .NET wrapper for OpenCV). The application features two main modes: **Auto** and **Manual**

 🛠️ Manual Processing
- Allows the user to load and manually enhance license plate images (especially those with blur, noise, glare, etc.).
- Supported image processing tools:
  - Negative (invert image)
  - Logarithmic Transform (enhance low contrast)
  - Histogram Equalization
  - Local Histogram Equalization (CLAHE)
- After enhancement, the user can apply OCR to extract the license plate number.
- Enhanced images can be saved into the "./ManualProcessed/" folder.

🖼️ GUI Overview
| Component            | Function                             |
|----------------------|--------------------------------------|
| PictureBox           | Display live feed or loaded image    |
| Button [Start]       | Start camera                         |
| Button [Capture]     | Capture and save image (Manual mode) |
| Button [OCR]         | Run OCR on current image             |
| Button [Negative]    | Apply Negative filter                |
| Button [Log Transform]| Apply Logarithmic transformation    |
| Button [Hist Equal]  | Apply Histogram Equalization         |
| Button [Local Hist]  | Apply CLAHE                          |
| TextBox              | Display recognized license text      |

🧠 Technologies Used
- **EmguCV** (OpenCV for C#)
- **Tesseract OCR**
- .NET WinForms or WPF (GUI)

 📁 Project Structure

