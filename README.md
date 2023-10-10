# SudheeshWAPerceptions
Perceptions challenge answer
For this challenge, I took the route of splitting the image into two regions and then using colors to detect the cones.
I decided to use opencv to load the image, detect boundaries/contours of colors, and draw the lines saving it onto a new file.
I used numpy to hold some form of mathematical standard for the colors and drawing the lines.

Stackoverflow and chatgpt helped me understand the use of centroids and calculating a line based on a set of points.
I was stumped by how we could avoid calculating the door or the reflection of the exit sign on the floor, since they are also slightly red, like the cones.
In this situation, however, I was able to use chatgpt and stackoverflow to understand how RGB colors and tolerance could work. Additionally, they helped me develop code that is able to filter out insignificant points that are red, but not directly in the path of the cones.
Then using centroids that chatgpt helped find, and splitting the image into two halves, I was able to divide the image and focus on each set of cones seperratly. Then I essentially tried to find the best fit line, and to implement a linear regression calculation, I was able to use stack overflow.

Finally, I wrote the line onto the image: (I hope this shows)
![image](https://github.com/sudthepud/SudheeshWAPerceptions/assets/43526655/b973148e-d6f8-4a95-ab10-d9b3278a3564)
.

