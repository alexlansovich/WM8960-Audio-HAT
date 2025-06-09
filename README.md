# WM8960-Audio-HAT
Audio driver for WM8960 on RPI CM4


# Activate I2c
activate i2c in raspi-config

# Add to config.txt driver 

[all]

dtoverlay=wm8960-soundcard

