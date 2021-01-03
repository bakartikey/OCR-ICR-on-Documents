OCR/ICR on documents

Objective:

The goal is to find an algorithm that can extract the maximum information from a given page

I broke the process in to the following 6 steps:

1. Character isolation
2. Noise reduction
3. Boundary removal
4. Normalising
5. Thinning
6. Feature extraction

Challenges:

There were many challenges to overcome.
1. Black Border Removal
2. ICR (Intelligent Character Recognition): recognize and convert hand-drawn characters into text
3. Scanned page (Detect edges and apply a perspective transform to obtain the top-down view of the document)
4. Remove noise
5. Shape detection and extraction
6. OCR
7. Handwriting recognition
8. Minimize errors
But the main problem was to “identify which part of the form contains text”.

My Approach

Input image
   ||
   \/
Detecting orientation of Image
   ||
   \/
Detecting and fixing skew angle
   ||
   \/
Removing form/table structure
   ||
   \/
Removing noise and making text clearer
   ||
   \/
Applying OCR and handwriting recognition
