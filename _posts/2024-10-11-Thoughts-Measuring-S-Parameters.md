# Thoughts on measuring S-Parameters

# Definition of S-Parameter
(discussed later)

# Measuring S-Parameters using VNA
I. Passive Device

II. Active Device
1. Question: What would happen on the measured $$S_{11}$$ if a 10-dB attenuator is attached to the device's input?
Definition: $$ S_{11} = \frac{V^{-}}{V^{+}} $$, reflected voltage over the incident voltage. $$ P^{-} = |\Gamma|^{2} P^{+} $$. Here, $$ \Gamma = S_{11} $$. <br>

Assuming the VNA provides 0 dBm of output power, and the $$ \Gamma = 12 dB $$. Upon passing the 10 dB attenuator, the incident power is -10 dBm. Here comes the tricky part: how do we deal with the squared $$ \Gamma $$ in the dB-scale? Let's remind ourselves of how to convert linear scale to dB scale: $$ |\Gamma|_{dB} = 10 log_{10} {|\Gamma|^{2}} = 20 log_{10} \frac{V^{-}}{V^{+}} $$. Therefore, we can use the $$ \Gamma $$ directly. 

Now, the -10 dBm incident power will lead to a -22 dBm reflected power immediately at the devices' input port. Such -22 dBm power will be further attenuated to -32 dBm upon passing the attenuator. Therefore, at the VNA's end, it sent 0 dBm of power but received -32 dBm back, and thus the measured $$ S_{11} $$ becomes -32 dB, 2 x attenuation (10 dB) lower than the device's actual $$ S_{11} $$. 


