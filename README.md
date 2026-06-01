# Audio Analysis Using Fourier Transform with Vivaldi’s Winter
This demonstrates the effect of a Low-Pass Filter and demonstrate how a filtering system can effectively isolate and process two distinct tracks: the live audio and the recording. 

<img width="812" height="592" alt="image" src="https://github.com/user-attachments/assets/e529c480-9f7c-4ee7-ac0c-afe93ff7891b" />

In this experiment, we compare a live version and a studio recording version of the track to analyze their similarities and differences after applying an ideal low-pass filter. The live version exhibits three (3) major dominant frequencies: the tallest peak occurs around 450 Hz with an amplitude of 1.8 x 10-3, followed by a peak at 550 Hz with an amplitude of 1.3 x 10-3, and a final sharp peak at 1100 Hz with an amplitude of 1.5 x 10-3. In contrast, the recording version also displays three major dominant frequencies, which are located at 70 Hz (2.6 x 10-3), 530 Hz (2.3 x 10-3), and 470 Hz (2.1 x 10-3).

To approximate the signal mathematically using its major frequency components in sinusoidal form:

x(t) = A1sin(2f1t)+ A2sin(2f2t) + ... 

For the recording version,
x(t) = (2.6 x 10-3)sin(270t)+ (2.3 x 10-3)sin(2530t) + (2.1 x 10-3)sin(2470t)... 

For the live version,
x(t) = (1.87 x 10-3)sin(2420t)+ (1.74x 10-3)sin(2471t) + (1.56 x 10-3)sin(21070t)... 

The equations for x(t) remain unchanged because the high-frequency interference—which includes background noise and a tiny layer of string friction—is concentrated at 2500 Hz and beyond, where the spikes are very short, saturated, and continuous in the resulting graphs. Since the dominant frequencies used in the approximation are all below this 2500 Hz cutoff, the low-pass filter does not affect the calculation of x(t).

Vivaldi’s Winter is dominated by high-pitched, rapid, and sharp violin sounds, which explains a lot from its title. So, we used a low pass filter as it helps with the separation between the desired musical signal and the unwanted high-frequency interference. The fundamental notes and important lower harmonics of the violin and the deep rhythm of the bass instruments are all seen in the lower frequency spectrum below 2500 Hz. On the other hand, the harsh string friction is concentrated across the upper spectrum which is above 2500 Hz. By having a low-pass filter the important low to middle frequencies are allowed to pass through not attenuated within the filter's passband, preserving the bright and high quality clarity, and cohesive orchestral sound. And, the result is demonstrated further using Matlab.
