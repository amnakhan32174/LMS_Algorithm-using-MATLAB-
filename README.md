# LMS_Algorithm-using-MATLAB-

This experiment implements an adaptive noise cancellation system using the Least Mean Squares 
(LMS) algorithm in MATLAB. The objective was to develop a filter capable of adapting in real 
time to minimize noise from a corrupted input signal. A clean sine wave was artificially 
corrupted with additive white Gaussian noise. A known FIR filter was used to simulate a system 
that produces the desired output. An adaptive LMS filter with a fixed number of taps was then 
trained to minimize the error between its output and the desired signal. Performance was 
evaluated using Mean Square Error (MSE) tracking and a confusion matrix comparing clean and 
noisy detections. The results showed a significant reduction in MSE, indicating effective noise 
suppression. Various plots such as error vs iteration, signal comparisons, and error analysis 
before and after filtering supported the findings. The LMS filter successfully tracked the signal 
with minimal lag and converged within acceptable limits. This work demonstrates the 
practicality of adaptive filtering for real-time noise reduction in signal processing applications.
