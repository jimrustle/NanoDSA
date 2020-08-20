# NanoDSA
small-sized acceptable performance dynamic signal analyzer


# yes this is inspired from the EEVBlog thread

no guarantees anything works out

- AD4003 + OPA828 (maxwell3e10 on eevblog)
- DAC for freq. response (as tracking gen?) and distortion measurements (Berni on eevblog)
- probably ST micro since they're my favorite

# design parameters

- DC to 1 MHz, ~100 db SNR
- 4096 points FFT
- ADC bits? 16? 18? 24?
- screen? (3-inch or 5-inch TFT LCD using SPI bus?)
- usb-to-computer support like in nanovna?

# comparable designs

## HP/Agilent 35670A
- [35670A datasheet](https://www.keysight.com/ca/en/assets/7018-06687/data-sheets/5966-3064.pdf)
- 122 uHz to 102.4 kHz, 16-bit ADC
- 102.4 kHz 1-channel, 51.2 kHz 2-channel
- 90 dB dynamic range
- +/- 0.15 dB accuracy
- 1600 lines resolution

## Stanford Research Systms SR785/780/770 
- [SR785 product page](https://www.thinksrs.com/products/sr785.html)
- DC to 102.4 kHz, 16-bit ADC
- 90 dB dynamic range (145 dB dynamic range with swept-sine)
- too lazy to read the rest

# Features?
- 1-1e6 averaging, using rms, time, peak-hold averaging
- freq response (as spectrum analyzer)
- power spectrum, PSD (noise analysis)
- whatever else is in the datasheets above

