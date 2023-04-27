# Sandstone Microstructure Segmentation With Attention U-Net
<p align="center">
</p>
<img src="https://interminerals.com/images/aggregates/_1200x630_crop_center-center_82_none/Jura-2.jpg?mtime=1553560515">
<p>Sandstone is a clastic sedimentary rock composed mainly of sand-sized (0.0625 to 2 mm) silicate grains. It comprises about 20–25% of all sedimentary rocks. In this project, I have trained the Attention U-Net deep learning model for performing image segmentation of XRM (tomography) scan of a sandstone cylinder of size about 2 mm
diameter to identify the regions of clay, quartz, air, and pyrite. </p>
<h2>Libraries Used</h2>
<ul>
  <li>Tensorflow</li>
  <li>Numpy</li>
  <li>Pandas </li>
  <li>Matplotlib</li>
  <li>Seaborn</li>
  <li>Sklearn</li>
</ul>
<h2>Dataset Visualization</h2>
<p align="center">
<img src="https://github.com/NavinBondade/Sandstone-Microstructure-Segmentation-With-Attention-U-Net/blob/main/Graphs/dataset_gist_ncar.png" width="750" height="500">
</p>
<h2>Segmentation Regions Visualization</h2>
<p align="center">
<img src="https://github.com/NavinBondade/Sandstone-Microstructure-Segmentation-With-Attention-U-Net/blob/main/Graphs/dataset_Background_Air.png" width="750" height="500">
</p>
<p align="center">
<img src="https://github.com/NavinBondade/Sandstone-Microstructure-Segmentation-With-Attention-U-Net/blob/main/Graphs/dataset_Clay.png" width="750" height="500">
</p>
<p align="center">
<img src="https://github.com/NavinBondade/Sandstone-Microstructure-Segmentation-With-Attention-U-Net/blob/main/Graphs/dataset_Pyrite.png" width="750" height="500">
</p>
<p align="center">
<img src="https://github.com/NavinBondade/Sandstone-Microstructure-Segmentation-With-Attention-U-Net/blob/main/Graphs/dataset_Quartz.png" width="750" height="500">
</p>
<h2>What is Attention U-Net?</h2>
<p>Attention is an important aspect of any computer vision task where we need to focus on specific regions in an image. Regarding image segmentation, attention is a massive help in highlighting the important regions of the image. Due to this the model converges much faster and has better generalization capabilitie</p>
<p>Here in Attention UNET, the author proposes a novel spatial attention mechanism called Attention Gate (AG). The Attention Gate helps to focus on target structures of varying shapes and sizes in medical images.The models trained with Attention Gate implicitly learn to suppress irrelevant regions in an input image while highlighting salient features useful for a specific task. This enables us to eliminate the necessity of using any explicit localization modules.</p>
<p>The Attention Gate can be easily integrated into any existing segmentation architecture such as U-Net with a minimal increase in the parameters. This increase in parameters boosts the model’s sensitivity and accuracy.</p>
<h2>Model Details</h2>
<p>The model has been trained on a sandstone microstructure dataset for 150 epochs. The model used categorical cross entropy as a loss function since it's a muti-class segmentation problem. Stochastic gradient descent has been used as the optimizer.</p>
<h2>Model Architecture</h2>  
<p align="center">
<img src="https://github.com/NavinBondade/Sandstone-Microstructure-Segmentation-With-Attention-U-Net/blob/main/Graphs/model_architecture.png">
</p>
<h2>Model Architecture</h2>  
<p align="center">
<img src="imagelink">
</p>
<h2>Model Training & Testing</h2>   
<p>On the training dataset, the loss was 0.0356, the accuracy was 98%, and the IoU score was 0.5747. Whereas on the testing dataset, the loss was 0.1106 the accuracy was 97%, and the IoU score was 0.6065.</p>
<h4>Model Loss:</h4>   
<p align="center">
<img src="https://github.com/NavinBondade/Sandstone-Microstructure-Segmentation-With-Attention-U-Net/blob/main/Graphs/Loss.png" width="1000" height="400">
</p>
<h4>Model Accuracy:</h4>  
<p align="center">
<img src="https://github.com/NavinBondade/Sandstone-Microstructure-Segmentation-With-Attention-U-Net/blob/main/Graphs/Accuracy.png" width="1000" height="400">
</p>


