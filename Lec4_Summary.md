# Networks

## Wireless Network Hierarchy

Wireless Networks are categorized into four types:

1. **Personal Area Network (PAN)**
2. Local Area Network (LAN)
3. Wide Area Network (WAN)
4. Global Area Network (GAN)

## Personal Area Network (PAN)

A **Personal Area Network (PAN)** refers to a network created between devices in an individual's immediate surroundings, typically within **10 meters**. It connects personal devices such as smartphones, tablets, wearables, and IoT gadgets.

Examples of technologies used in PANs include **Infrared (IR)**, **Radio-Frequency identification (RFID)**, **Near Field Communication (NFC)**, and **Bluetooth**.

## Wave Propagation Fundamentals

### Why Some Waves Pass, Some Heat, and Some Bounce?

A wave is only **absorbed** if something inside the material can **respond** (move / vibrate / oscillate / jump) at the same frequency.

**Reflection** occurs when the material starts to respond to the wave but cannot absorb the energy, causing it to throw the energy back out.

### Different Frequencies and Their Interaction with Matter

|Frequency Range|What Can React?|Main Interaction|Does It Pass Through Walls?|
|:--|:--|:--|:--|
|**Radio** (kHz–MHz–low GHz)|Almost nothing (too slow)|Weak — walls barely notice it|**Yes (passes)**|
|**Microwave / Infrared** (GHz–THz)|Molecules rotate & vibrate|Strong absorption → heat|**No (blocked or absorbed)**|
|**Visible Light** (10¹⁴ Hz)|Electrons in atoms get excited|Absorbed / scattered (color)|No (opaque) — unless transparent like glass|
|**X-ray** (10¹⁷ Hz and above)|Electrons can’t oscillate, but can be knocked out (ionization)|Weak absorption except in dense elements|Passes through skin, **blocked by bone/lead**|

### Microwave/Wi-Fi Safety Comparison

The reason people are not "cooked" by Wi-Fi, despite using similar frequencies to microwaves, is related to power levels:

- Microwave ovens use **hundreds of watts** of highly concentrated energy trapped in a metal box.
- Wi-Fi routers use **tiny amounts of power** (around **0.1 watts**) that spread out in all directions and fade quickly.

### Comparison of 2.4 GHz Band vs. 5 GHz Band

|Feature|2.4 GHz Band|5 GHz Band|
|:--|:--|:--|
|**Frequency**|2.400–2.4835 GHz|5.150–5.825 GHz (varies by region)|
|**Wavelength ($\lambda$)**|**~12.5 cm**|**~6 cm** (Calculated example: $\lambda = 3 \times 10^8 / 5 \times 10^9 = 0.06 m = 6 cm$)|
|**Throughput**|Lower|**Higher**|
|**Interference**|High (microwaves, Bluetooth, cordless phones)|**Lower** (less crowded, more channels)|
|**Penetration / Wall Traversal**|**Better** (longer wavelength → penetrates walls/floors more easily)|Worse (shorter wavelength → more attenuation)|
|**Coverage Range (Indoor)**|**Longer range** (~30–45 m indoor)|Shorter range (~10–30 m indoor)|
|**Non-overlapping channels**|3 (US: 1, 6, 11)|**23+**|

_Note: A Pair-and-Share Activity requires drawing the 2.4 GHz wave and the 5 GHz wave_.

## Infrared (IR) Wireless Communication

### Characteristics and Use

- **Nature:** Infrared light is a type of electromagnetic radiation with wavelengths longer than visible light, used for short-range communication.
- **Range:** Typically between **1–5 meters**.
- **Frequency Range:** 300 GHz to 400 THz (Terahertz).
- **Bandwidth:** Low data transfer speeds (~115 kbps).
- **Operation:** IR operates by sending a signal in a straight line from source to destination, requiring **line-of-sight communication** (a clear, unobstructed path).
- **Usage:** Primarily used in consumer electronics like TV remote controls, wireless mice, and early mobile phone data transfers (before Bluetooth).
- **Security:** Data is **not encrypted**, making it technically not secure. However, it is **difficult to hack** because of the strict requirement for line-of-sight and its limited range.

## Radio-Frequency Identification (RFID)

### Definition and Applications

- **Definition:** RFID uses electromagnetic fields to automatically identify and track tags attached to objects.
- **Distinction:** RFID is **not a barcode**. Unlike Bluetooth and IR, RFID can be used for passive communication.
- **Applications:**
    - **Access control:** RFID badges for building entry.
    - **Inventory management:** Retail stores and warehouses use RFID to track products.
