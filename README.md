# SudheeshWAPerceptions
Perceptions challenge answer.
For this challenge, I took the route of depending on the colors of the cones to detect them.
I used opencv to load the image, detect boundaries/contours of colors, and draw the lines and saving it onto a new file.
I used numpy for operations on the colors and other mathematical operations in the solution, which was discovered through stack overflow.

Stackoverflow helped me understand how i could find the cones using colors and assign points to the cones once finding them, and storing their centers with the term of centroids, and calculating a line based on a set of points.
I was stumped by how i could avoid calculating the door or the reflection of the exit sign on the floor, since they are also slightly red, like the cones.
In this situation, however, I was able to use stackoverflow and also chatgpt to understand how RGB colors and tolerance could work. Additionally, they helped me develop code that is able to filter out insignificant points that are red, but not directly in the path of the cones. Essentially, i was able to not count the points that were not going to contribute towards a line, like the door and the exit sign which went out of the way of the points for the cones.
Then using the array of points for each set of cones on each half, i was able to focus on each set of cones seperratly. Then I essentially tried to find the best fit line, and to implement a linear regression calculation, I was able to use stack overflow. This worked because the points were not perfectly straight, since the cones werent in a straight line meaning center of those cones were not in a straight line. Therefore finding the best fit line was necessary. Lastly I used opencv to write those lines on and stored the image.

Finally, I wrote the lines onto the image: (I hope this shows)
![image](https://github.com/sudthepud/SudheeshWAPerceptions/assets/43526655/b973148e-d6f8-4a95-ab10-d9b3278a3564)
.

