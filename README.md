import cv2

# Read the image
img = cv2.imread("image.jpg")

# Check if the image is loaded
if img is None:
    print("Image not found!")
else:
    # Apply Gaussian Blur
    blurred = cv2.GaussianBlur(img, (15, 15), 0)

    # Display original and blurred images
    cv2.imshow("Original Image", img)
    cv2.imshow("Blurred Image", blurred)

    cv2.waitKey(0)
    cv2.destroyAllWindows()
    
