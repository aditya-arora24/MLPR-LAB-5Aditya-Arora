## MLPR-LAB-5Aditya-Arora
lab 5 mlpr
# Aim
The primary objectives of this lab are to:

Detect faces in an image using Haar Cascade classifiers

Extract color features (Hue and Saturation) from detected faces

Apply K-Means clustering to group faces based on their color characteristics

Classify a template image into one of the identified clusters

Visualize the clustering results with centroids and data points

# Methodology
1. Face Detection

Load the input image (plaksha_Faculty.jpg)
Convert to grayscale for face detection
Apply Haar Cascade classifier to detect facial regions
Draw bounding boxes and labels on detected faces

2. Feature Extraction

Convert the original image to HSV color space
Extract mean Hue and Saturation values for each detected face
Store these features as 2D data points

3. K-Means Clustering

Apply K-Means algorithm with k=2 clusters
Group faces based on similarity in Hue-Saturation space
Calculate cluster centroids

4. Template Classification

Load template image (Dr_Shashi_Tharoor.jpg)
Extract Hue-Saturation features
Predict which cluster the template belongs to using the trained K-Means model

5. Visualization

Create scatter plots showing cluster assignments
Display centroids and template image position
Use face thumbnails as markers for enhanced visualization

# Key Findings
The face detection algorithm successfully identified multiple faces in the faculty image using the Haar Cascade classifier. Bounding boxes with labels were accurately placed on each detected face, demonstrating the robustness of this approach for frontal face detection.
The K-Means clustering analysis revealed that faces could be successfully grouped into two distinct clusters based on their skin tone characteristics in the Hue-Saturation color space. Cluster 0 (green) and Cluster 1 (blue) showed clear separation, indicating that color-based features provide meaningful information for grouping faces with similar characteristics.
The cluster centroids, marked with black and yellow X markers, represent the average Hue-Saturation characteristics of each group. These centroids serve as reference points for classifying new faces and demonstrate how K-Means identifies the most representative color characteristics for each cluster.
The template image classification demonstrated practical applicability of the trained model. The template was successfully classified into one of the two clusters based on its proximity to the cluster centroids using Euclidean distance. The violet marker shows the template's position in the feature space, confirming that distance-based classification can effectively assign new faces to appropriate groups.






# Conclusions

Face Detection: Haar Cascade classifiers are effective for frontal face detection with proper parameter tuning.

Feature Selection: Hue and Saturation provide meaningful features for skin tone-based clustering, as they are relatively invariant to lighting changes.

Clustering Performance: K-Means successfully groups faces into distinct clusters based on color characteristics, demonstrating the effectiveness of distance-based classification.

Template Classification: The trained model can accurately classify new faces into existing clusters, showing practical applicability for face grouping tasks.

Visualization: Scatter plots with face thumbnails provide intuitive understanding of cluster distributions and decision boundaries.



<img width="1576" height="1000" alt="image" src="https://github.com/user-attachments/assets/6a2c212b-cdf9-4f2f-8738-63ad4d344ca7" />

<img width="1135" height="627" alt="image" src="https://github.com/user-attachments/assets/2971c310-4f30-4e51-b457-1c711f562aaa" />

<img width="492" height="494" alt="image" src="https://github.com/user-attachments/assets/39fe937c-1865-4b34-91ff-1a094af4da72" />

<img width="1134" height="618" alt="image" src="https://github.com/user-attachments/assets/64221631-a707-4a05-986e-2cb3ba82a0b7" />

<img width="939" height="779" alt="image" src="https://github.com/user-attachments/assets/d56d28a9-47a2-4672-9a5a-52e93c715019" />

