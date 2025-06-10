
# 🎧 WM8960-Audio-HAT
Audio driver for **WM8960** on **Raspberry Pi CM4**.  
No need to install drivers — just activate.

---

## 🔧 Setup Instructions

### 1️⃣ Enable I2C
Enable I2C through `raspi-config`:
```bash
sudo raspi-config
```
- Go to **Interfacing Options**.
- Select **I2C** and enable it.

---

### 2️⃣ Configure `config.txt`
Open `/boot/config.txt` and add the following line:
```ini
[all]
dtoverlay=wm8960-soundcard
```

---

## ⚠️ Additional Steps
✅ Update your system and kernel:
```bash
sudo apt update
sudo apt full-upgrade
```

✅ Ensure the **WM8960 HAT** is physically connected to your Raspberry Pi CM4.

✅ After reboot, check the audio device:
```bash
aplay -l
```

---

## 📚 Useful Links
- [Raspberry Pi I2C Documentation](https://www.raspberrypi.com/documentation/computers/raspberry-pi.html#i2c)
- [WM8960 Datasheet](https://www.ti.com/product/WM8960)

---

Enjoy high-quality audio with your Raspberry Pi CM4! 🎶
