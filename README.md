# Image-compression
from PIL import Image

def compress_image(input_image_path, output_image_path, quality=55):
    with Image.open(input_image_path) as img:
        img.save(output_image_path, "JPEG", quality=quality)

# Use raw string for Windows paths
input_image_path = r"C:\Users\anush\OneDrive\Desktop\a.jpg"
output_image_path = r"C:\Users\anush\OneDrive\Desktop\output.jpg"

compress_image(input_image_path, output_image_path)
