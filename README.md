# Analog Circuit and Theory

This repository contains the following MATLAB live script files, Each script gives an indepth description of an analog circuit design theory:

### 1. Broadband_matching_lumped_filter_network:
Simple two-element and quarter-wave impedance matching can deliver perfect power transfer at a single frequency. However, its bandwidth is limited. Limited bandwidth reduces the ability to transmit signals with broader bandwidth, such as a pulse. The algorithm presented here provides a systematic method to generate an impedance matching system with any desirable gain and bandwidth tradeoff constrained by the Fano-Bode criterion. The shape of the pass band is carefully defined using traditional filter design methods such as Butterworth and Chebyshev's approximation. The designed filter network is then synthesized using Cauer Form 1.

### 2. Broadband_matching_distributive_filter_design_method
Similar to the script above, This algorithm also presents a systematic method to obtain an impedance matching system that allows any desirable gain and bandwidth tradeoff constrained by the Fano-Bode criterion. The difference is that the impedance function is synthesized using the Richard transform, resulting in a distributive network instead of a lumped network. Distributive network matching is better suited for matching with the wavelength of the frequency of concern is small compared to the designated footprint. Meaning this is useful at high frequency or mechanical impedance matching for ultrasound applications.

### 3. Noise_analysis_TIA_vs_VA 
High-speed TIA design using opamp might be difficult. This is because high-speed opamps are commonly JFET or BJT input, which have a high input-referred current noise. Depending on the opamp, The input-referred current noise usually increases linearly after 1-100Mhz. This code explains the procedures necessary to calculate the output referred noise and noise figure for a given TIA or VA design. Note: When choosing TIA vs VA designs, noise contribution should not be the sole consideration; this script does not take care of this aspect. 

### 4. Transmission_line_effect_of_arbitrary_signal
Impedance matching can be costly to implement. When only voltage or current signal is of concern, it is important to understand the level of signal distortion before implementing impedance matching. This algorithm outputs a resulting time domain signal after an arbitrary signal has passed through an arbitrary transmission line with arbitrary termination impedance.
