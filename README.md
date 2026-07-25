# USB-2-3.5mm
Personal Project to drive analog speakers from USB Type C.
##
I utilized a Cmedia CM108B audio IC and a MAX97720A Amplifier IC. The CM108B allows the USB Host (Phone, Laptop, etc...) to detect if it needs 5V power, then, verify what kind of device it is powering. The Cmedia IC then sends an identifier notifying the Host that the device is an audio device, making it load drivers and prepare for audio playthrough. Once this is done, the IC sends the Audio data through its own DACs and internal amplifiers to create a signal.

The MAX97220A is set with a gain of 3.52dB and an input impedance of 10k. The output of the MAX IC is wired directly onto the 3.5mm.
