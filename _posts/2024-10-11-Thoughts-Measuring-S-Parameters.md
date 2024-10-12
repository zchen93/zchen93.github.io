# Thoughts on measuring S-Parameters

# Definition of S-Parameter
(discussed later)

# Measuring S-Parameters using VNA
I. Passive Device

II. Active Device
1. Question: What would happen on the measured $$S_{11}$$ if a 10-dB attenuator is attached to the DUT's input?
Definition: $$ S_{11} = \frac{V_{1}^{-}}{V_{1}^{+}} $$ given $$ V_{2}^{+} = 0 $$, reflected voltage over the incident voltage. $$ P^{-} = |\Gamma|^{2} P^{+} $$. Here, $$ \Gamma = S_{11} $$. 

Assuming the VNA provides 0 dBm of output power, and the $$ \Gamma = 12 dB $$. Upon passing the 10 dB attenuator, the incident power is -10 dBm. Here comes the tricky part: how do we deal with the squared $$ \Gamma $$ in the dB-scale? Let's remind ourselves of how to convert linear scale to dB scale: $$ |\Gamma|_{dB} = 10 log_{10} {|\Gamma|^{2}} = 20 log_{10} \frac{V^{-}}{V^{+}} $$. Therefore, we can use the $$ \Gamma $$ directly. 

The -10 dBm incident power will now lead to a -22 dBm reflected power immediately at the devices' input port. Such -22 dBm power will be further attenuated to -32 dBm upon passing the attenuator. Therefore, at the VNA's end, it sent 0 dBm of power but received -32 dBm back, and thus the measured $$ S_{11} $$ becomes -32 dB, 2 x attenuation (10 dB) lower than the device's actual $$ S_{11} $$. 


2. Question: What would happen on the measured $$ S_{21} $$ if a 10-dB attenuator is attached to both the input and output ends of the DUT?
Definition: $$ S_{21} = \frac{V_{2}^{-}}{V_{1}^{+}} $$ given $$ V_{2}^{+} = 0 $$.

Similarly, assuming the VNA provides 0 dBm of output power, and $$ S_{21} $$ of the DUT is 10 dB (gain). At the DUT's input terminal, it sees -10 dBm of power. Adding the 10 dB $$ S_{21} $$ gain, the power level becomes 0 dBm at the DUT output terminal. At the VNA's port 2, it sees the attenuated -10 dBm signal again, so the measured $$ S_{21} $$ will be recorded as -10 dB, which is 2 x attenuation (10 dB) lower than the actual DUT's $$ S_{21} $$. 
