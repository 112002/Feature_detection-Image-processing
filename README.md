# Feature_detection-Image-processing
In PC vision and picture handling highlight discovery incorporates techniques for figuring deliberations of picture data and settling on nearby choices at each picture point whether there is a picture highlight of a given kind by then or not. The subsequent highlights will be subsets of the picture space, frequently as segregated focuses, constant bends or associated regions.Feature identification is a low-level picture preparing activity. That is, it is typically proceeded as the primary procedure on a picture, and analyzes each pixel to check whether there is an element present at that pixel. On the off chance that this is essential for a bigger calculation, at that point the calculation will commonly just look at the picture in the district of the highlights. As an underlying pre-essential to highlight identification, the info picture is typically smoothed by a Gaussian bit in a scale-space portrayal and one or a few component pictures are figured, regularly communicated as far as nearby picture subsidiaries activities. 

- Example of Corner Detection <br />

` I = imread('circuit.tif');
corners = detectFASTFeatures(I,'MinContrast',0.1);
J = insertMarker(I,corners,'circle');
imshow(J) `


