
# HackRF One: Software Defined Radio (SDR) for Hackers

## Capabilities:
- **Operating Frequency:** 1 MHz to 6 GHz
- **Transceiver Type:** Half-duplex
- **Sample Rate:** Up to 20 million samples per second
- **Sample Resolution:** 8-bit quadrature samples (8-bit I and 8-bit Q)
- **Compatibility:** GNU Radio, SDR#, and more
- **Configurability:** Software-controlled RX and TX gain, baseband filter, antenna port power (50 mA at 3.3 V)
- **Connectors:** SMA female antenna, SMA female clock input and output for synchronization
- **Interface:** Hi-Speed USB 2.0
- **Power:** USB-powered
- **Hardware:** Open source hardware

## Setting Up Your HackRF One
### Step 1: Connect Your HackRF One

1. Connect your HackRF to a USB port.
2. Download the HackRF utilities from the Kali repository:

   ```bash
   kali > sudo apt install hackrf
   ```

3. Check the version of your HackRF One:

   ```bash
   kali > sudo hackrf_info
   ```
Here is the firmware update and Windows driver installation process for HackRF One documented in Markdown format:

# Setting Up HackRF One SDR

This guide covers firmware upgrade for HackRF One software-defined radio and using it with Windows software.

## Firmware Update

To update to the latest firmware:

1. Download the firmware binary from GitHub:
   ```
   https://github.com/mossmann/hackrf/releases
   ```
2. Extract the archive to get the `hackrf-2021.03.1` folder 
3. Navigate to `hackrf-2021.03.1/firmware-bin` 
4. Flash the new firmware:
   ```
   hackrf_spiflash -w hackrf_one_usb.bin
   ```
5. Disconnect and reconnect HackRF One
6. Verify updated firmware with:
   ```
   hackrf_info
   ```

## Windows Driver Setup

To use HackRF One in Windows apps like SDR#:

1. Install [Zadig](https://zadig.akeo.ie/)
2. Connect HackRF and select it in Zadig
3. Click "Install Driver"  
4. Download [ExtIO_HackRF DLL](https://github.com/ExtIO_HackRF/releases)
5. Copy `ExtIO_HackRF.dll` to SDR# folder
6. Launch SDR# 
7. When prompted, select `ExtIO_HackRF` hardware   

Now HackRF One can be used for receiving and transmitting radio signals with SDR# and other Windows software.
