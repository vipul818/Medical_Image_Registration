# Medical Image Registration
![Screenshot from 2022-12-23 18-56-57](https://user-images.githubusercontent.com/72666431/209343655-947a78e6-911c-4519-a4a8-9cae5d8af1b1.png)

<p>This project is about performing image registration on whole slide images.
  
Image registration is the process of transforming different images of one scene into the same coordinate system.Image registration has a wide variety of applications: it is essential as soon as the task at hand requires comparing multiple images of the same scene. It is very common in the field of medical imagery, as well as for satellite image analysis and optical flow.</p>
<p> Features:
  <ol>
  <li>Image registration for whole slide images in cancer imaging.</li>
  <li>Used SIFT feature for key point detection and registration via OpenCV.</li>
</ol>
</p>



## 1. Create thumbnail of the image
<p>Since WSIs( whole slide images) can be very large in size(can go upto some gigabytes) it is difficult to read and explore their features. This can be done using <strong>openslide</strong>( Python library).
It can be installed using the following command:</p>

`pip install openslide-python`

<p>For creating the thumbnail, we will: 
<ol><li> Import required packages and functions
<li> Read the image and explore the properties of it
<li> Display the image 
</ol></p>
 <a href="https://github.com/vipul818/Medical_Image_Registration/blob/main/create_thumbnail.ipynb">Notebook for Creating thumbnail</a>


## 2. Perform SIFT operation
<p>SIFT (Scale-invariant feature transform) is the original algorithm used for keypoint detection.
For performing image registration, we will:
<ol><li> Import the required packages and functions
<li> Create rotate image function
<li> Create the SIFT function
<li> Apply the created functions over the thumbnails
</ol>
</p>
<a href="https://github.com/vipul818/Medical_Image_Registration/blob/main/Image_Registration.ipynb">Notebook for performing SIFT operation</a>
