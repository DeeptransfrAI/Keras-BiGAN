# Keras-BiGAN
BiGAN implementation in Keras to detect similarities in Landscapes.


![alt text](https://i.imgur.com/owXSkXf.png)
Detecting feature-wise similarity of landscape images.
Left is the target, and right are the most similar images in the dataset (in order).


![alt_text](https://i.imgur.com/wgiKuiK.png)
Clusters created from BiGAN's feature space, using k-means clustering. Each row is another cluster.


![alt_text](https://i.imgur.com/lcUzGZk.png)
Images generated by this BiGAN.
Top are generated from nothing. Bottom shows real images (1st and 3rd row) and their respective reconstructions (2nd and 4th row).


To use:
- Create 3 directories: "data", "Results", "Models"
- In data, create a folder with the images.
- Specify training details in bigan.py
- Train BiGAN using bigan.py
- Make predictions using the functions in guess.py

guess.py also includes a "game" which will try to guess how you rate images in a dataset, using Inverse Distance Weighting in BiGAN's feature space.

Enjoy!
