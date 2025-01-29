

---

### *README - Efficient CBIR Using Privacy-Preserving Feature Extraction*

#### *Project Title:*  
*Efficient Content-Based Image Retrieval Using Privacy Preserving Based Feature Extraction on Cloud*

#### *Authors:*  
- Ms. G. Sahishna (21WH1A1266)  
- Ms. M. Harshitha (21WH1A12B0)  
- Ms. K. Manaswini (21WH1A12C7)  
- Ms. A. Srivarshitha (21WH1A12C8)  

#### *Institution:*  
BVRIT Hyderabad College of Engineering for Women  
Affiliated to Jawaharlal Nehru Technological University, Hyderabad  

#### *Guide:*  
Ms. M. Sudha Rani (Assistant Professor, IT Department)  

---

## *Project Overview*
This project implements a *Content-Based Image Retrieval (CBIR) system* on a *cloud platform* while ensuring *privacy-preserving feature extraction*. The system enables efficient image retrieval without revealing sensitive image content.  

## *Key Features*
- *Privacy-Preserving Image Retrieval*  
  - Encrypts images before uploading to the cloud.  
  - Uses privacy-preserving techniques to extract image features.  

- *Efficient Content-Based Retrieval*  
  - Searches for similar images based on extracted features.  
  - Reduces computational and communication overhead.  

- *Security Enhancement*  
  - Ensures user data privacy using encryption techniques.  
  - Uses local binary pattern-based feature extraction.  

---

## *System Architecture*
The system is divided into two phases:

1. *Local System (Admin Side)*
   - Converts color images to grayscale.  
   - Encrypts images using *Bit Plane Randomization on MSB*.  
   - Extracts key points using *Difference-of-Gaussian (DoG)*.  
   - Constructs *Local Binary Pattern (LBP) histograms*.  
   - Transfers encrypted images and feature vectors to the cloud.  

2. *Cloud Server (Retrieval Side)*
   - Accepts query images from the user.  
   - Encrypts query images and extracts features.  
   - Compares extracted features with stored encrypted images.  
   - Returns the best-matching images based on similarity.  

---

## *Technologies Used*
### *Programming Languages:*
- *Python* (Main programming language)
- *HTML* (Web-based interface)
- *PHP* (For server-side communication)
- *MySQL* (Database for storing metadata)

### *Libraries Used:*
- *OpenCV* (Image processing and feature extraction)
- *NumPy* (Numerical computing)
- *Matplotlib* (Visualization)
- *Pillow (PIL)* (Image handling)

### *Cloud Services:*
- *Amazon EC2* (Cloud computing service for image retrieval)

---

## *Setup and Installation*
### *1. Install Dependencies*
sh
pip install opencv-python numpy matplotlib pillow


### *2. Run the Local System (Admin)*
- Convert images to grayscale.
- Encrypt images using the provided script.
- Generate feature descriptors and store them in a CSV file.
- Upload encrypted images and the CSV file to the cloud.

### *3. Run the Cloud Server*
- Accept query images from users.
- Extract query image features.
- Compare query features with the stored image database.
- Retrieve and display similar images.

---

## *How It Works*
1. *User uploads an image to search for similar images.*
2. *The system encrypts and processes the query image.*
3. *Features are extracted and compared with the encrypted image database.*
4. *The most similar images are retrieved and displayed to the user.*

---

## *Future Enhancements*
- Extend support for *color image retrieval*.
- Improve encryption efficiency to *reduce processing time*.
- Use *deep learning-based feature extraction* for better accuracy.
- Optimize system for *real-time image retrieval*.

---

## *Contributors & Acknowledgments*
We would like to express our gratitude to:  
- *Dr. Aruna Rao S L* (Professor & HoD, IT Department)  
- *Dr. K.V.N. Sunitha* (Principal, BVRIT Hyderabad)  
- Faculty members and fellow students for their support.

---

## *License*
This project is for educational and research purposes only. Unauthorized distribution or commercial use is prohibited.

---
