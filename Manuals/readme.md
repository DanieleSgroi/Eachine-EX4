# Manuals

This repository contains the OEM manuals.

# The Frequency problem...

DF806B Wi-Fi can operate either on Ch. 36 (5180 MHz) or Ch. 149 (5745 MHz) with badwidth allocation of 20 MHz according to IEEE 803.11n standard.

In Europe channel 36 is restricted for indoor use only with a maximum transmission power of 200mW (23dBm) E.R.P.

The upper channel 149 can be used outdoor according to Short Range Device (SRD) specification for transmissions up to 25mW (14dBm) E.R.P.

![5GHz Wi-Fi](./5GHz-1024x264.png)

According to the FCC test reports, the DF806 Wi-Fi module (AR1021X) transmits with an average RF power of +16 dBm, while the Controller Wi-Fi module (WT9342) transmits with an average RF power of +20 dBm.

This is sort of chatch "22" for European users: if we want to legally use the drone outdoor, we should select Channel 149 but the drone does not have a means to reduce the transmitted power to the specified limit of 25 mW. 

Furthermore, controller range will be very limited, if the RF power will be reduced to 25 mW. 

On the other hand, we are legitimate to use the full 200 mW of RF power only indoor, where range is not an issue...

This shall be further investigated, maybe with real RF power measures on an European unit. 

As final note, my Eachine EX4 box includes the CE marking that should guarantee compliances to the European rules...

# How to switch the operating frequency

To change the drone channel, press the power button 4 times quickly when the drone is off.

The blue LED will start flashing for about a minute and then go out.

After re-enabling it will be on the other channel.

The controller should be able to automatically bind to the new channel.
