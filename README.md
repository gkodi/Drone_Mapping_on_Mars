## Mapping paleolacustrine deposits with a UAV-borne multispectral camera: Implications for future drone mapping on Mars.

NASA’s Ingenuity Mars Helicopter has ushered in a new era in planetary exploration by utilizing Unmanned Aerial Vehicles (UAVs) to enhance our understanding of planetary surfaces. This project evaluates the potential of UAVs for mapping Martian environments, using Lake Natron, Tanzania, as an analog for Martian paleolakes.

During two field seasons (January and July 2023), we employed a Phantom 4 Pro drone equipped with a MicaSense RedEdge-M multispectral camera and a TerraSpec Halo VNIR-SWIR spectrometer to capture high-resolution imagery and spectral data. Almost all image processing and analysis were performed using Python scripting, except for image mosaic and Digital Elevation Model (DEM) generation.

We benchmarked the onboard image processing capabilities using a Raspberry Pi 5 single-board computer. 

In this repository, we share all the code developed during our study. Processing steps include,
1. DN to radiance conversion
2. Panel radiance extraction
3. Calculate reflectance factors using DLS data
4. Calculate reflectance at MicaSense band
5. Convert radiance to reflectance using 1 point empirical line method (1p ELM)
6. Convert radiance to reflectance using 2 point empirical line method (2p ELM)
7. Atmospheric correction using 6SV method
8. Convert radiance to reflectance using DLS data
9. Calculate Band indices
10. Weighted Kmean clustering
11. Finding the optimal number of clusters using the elbow method
12. Cmean clustering

We also included sample image data used in the study. Feel free to contact us for more information/data.

