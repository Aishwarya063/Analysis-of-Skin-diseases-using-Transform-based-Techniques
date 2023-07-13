# Analysis-of-Skin-diseases-using-Transform-based-Techniques
Software Required: 
MATLAB
PhotoShop
Stage I:
Firstly a 130 images must be collected which consists of various skin diseases with different degrees of infection levels. These 130 images consists of 80 images of database and 50 images of for testing. These images must be copy pasted into new file of Photo shop. All of these images must be normalized to 50*50 matrix in such way that the images are unaffected by skew, rotate, and scale. Images must be named in .tiff form. Using contrast and brightness features we need to adjust the intensity levels of the image. Using minimum rectangle feature all the images must be cropped in order have the exact image, avoiding the wastage around it.

Stage II:
Smallest unit of an image is pixel. FFT/DCT algorithm is used in this. Image which is run through FFT/DCT for loop gives out real and imaginary part and real part is represented in matrix form. This matrix form is first put in Transpose form and later concatenated which results in 2500 elements of an image being arranged in a single column. When a image is put for testing. That image’s 2500 elements are compared with images of database which are divided into 4 groups each consisting of 100 images and Euclidean distance is used to compare each element of testing to each element of image from database. If minimum Euclidean distance if found the images are considered to be matched. 

Stage III:
After the image is run through the FFT/DCT and found it’s match. It is represented using subplot with one side as testing image and other side with matched database image. 

"N" on top of image denotes - Image of normal and healthy skin
"A" on top of image denotes - Image of skin lesion 
