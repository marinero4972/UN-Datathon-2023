# UN-Datathon-2023
Calculating area of rooftops

# Introduction
Buildings are important carriers for the construction of distributed photovoltaic facilities. A very important factor in determining the development potential of distributed photovoltaics in a region is the roof area. They are of extremely important value for the calculation of photovoltaic power generation and final benefits.
For area measurement, we thought of applying computer vision methods to remote sensing maps, and finally proposed an urban roof area measurement method based on a remote sensing image segmentation model, which can yield more accurate results.
Driven by large models, artificial intelligence has developed rapidly this year. Especially after the Segment Anything model was proposed, many influential works appeared in the field of image segmentation. The AIE-SEG model we use is the latest large-scale remote sensing AI segmentation model released by Alibaba Damo Academy last month. It can quickly identify nearly a hundred types of remote sensing features such as farmland, water bodies, and buildings.
In this method, we first segment the area of the target city in Amap or Google Maps and download it as an image in TIFF format. Next, we used the AI-Earth platform to segment the built-up areas of the target city using the AIE-SEG model. In the end, the total area of the rooftops is the sum of the areas of the divided patterns. 

# Requirements
numpy
aie

# Platform
We run our code on AI Earth's platform. [AI Earth](https://engine-aiearth.aliyun.com/)

# Data
Our data is from Google Map and Amap.
