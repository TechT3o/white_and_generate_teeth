# Whiten and generate teeth

In this repo you can find the [google colab notebook](https://colab.research.google.com/drive/1TvhI0dULkjPITJUxOMW7u8dPnukTK5H_?usp=sharing) that includes the code to perform automatic teeth whitening in cases fo yellow teeth and teeth generation in cases of missing teeth in head portrait images of people.

## Teeth Whitening

Firstly the landmarks of the inner lips are found to get the region where the teeth should be found. Then HSV color filtering is performed to remove the gums and tongue and keep only the teeth. Then the image is converted to the LAB colorspace, the yellow pixels are found and are desaturated to become white. This can be seen below:
![whiten_teeth](https://github.com/TechT3o/whiten_and_generate_teeth/assets/87833804/44b1023b-9387-4fba-987a-ce4b0c32fe94)

## Teeth Generation

Firstly the landmarks of the inner lips are found to get the region where the teeth should be found. Then this mask is used along with Stable Diffusion with inpainting to generate teeth inside the mouth region on top of the original image. This functionality is shown below:

![missing_teeth](https://github.com/TechT3o/whiten_and_generate_teeth/assets/87833804/d74f5155-74dd-4f6f-b6bb-a8556f06386b)
