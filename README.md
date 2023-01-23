Part I
Read the grayscale image called test.jpg
Write your own code to compute a 64-bin gray scale histogram of the image. You cannot use built in histogram functions from any library (e.g. numpy.histogram, scipy.stats.histogram, skimage.exposure.histogram, opencv.calcHist, etc) for this.
Plot the histogram.
Also, call Numpy histogram function to compute 64-bin histogram for the same image. Plot it side by side with yours to show that they are identical.
Expected output:



Part II

Complete function part2_histogram_equalization() to perform a 64-bin grayscale histogram equalization on the same test.jpg image used in the last part. You need to plot the original image, its 64-bin histogram, the image after histogram equalization, and its 64-bin histogram. 

You are not allowed to use the Skimage functions, i.e., exposure.histogram, exposure.equalize_hist, or any equivalent functions from any other library for this part.

Tutorials on histogram equalization:

https://www.youtube.com/watch?v=GWCB3pKi2ko

https://www.tutorialspoint.com/dip/histogram_equalization.htm

https://en.wikipedia.org/wiki/Histogram_equalization

Expected output:



Part III

Complete function part3_histogram_comparing() to compare the 256-bin histograms of two images day.jpg and night.jpg. You will need to read both images, convert them to grayscale, compute their 256-bin histograms and print the Bhattacharyya Coefficient of the two histograms. 

You can use numpy histogram function to compute these histograms.

Expected output:

Bhattacharyya Coefficient: 0.8671201323799057



Part IV 

Complete function part4_histogram_matching() to match the histograms of the same two images day.jpg and night.jpg from part 3. 

You need to implement the algorithm given on the last page of the histogram equalization example on eclass

You can use numpy histogram function to compute the histograms.

(a) (30%) Grayscale:

Read both images, convert them to grayscale, and match the 256-bin histogram of the day image to that of the night image to generate a new grayscale image that should be a darker version of the day image. Show the grayscale day, night, and matched day images side by side.

(b) (10%) RGB: 

Repeat the grayscale histogram matching process from part (a) with each channel of the two images and put together the resultant matched channels into a new RGB image. You can also use the single-intensity mapping obtained from the grayscale images in (a) to match each of the three channels as suggested in the third tutorial below. Show the RGB day, night, and matched day images side by side.
