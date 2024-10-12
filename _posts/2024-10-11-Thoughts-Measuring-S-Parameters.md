# Thoughts on measuring S-Parameters

# Definition of S-Parameter
(discussed later)

# Measuring S-Parameters using VNA
I. Passive Device

II. Active Device
1. Question: What would happen on the measured $$S_{11}$$ if a 10-dB attenuator is attached to the device's input?
Definition: $$ S_{11} = \frac{V^{-}}{V^{+}} $$, reflected voltage over the incident voltage. $$ P^{-} = |\Gamma|^{2} P^{+} $$. Here, $$ \Gamma = S_{11} $$.
Assuming the device provides 0 dBm of output power, and the $$ \Gamma = 12 dB $$. Upon passing the 10 dB attenuator, the incident power is -10 dBm. Here comes the tricky part: how do we deal with the squared $$ \Gamma $$ in the dB-scale? Let's remind ourselves of how to convert linear scale to dB scale: $$ \Gamma_{dB} = 20 log_{10} {\Gamma} = 20 log_{10} \frac{V^{-}}{V^{+}}.