- **Range and Frequency Bands:**
    - **Low-frequency (LF):** 125–134 kHz, used for short-range applications.
    - **High-frequency (HF):** 13.56 MHz, typically used for ID badges and smart cards.
    - **Ultra-high-frequency (UHF):** 850–950 MHz, used for longer-range applications like inventory tracking.
    - The overall range varies from a few centimeters (HF) to several meters (UHF).
- **Data Transfer:** Typically low, sufficient for identification and tracking.

### Types of RFID (Based on Energy Source)

1. **Active RFID:**
    
    - Tags have an **integrated power source** (a battery).
    - They broadcast a pre-programmed RF signal.
    - The RF signals can be picked up by an RFID reader within the tag's broadcast range.
2. **Passive RFID:**
    
    - Tags **do not have an internal power source** and are powered by the reader.
    - They consist of an Antenna and a small chip for processing and memory.
    - **How it works:** The antennas of the Emitter and Tag are coupled via an Electromagnetic Field. An alternating current passes through the primary coil (Emitter), inducing a field that creates current in the secondary coil (Tag). The Tag uses this induced current for power.
    - **Limitation:** Inductive coupling through air is very inefficient, resulting in a quite limited read/write range.

## Near Field Communication (NFC)

### Characteristics and Operation

- **Nature:** NFC is considered a type of RFID and is essentially an extension of RFID technology.
- **Frequency:** Operates in the **13.56 MHz** frequency band.
- **Range:** Designed specifically for **very close-range communication** (usually within **4 cm**).
- **Sophistication:** While using a shorter distance, NFC has more sophisticated data and processing than general RFID, including **encrypted data**.
- **Security:** Considered **secure** for payment applications because of its short range and encryption protocols.
- **Infrastructure:** The most commonly used format for storing data on an NFC tag is **NDEF (NFC Data Exchange Format)**, which standardizes how data is structured and encoded for interoperability.

### Applications

- Card payment and Mobile payments (Tap-to-pay systems like Google Pay, Apple Pay, Samsung Pay).
- Digital wallets (storing payment cards, boarding passes).
- Access control (smart cards).
- Smart posters (posters embedded with NFC tags that provide information or URLs when tapped).

### Data Types Stored on an NFC Tag

The format and size of stored data depend on the tag's type and memory capacity. Key data types include:

1. Text (simple message).
2. URLs and Web Links.
3. Contact Information (vCard).
4. Phone Numbers (triggers a call).
5. Email Address (or a pre-defined template).
6. Geolocation Coordinates (opens location on a map).
7. Wi-Fi Configuration (allows automatic connection without manual password entry).
8. Bluetooth Pairing Information (allows quick pairing with devices like headphones).
9. Launch an Application (or perform specific actions within an app).
10. Payment Information (encrypted data stored in contactless cards; typically not accessible or modifiable by end users).

### NFC Use on Phones

- **Reading NFC Tags:**
    - On Android and iPhones with iOS 14+, reading is automatic when the device is brought near the tag.
    - Older iPhones (7 to X) require a third-party app (e.g., NFC Tools).
- **Writing to NFC Tags:**
    - Use apps like NFC Tools or NXP TagWriter to write data (text, URL, vCards, etc.) to NFC tags.

### RFID (General) vs. NFC (Subset of RFID) Comparison

|Feature|RFID (General)|NFC (Subset of RFID)|
|:--|:--|:--|
|**Meaning**|Radio-Frequency Identification|Near Field Communication|
|**Frequency Ranges**|LF (125 kHz), **HF (13.56 MHz)**, UHF (860–960 MHz)|**Only HF (13.56 MHz)**|
|**Range**|From a few cm to 12+ meters depending on type|Up to **~4 cm** (very short range)|
|**Communication Direction**|Mostly one-way (reader → tag)|**Two-way** / peer-to-peer (phone $\leftrightarrow$ tag or phone $\leftrightarrow$ phone)|
|**Power Source (Tag)**|Can be Passive, Semi-Passive, or Active|Mostly Passive tags, but devices like phones are powered readers|
|**Data Format Standards**|Varies by type (no universal format)|**NDEF**, standardized for interoperability|
|**Security Level**|Low (ID-only) → High (encrypted active tags)|**Generally high security**, optimized for authentication and payment|
|**Reader Devices**|Specialized RFID readers/scanners|Smartphones (Android & iPhone) + NFC readers|
|**Cost (Tags)**|Passive: $0.05–$0.20; Active: $10–$50+|NFC: $0.20–$1 (simple) / $1–$5 (secure)|
|**Cost (Readers)**|Basic: $50–$300; Industrial long-range: $500–$2000+|NFC readers: $10–$50 (USB/Bluetooth); Smartphones already support it|


# Kotlin

- **Kotlin** is listed as a topic on the agenda.
- Students are directed to "See Waterloo’s University Slides" for information on Kotlin.
- Suggested readings include the Kotlin slides and a free Kotlin book.