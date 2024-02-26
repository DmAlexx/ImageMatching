Questions
1. The affine transform does not seem to be working well in this case. Why?
   - the affine transform may not work well in this case because it assumes a linear mapping between the source and destination points.
   - on this image we have non-parallel vertical lines at a significant angle.
     
3. What can you tell me about the values you have obtained for the inliers vector? What does it mean?
   - The function estimateAffine2D() returns two values: the affine transformation matrix and an array containing binary values of 0 and 1,
   - indicating the internal (1) and external (0) points, determined by the algorithm RANSAC. So we understand which points belong
   - to the background and which ones belong to the transformed area.
     
5. How does the result from homography look? Does it work well enough?
   -The result from homography looks quite good for a document with non-parallel lines.
