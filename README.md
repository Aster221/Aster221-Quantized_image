
from PIL import Image

import matplotlib.pyplot as plt


image_path = '1.png'

image = Image.open(image_path)

quantized_image = image.quantize(colors=16)


plt.figure(figsize=(12, 6))

plt.subplot(1, 2, 1)

plt.title('Original Image')

plt.imshow(image)

plt.axis('off')

plt.subplot(1, 2, 2)

plt.title('Quantized Image (16 Colors)')

plt.imshow(quantized_image)

plt.axis('off')

plt.show()

quantized_image.save('2.png')

<div align="center">
  <img src="Q1.jpg" />
</div>
