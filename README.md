# USB-2-3.5mm
Personal Project to drive analog speakers from USB Type C.
##
I utilized a Cmedia CM108B audio IC and a MAX97720A Amplifier IC. The CM108B allows the USB Host (Phone, Laptop, etc...) to detect if it needs 5V power, then, verify what kind of device it is powering. The Cmedia IC then sends an identifier notifying the Host that the device is an audio device, making it load drivers and prepare for audio playthrough. Once this is done, the IC sends the Audio data through its own DACs and internal amplifiers to create a signal.

However, the IC has a low output impedance and a typical RMS output close to a volt, which is good for headphones and acceptable for speakers. But, if we were to power something else such as a car stereo, we would benefit a lot better by converting this output to high impedance, and amplifying it to an amplitude ranging from 1.25-2.1 RMS Voltage. The MAX97220A is set with a gain of 3.52dB and an input impedance of 10k, which should then impedance match better with a car stereo, and also have a beefier signal amplitude, even if not by much (staying safe, to prevent clipping).
