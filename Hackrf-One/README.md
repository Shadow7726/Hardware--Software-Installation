# Hardware--Software-Installation

Absolutely, here's the information rearranged into Markdown format with a more structured layout:


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
