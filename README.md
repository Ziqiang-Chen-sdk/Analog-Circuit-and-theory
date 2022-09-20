# Analog Circuit and Theory

This repository contains the following MATLAB live script files, Each script gives an indepth description of an analog circuit design theory:

### 1. Broadband_matching_lumped_filter_network:
Simple two-element and quarter-wave impedance matching can deliver perfect power transfer at a single frequency. However, its bandwidth is limited. Limited bandwidth reduces the ability to transmit signals with broader bandwidth, such as a pulse. The algorithm presented here provides a systematic method to generate an impedance matching system with any desirable gain and bandwith tradeoff constrained by the Fano-Bode criterion. The shape of the pass band is carefully defined using traditional filter design methods such as Butterworth and Chebyshev's approximation. The designed filter network is then synthesized using Cauer Form 1

### 2. Broadband_matching_distributive_filter_design_method
Similar to the script above, This algorithm also present a systematic method to obtain a impedance matching system that allows any desirable gain and bandwith tradeoff constrained by Fano-Bode criterion. The difference is that impedance function is synthesized using Richard transform resulting in dirtributive network instead of lumped network. Distributive networks matching are better suited for matching with the wave length of the frequency of concern is small compare to the designated footprint. meaning this is useful at high frequency or mechanical impedance matching for ultrasound

### 3. Noise_analysis_TIA_vs_VA 
Highspeed TIA using opamp migh be difficult, this is because highspeed opamps are commonly JFET or BJT input, whcih have a high current noise. This input refered current noise usually increases linearly after 1-100Mhz depend on the opamp. This code explaines the procedures necessary to calculate the output referred noise and noise figure for a given TIA or VA design. Note: When choosing TIA vs VA designs, noise contribution should not be the sole consieration. 

### 4. Transmission_line_effect_of_arbitrary_signal
Impedance matching can be costly to implement, when only voltage or current signal is of concern, it is important to un-
derstand the level of signal distortion before implementing impedance matching. This algorithm outputs a resulting time domain signal after an arbitrary signal, has passed through an arbitrary transmission line with arbitrary termination impedance.
