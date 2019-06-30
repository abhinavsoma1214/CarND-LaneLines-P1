The goals of this Finding-Lanes project is that:
Make a pipeline that finds lanes on the road
Compile all the images to form a lane detection algorithm which detects lanes in the given video
To write a writeup of the steps I took to get the end result 

All the code is available in lane-linecode.ipynb

Describe the Pipeline:
I imported the image to be read 
1) Then I turned that colored image into a grayscale image version of it
2)  After I converted the image to a greyscale version of it, I turned it into a GaussianBlur. The GaussianBlur allowed for everything execpt the lane line to be present, highlighting the lane lines and blurring environment around the lane lines
3) After I converted the image into a GaussianBlur into an Canny Edge Detection. Canny Edge Detection is a filter where it highlights the lane lines and muting out the environment.
4) After I converted the image into Canny Edge Detection, I defined the region of interest. The region of interest is a space in the Canny Edge Dectection where I, with some help from Vuiseng9, adapted some of his code into my algorithm to suit my purpose of using it to specify this area as a region of interest. This means with the use of the already defined Canny Edge Detection image that I created earlier and OpenCV will use matplotlib to better classify the region that needs to be isolated and outlined for the cameras to follow.
5) After creating the region of interest from the Canny Edge Detection version of the solidYellowLeft.jpg, with the help of Vuiseng9, I adapted his version of the code into my algorithm where it blended the two images, the region of interest and solidYellowLeft.jpg, due to this blending lines will be better defined and the image would be a little darker.
6) Then I created a pipeline where all of the images are compiled with the help of liferlisiqi and then create a video of it. I then translated this pipeline into video format to compile the images into one successful video with lane line detection.
Results & Reflection: The results of the first project is that I have created a project from an image to a video which is a compilation of images. I believe that I have created that with the end result of my project which I have been working very hard on. I can't forget two sources where I got most of my direction from and it would be plagerism if I did not include them in my works cited and that is Vuiseng9 & liferlisiqi. I believe that not only did I complete the project but I have completed it with the best of my ability trying to learn things on the fly.
Potential Shortcomings:
The lane lines
The time that it took to submit the project
The color of the lane lines that are being tracked are not in the colors that would be best suited for the effectiveness of reading the lane lines.
Potential Improvements:
I can finish my projects faster 
Condense my code shorter than my first project
Resources that I have adapted into my code:
https://github.com/vuiseng9/SDCND-P001-Finding-Lane-Lines
https://github.com/liferlisiqi/Finding-Lane-Lines

MLA Citation:
vuiseng9. “vuiseng9/SDCND-P001-Finding-Lane-Lines.” GitHub, github.com/vuiseng9/SDCND-P001-Finding-Lane-Lines.
Liferlisiqi. “Liferlisiqi/Finding-Lane-Lines.” GitHub, 2 Jan. 2018, github.com/liferlisiqi/Finding-Lane-Lines.