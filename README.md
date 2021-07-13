# Image-Steganography
Task 2 – Image Steganography

Steganography refers to the method of hiding data inside any form of digital media such as audio, video, image, etc. 
The most basic image steganography technique is based on the Least Significant Bit (LSB) encoding. 
The idea behind this technique is that any modification in the LSB bitplane of the image will not be much perceptible by the human visual system. 
The general process for LSB based image steganography includes bitplane slicing of the image and gathering the LSB bitplane, then inserting the ASCII code of the message into this bitplane.


You are given input images numbered from 00 to 99, here. Each of them is an 8-bit grayscale 256x256 pixels image. Each image contains a unique, meaningful textual message encoded in the LSB bitplane, using slightly different strategies and sentinel values. In this Excel file, check the sentinel value and encoding strategy for the input images. Your task is to implement a decoder for the given image and extract the hidden message. As the output of your program, the hidden text message in the image should be printed. 

You will select one of the images as input, according to your student ID as follows:
• If you are doing the homework individually, you will select the image based on the last two digits of your student ID. (i.e., if your student ID is 123456789, you will use input image 89.tif)
I used input image 68.tif
• If you are doing the homework in pairs, you can select one of the two alternatives in this way: Assume that student ID1 is 123456789 and student ID2 is 987654321, you can select 91.tif or 19.tif as the input image.
The text messages are encoded in the LSB bitplane of the images, using different sentinel values and encoding strategies, as stated in the Excel file. Sentinel character is used to indicate the end of the secret message. In this assignment, eight different encoding strategies, Strategy0 through Strategy 7, were employed. These strategies are explained with an example below. Assume that we have an 8-bit 10x5 pixels grayscale image and we want to encode text message “msg” in the LSB bitplane of this image. For this example, we will use “#” character as the sentinel value, to indicate the end of the message. We use the binary ASCII codes of each character in the message, as shown in the below table. The encoding procedure for each strategy is illustrated in Figure 2. For each strategy, LSB bitplane is shown and X symbols in the figure correspond to “don’t care”.
![image](https://user-images.githubusercontent.com/72042095/125511297-067b95f2-c7eb-46bc-87d5-d63847567a8c.png)
