# Feature_detection-Image-processing
In PC vision and picture handling highlight discovery incorporates techniques for figuring deliberations of picture data and settling on nearby choices at each picture point whether there is a picture highlight of a given kind by then or not. The subsequent highlights will be subsets of the picture space, frequently as segregated focuses, constant bends or associated regions.Feature identification is a low-level picture preparing activity. That is, it is typically proceeded as the primary procedure on a picture, and analyzes each pixel to check whether there is an element present at that pixel. On the off chance that this is essential for a bigger calculation, at that point the calculation will commonly just look at the picture in the district of the highlights. As an underlying pre-essential to highlight identification, the info picture is typically smoothed by a Gaussian bit in a scale-space portrayal and one or a few component pictures are figured, regularly communicated as far as nearby picture subsidiaries activities. 

- <b>Example of Corner Detection</b> <br />

` I = imread('circuit.tif'); 
corners = detectFASTFeatures(I,'MinContrast',0.1);
J = insertMarker(I,corners,'circle'); 
imshow(J) `

<img align="right" width="250" height="300" src="https://www.mathworks.com/help/vision/ug/feature_detection_corner.png">
- <b>What Makes a Good Local Feature?</b>
<br>
Detectors that rely on gradient-based and intensity variation approaches detect good local features. These features include edges, blobs, and regions. Good local features exhibit the following properties:
<br>
<b>Repeatable detections:</b>
<br>
When given two images of the same scene, most features that the detector finds in both images are the same. The features are robust to changes in viewing conditions and noise.

<b>Distinctive:</b>
<br>
The neighborhood around the feature center varies enough to allow for a reliable comparison between the features.
<b>Localizable:</b>
The feature has a unique location assigned to it. Changes in viewing conditions do not affect its location.
