# CompTIA-APlus-Study-Log

<br>

## Objective 1.1: Install/Configure Laptop Hardware

**The Lab:** Tore down an `Acer Aspire One` to identify and replace components.

### 🔋 Battery
* **What I Did:** Unlocked the battery using the mechanical slider, followed by using the battery removal button.
* **What I Learned:** The battery is **very easy to remove** on this device. it is `10.8v`, `2200mAh`, `23.76Wh`.

### 💾 Hard drive
* **What I Did:** I removed the left-most plastic door with 2 screws. Followed by 1 screw on the actual hard drive.
* **What I Learned:** The `HDD` is **very snug** and difficult to remove from the `SATA` (Serial Advanced Technology Attachment) connector. The `HDD` was easily reinstalled.

* **Comparing Formats**
  * **Types**
    * **SSD:** (Solid State Drive) Uses flash memory (like a USB stick). No moving parts, super fast, and durable.
    * **Hybrid:** (`SSHD`) A magnetic disk with a small amount of `SSD` memory built in. It keeps your most-used files on the fast part for a speed boost.
    * **Magnetic Disk:** (`HDD` - Hard Disk Drive) Uses spinning magnetic platters and a read/write arm. Slower and more fragile.
  * **Sizes**
    * **1.8in:** a very old, and very portable style/ size of hard drive.
    * **2.5in:** The standard, and what I found in my laptop.

### 🧠 Memory (RAM)
* **What I Did:** Removed the middle panel door via a single screw, and unclipped the 2 metal latches, allowing the single ram stick (`SO-DIMM`) to loosen.
* **What I Learned:** 1. Ram is **easily replaced**. 2. This old laptop only uses `1 GB` of RAM.

### 🔌 mPCIe
* **What I Did:** Removed the right panel door via a single screw, and found an empty `mini PCIe` slot.
* **What I Learned:** `mPCIE` is mostly used for adding `wifi` and `Bluetooth` functionality, but is often capable of many other additions, such as `storage` or `eGPU`.

### ⌨️ Keyboard
* **What I Did:** There is a tiny notch above the `f8` key. Once pushed in, the keyboard can be gently pried out. Disconnected ribbon cable via `ZIF` connector.
* **What I Learned:** I personally had a **hard time getting the notch to click**. Keyboards are much easier to replace than I initially thought. Uses `ribbon cables` and `scissor-switch` keys.

### 🔩 Plastics
* **What I Did:** Removed `14` screws from the back, `+1` near HDD, `+1` near RAM, `+5` under keyboard, removed the touchpad ribbon cable, removed the power button ribbon cable, took a pry tool around the plastics.
* **What I Learned:** First time going this deep into a laptop, I am **confidently nervous**. Nothing too difficult thus far.

### 🖱️ Touchpad
* **What I Did:** Removed the plastics (my touchpad was built into the plastics from the last step.)
* **What I Learned:** If the touchpad has an electronic problem, I can replace the **controller board**. If the touch pad has physical damage, I'd have to replace the **entire keyboard frame /plastics**.

### 📡 Wireless Card
* **What I Did:** Under the touchpad plastics, I removed the 2 antenna cables (`U.FL` connectors) and a screw.
* **What I Learned:** the wifi card is **tiny!**

### 🟩 Motherboard 
* **What I Did:** Removed 1 screw, 4 ribbon cables (power supply, screen, speakers).
* **What I Learned:** It's **surprisingly simple** to take out the motherboard.

### 🔊 Speaker
* **What I Did:** 2 more screws, 1 ribbon cable (already disconnected).
* **What I Learned:** Both speakers share the **same connector port**.

### 💡 CPU
* **What I Did:** (Everything from the previous steps.) Removed heatsink.
* **What I Learned:** My PC uses a `intel NH82801GBM L9265H53 SL8YB '04`. It is **soldered** (`BGA`) and **not replaceable**.

<br>

## Objective 1.2: Install/Configure Laptop Display

*I had a hard time with dismantling my laptop's display; there was a hidden screw that required you to cut out a portion of plastic with an exacto knife(I only found this out from an official on a forum), very strange.*

### 📷 Webcam & Microphone
* **Location:** Top center, behind the screen assembly.
* **Connection:** Both are connected directly to the same control board, and that board is wired through the hinge to the motherboard via ribbon cable.
* **A+ Relevance:** The placement is best for a user's audio and video needs. If a user reports the webcam or microphone not working, the **wire through the hinge** seems like a likely fail point.

### 📶 Wi-Fi Antennas
* **Location:** Routed around the perimeter of the `LCD` panel, behind the bezel.
* **Connection:** These wires (black and white) run down through the hinge and connect to the Wi-Fi card (`mPCIe`/`M.2`) on the motherboard via `U.FL` connectors.
* **A+ Relevance:** Having the antennas as high as possible will provide better reception. A weak connection could likely be caused by a **disconnected antenna** or **damage where they pass through the hinge**.

### 🖥️ LCD Panel
* **Location:** Held into the metal frame by 4 small screws.
* **Connection:** Connected by a flat ribbon cable (`LVDS`/`eDP`) that also runs through the hinge.
* **A+ Relevance:** Damage to this **hinge cable** could cause display issues such as flickering or even no image at all. (Note: This model uses an `LED` backlight.)

<br>

## Objective 1.3: Laptop Features

### ✨ Special Function keys
* **A+ Detail:** Activated with <kbd>Fn</kbd> + <kbd>F#</kbd>/Icon keys (e.g., <kbd>Fn</kbd> + <kbd>F1</kbd>.) Controls various quick functions such as brightness, volume, Wi-Fi, display output, touchpad toggle, keyboard backlight, etc. Troubleshooting: **Requires manufacturer drivers/utility software** to function correctly; may be disabled in `BIOS`/`UEFI`.

### 🧩 Docking station vs. Port replicator
* **A+ Detail:** Both are external devices that connect to your machine via a single cable (`USB-C`/`Thunderbolt` or proprietary). The device is a connection hub for your laptop's peripherals. Although similar, a **docking station** typically offers **more/different ports**, and usually, your power passes through (charges laptop). A **port replicator** mainly **duplicates existing ports**.

### 🔒 Physical laptop lock and cable lock
* **A+ Detail:** Allows the user to insert a cable into the `Kensington lock slot` (or `Noble Wedge`) to deter theft.

<br>

## Objective 1.4 Compare/Contrast various mobile devices.

* **Tablets:** Larger screen (media focus). Mobile OS. A+ Angle: Treat like a big phone for Wi-Fi/App issues. 📱
* **Smartphones:** All-in-one (cellular). Mobile OS. A+ Angle: Core device (connectivity, OS, security, sync). 📞
* **Smart watches:** Wrist notifications/tracking. A+ Angle: `Bluetooth` pairing/sync issues with phone. ⌚
* **Fitness monitors:** Health metrics focus. A+ Angle: `Bluetooth` pairing/sync with fitness app. 💪
* **VR/AR headsets:** Immersive digital view (VR) / Overlay (AR). A+ Angle: PC/Console connectivity issues, sensor calibration. 🕶️
* **E-readers:** Reading focus. A+ Angle: E-ink display (ghosting/refresh issues = unique troubleshooting). 📖
* **GPS:** Dedicated navigation. A+ Angle: Satellite signal issues (needs clear sky), map updates. 🗺️

<br>

## Objective 1.5: Accessories & Ports

### Wired Connection Types

|| Mini USB | Micro USB | USB C | Proprietary Vendor-Specific | Ports (Communication/Power) |
| --- | --- | --- | --- | --- | --- |
| **Max Speed (Typical)** | Up to `480Mbps` (`USB 2.0`) | Up to `480Mbps` (`USB 2.0`) | Up to `40Gbps` (with `Thunderbolt`/`USB4`) | Varies | Varies |
| **Power Delivery** | Low (`~5W` Max) | Low (`~5W` Max) | High (Up to `240W` `PD`) | Varies | Varies |
| **Status / Versatility** | Obsolete; Mainly found on old cameras | Phasing out; Mainly for older / budget devices | **Industry Standard** for video, data, and power | Niche; For a single product/brand | Essential; to specific functions (e.g., `Barrel Jacks`) |

### Wireless Connection Types

|| NFC (Near Field Communication | Bluetooth | IR (Infrared) | Hotspot |
| --- | --- | --- | --- | --- |
| **Data Rate** | Very Low (Up to `424 Kbps`). | Low to Medium (Up to `~24 Mbps`, depending on version). | Very Low (Mainly for simple commands). | High (Matches the Wi-Fi or cellular connection being shared). |
| **Security/Pairing** | High Security (due to short range ~4cm) | PIN Protected; can be vulnerable at longer range (~10m). | Not applicable (no data security needed for basic commands). | Standard Wi-Fi security (`WPA2`/`WPA3`) with a password. |
| **Core Function** | Works via magnetic induction; like a mini-transformer. | Works via radio waves (`2.4 GHz` band). | Works via light, like a very simple flashlight (line-of-sight). | Creates a Wi-Fi network from another connection (like cellular). |

<br>

---
---
---

<br>

> [!NOTE]
> **Moving forward**, I'll be adopting a `jot notes` **study method** to help me learn more efficently.<br>
> `A+ Angles` (Troubleshooting common symptoms) will also become jot notes, but listed after a `~`.
> <details>
> <summary> e.g. </summary>
> <b>USB C:</b> Modern Standard; Very Fast for data and power (up to <code>40Gbps</code>/<code>240W</code> PD) ~ Does the port support PD, or thunderbolt ⚡?
> </details>

<br>

---
---
---

<br>

## Objective 1.6: Mobile Device - Network Connectivity

### 🛜 Wireless/Cellular data network
*  **Hotspot:** Share cellular data via WiFi. Set `SSID`(network name) & pswd ~ Reception? Plan limits? Verify pswd.
*  **Tethering:** Shares phone data via `USB`(Faster) or `Bluetooth`(slower) ` ~ Plan limit? Lose cable? Drivers? BT Pairing trbl?
*  **Airplane mode:** Disables all wireless radios (`Cellular`, `Wifi`, `BT`, `NFC`, `GPS`) ~ Can be used to reset radios. Is it accidentally enabled?

### 🟦🦷 Bluetooh
*  The pairing steps are common knowledge ~ Interference(`2.4GHz`)? Discoverable? Forget/Repair.

### 📧 Email configuration
*  **POP3:** Downloads Mail from the server to a device, and deletes the server copy.
*  **IMAP:** Syncs/copies mail from the server to all devices. Any changes made on your device (e.g., deleting mail) sync back to the server.
*  **Port and SSL Settings:** `ports` tell the pc which application data is intended for. `SSL` is an older protocol of `TLS`.  Both protocols are encryption methods for email.
*  **S/MIME:** End-to-end encryption. The sender signs the mail with their private key; the receiver uses the sender's public key to verify.

### PRI updates vs PRL updates
* **PRI:** (Preferred Roaming Instructions) Contains Instructions for how the phone should act on the network.
* **PRL:** (Preferred Roaming list) Contains a list of towers the phone is allowed to connect to, and preferred towers.

### IMEI vs. IMSI
* **IMEI:** Phones 15 digit harware ID ~ Network can block stolen phones from internet.
* **IMSI:** SIM card subscriber ID. Identifies you, not your hardware. ` IMSI authenticates you, allows you to make calls.
  
<br>

---

<br>

## Objective 2.1: Ports & Protocols

*I've created my own ports memorization game here: (link was removed due to privacy)*

* **TCP:** Slow; Handshake required. Memorization Trick: TrustedCP
* **UDP:** Quick; fire and forget. Memorization Trick: UntrustedDP

<br>

## Objective 2.2 Compare & Contrast Network Hardware.
*I used AI to summarize my definitions here, so that I can take note refreshers more efficiently.*  

* **Router:** Connects different networks together (like your home network to the internet) and directs traffic between them.
* **Switch:** Connects devices within the *same* network (like PCs, printers) and intelligently forwards data only to the intended device.
    * **Managed Switch:** Advanced switch that allows configuration (`VLANs`, traffic monitoring, security).
    * **Unmanaged Switch:** Plug-and-play switch with no configuration options; just adds more ports to a network.
* **Access Point (AP):** Creates a wireless local area network (`WLAN`), allowing Wi-Fi devices to connect to a wired network.
* **Cloud-based Network Controller:** Software that allows centralized management of network devices (switches, APs) remotely via the internet (the cloud).
* **Firewall:** A security device (hardware or software) that blocks or allows network traffic based on security rules to protect a network.
* **Network Interface Card (NIC):** A physical component (internal card or `USB`) that allows a computer to connect to a network.
* **Repeater:** A simple device that receives a weak network signal and retransmits it to extend the range.
* **Hub:** An old, basic device that connects network devices but inefficiently broadcasts *all* data to *every* port (unlike a smart switch).
* **Cable/DSL Modem:** A device that connects your home network to your Internet Service Provider (ISP) over cable TV lines or phone lines (DSL).
* **Bridge:** Connects two different network segments so they act as one single network.
* **Patch Panel:** A mounted hardware assembly with ports to organize and manage incoming and outgoing Ethernet cables in a closet or server room.
* **Power over Ethernet (PoE):** Technology that sends both data and electrical power to devices (like IP cameras or phones) over a single Ethernet cable.
* **Ethernet over Power (EoP):** Technology that uses a building's existing electrical wiring to transmit network data, using adapters plugged into wall outlets.

<br>

## Objective 2.3: Configuring SOHO.

### 📶 Wi-Fi Settings
* **SSID:** The Wi-Fi network name you broadcast.
* **Encryption:** `WPA3` is the best/newest. `WPA2-AES` is the most common secure standard. `WPA` & `WEP` are old and insecure.
* **Channel:** Set to `Auto` is usually fine. If you have interference on the `2.4GHz` band, manually set it to channel `1`, `6`, or `11`, as these don't overlap.

### 🌐 IP Addressing
* **DHCP:** Enabled by default. This is the service that automatically hands out private `IPv4` addresses (like `192.168.1.100`) to devices on your network.
* **Subnet Mask:** Defines the size of your local network. Usually, `255.255.255.0` is used for home networks.

### 🔥 Firewall & NAT
* **NAT:** (Network Address Translation) The core job of the router. It hides all your private/internal `IPs` behind your single public `IP` from the `ISP`.
* **MAC Filtering:** A "guest list" based on a device's physical `MAC address`. It's weak security (`MACs` can be faked) and a hassle.
* **Port Forwarding:** A rule you create to let outside traffic in to a *specific* device on your network (e.g., allowing game server traffic on `port 25565` to go to your gaming PC at `192.168.1.50`).
* **UPnP:** (Universal Plug and Play) lets apps (like games) automatically create port forwards. It's convenient but a security risk (malware could use it too).
* **DMZ:** (Demilitarized Zone) A setting that puts one device (e.g., a console) completely outside the firewall, exposing all its ports to the internet. It's a last resort and very risky.

### 🚦 Traffic Control
* **QoS (Quality of Service):** A "fast lane" for your network. You can set rules to prioritize important traffic (like your Zoom call or Xbox game) and de-prioritize other traffic (like a large download).

<br>

## Objective 2.4: Compare Wireless Network Protocols.

### 802.11 Mnemonics
* **802.11(protocols):** `b, a, g, n, ac, ax`= "Baggin Ack Axe" (fun to say, easy to remember) - Used to organize letters by release order. 
* **802.11(Ghz):** Surrond the "5" = `2.4, 5, 2.4` & `both, 5, both`. b=2.4, a=5, g=2.4, n=both, ac=5, ax=both.

### Frequencies
* **2.4Ghz:** Slow & Long Range. This band is very crowded. -- has channels 1-11; channels 1, 6, 11 don't overlap
* **5Ghz:** Fast & Short Range. This band struggles to go through walls.

### 🏠 PAN & IoT Standards
* **Bluetooth:** Short-range (PAN - Personal Area Network). Connects peripherals (headsets, keyboards). 🎧
* **NFC (Near Field Communication):** *Extremely* short~4 cmge (~4cm). Used for "tap-to-pay." 💳
* **RFID (Radio-Frequency Identification):** One-way reader scans a passive tag (e.g., access badges, store anti-theft tags). 🏷️
* **Zigbee / Z-Wave:** Low-power `mesh networks` for smart home (IoT) devices (lights, locks). *Require a hub.* 💡

### WAN
* **3G:** The old, slow standard. (Think early smartphones).
* **4G / LTE:** (Long Term Evolution) The fast, modern standard for many years. `LTE` is just a specific type of `4G`.
* **5G:** The *newest and fastest* standard. Offers much higher speeds and lower latency (less lag).

<br>

## Objective 2.5: Services Provided by a Networked Host.

### Server Roles
* **Web Server:** Hosts websites and serves pages to users. ~ Uses `HTTP` (port 80) & `HTTPS` (port 443).
* **File Server:** Stores and manages files in a central location (e.g., `SMB` for Windows, `AFP` for Mac). ~ Key for shared drives on a business network.
* **Print Server:** Manages print jobs and shares printers with multiple users.
* **DHCP Server:** Automatically assigns `IP` addresses to devices
* **DNS Server:** Translates domain names to IP addresses.
* **Proxy Server:** Middleman for client requests. It can filter content, cache (save) common websites to speed things up, and hide your internal `IP`.
* **Mail Server:** Handles sending (`SMTP`) and receiving (`IMAP`/`POP3`) email.
* **Authentication Server:** sends your credentials over the network to the Authentication Server. Log in from any device.
* **Syslog:** A server that collects log messages from all other network devices into one central place.

### Internet Appliance
* **UTM:** (Unified Threat Management) An all-in-one security device. It's a Firewall + `IDS`/`IPS` + `Proxy` + `VPN` + more... all in one box.
* **IDS:** (Intrusion Detection System): A "burglar alarm." It detects potential attacks and sends an alert.
* **IPS:** (Intrusion Prevention System): A "security guard." It detects attacks and actively tries to stop them.
* **End-Point Management Server:** A server that manages all the "end-points" (desktops, laptops, phones) in a business. ~ Used to push software updates, enforce security policies, and track inventory.

<br>

###  Objective 2.7: Connection Types
* **LAN:** *(Local Area Network)* Your private network (home, office building).
* **WAN:** *(Wide Area Network)* Connects `LANs` together. The Internet is the biggest `WAN`.
* **PAN:** *(Personal Area Network)* A tiny network for your personal devices. ~ `Bluetooth` is the best example.
* **MAN:** *(Metropolitan Area Network)* A network spanning a city or large campus.
* **WMN:** *(Wireless Mesh Network)* A network of wireless APs that all talk to each other to create a large, seamless Wi-Fi coverage area.

<br>

### Objective 2.8: Network Tools
* **Loopback plug:** A small plug that redirects outgoing signals right back into the port. ~ Used to test if a computer's NIC is working.
* **Punchdown tool:** The tool used to "punch" the small wires of an Ethernet cable into a patch panel or a keystone (wall) jack.
* **WiFi analyzer:** An app for phone or laptop that shows you all the nearby Wi-Fi networks. ~ Used to find the SSID, signal strength, and channel of all networks.
  
<br>

### Objective 3.1: Cable Types

#### Network Cables
* **Ethernet:** `(Cat 5, Cat 5e, Cat 6)` Standard RJ-45 for LAN. `Cat 5` = Old (100Mbps), `Cat 5e` = Good (6Gbps), `Cat 6` = Better (10Gbps, but for shorter distances) ~ `Cat 5e` or `Cat 6` for all modern networks to get gigabit speed.
* **Plenum:** Cable with a special fire-resistant Plenum-rated jacket (plastic coating). ~ *Required by building code* for cables run in "plenum" spaces (air ducts, drop ceilings) because it won't release toxic smoke in a fire.\
* **Shielded (STP) vs. Unshielded (UTP):** UTP = Standard, cheap Ethernet cable. STP  = Has a metal foil shield inside. ~ Use STP in electrically "noisy" areas.
* **568A/568B:** The two standards (color-coded pin order) for wiring an RJ-45 connector..
* **Fiber:** Transmits data using light pulses. Made of glass.
* **Coaxial (Coax):** The cable used for Cable TV. Has a single solid copper core.
*All standard Ethernet (UTP/STP) has a maximum distance of 100 meters (328 ft). After that, the signal degrades.*

#### Video Cables
* *skipped common knowledge cables*
* **DVI:** DVI-D = Digital only. DVI-A = Analog only (rare). DVI-I = Integrated (carries both digital and analog signals in one connector).

#### Multi-purpose cables
* **Lightning:** -pin, Apple proprietary connector for iPhones/iPads. Reversible. ~ Being replaced by USB-C on the newest Apple devices.
* **Thunderbolt:** High-speed data/video standard developed by Intel & Apple. ~ Lightning bolt logo ⚡. Fastest speeds (up to 40 Gbps).
* **USB (2.0 vs 3.0):** USB 2.0 = Slow (480 Mbps), port is often black. USB 3.0 (and up) = Fast (5 Gbps+), port is often blue. ~ Backward compatible, but you only get the speed of the slowest part (e.g., a USB 2.0 drive in a 3.0 port runs at 2.0 speed).
* **USB-C:** Small, oval, reversible. ~ Can run at slow USB 2.0 speeds, fast USB 3.1 speeds, or  Thunderbolt speeds.

#### Peripheral & Hard Drive Cables
* **Serial:** Old, 9-pin "D" connector. Very slow. ~ Obsolete for peripherals, but still used to configure network switches/routers via a `console` port.
* **SATA:** Modern standard for internal `HDDs`, `SSDs`, optical drives. Small, "L"-shaped connector. ~ You need two cables: a thin 7-pin for **data** and a wider 15-pin for **power**.
* **IDE (PATA):** Old, wide 40-pin ribbon cable for hard drives. ~ Obsolete. One cable handled two devices (`Master`/`Slave`).
* **SCSI:** Old, high-performance standard for servers. Used wide ribbon cables or chunky external ports. ~ Obsolete (replaced by `SAS` and `SATA`), just know it was a server standard.

#### Adapters
* **DVI to HDMI:** `DVI-D` to `HDMI` is an easy, passive adapter. ~ Both signals are **digital**. (`DVI` doesn't usually carry audio).
* **USB to Ethernet:** A dongle that gives you an `RJ-45` port via `USB`. ~ Common for thin laptops/tablets that don't have a built-in `Ethernet` port.
* **DVI to VGA:** A passive adapter only works if the `DVI` port is `DVI-I` (carries the analog signal). ~ If the port is `DVI-D` (digital only), you need an **active converter**.
  
<br>

### Objective 4.1: Cloud Computing Concepts

#### Common Cloud Models
* **IaaS:** (Infrastructure): Provider gives you raw hardware 
* **SaaS:** (Software): Provider manages everything. You just use the software. ~ e.g. Netflix, Gmail, Youtube.
* **PaaS:** (Platform): Provider gives Hardware + OS + Dev Tools.

<br>

### Objective 4.2: Set up client-side virtualization

* **VM Purpose:** Sandbox (testing/security), Legacy OS support, Cross-platform compatibility.
* **Resource Requirements:** VMs need dedicated RAM, CPU cores, and Storage. `VT-x` (Intel) or `AMD-V` (AMD) must be enabled in `BIOS`.
* **Hypervisor (The Manager):** The Hypervisor is the software that creates and manages the VMs.
* **Network Requirements:** `Bridged` = On the main `LAN` (own `IP`). `NAT` = Hidden behind Host. Internal = No internet access (secure sandbox).
* **Security Requirements:** Keep Guest OS patched. Ensure VM Isolation to prevent malware from escaping to the Host. (when testing potential viruses)
* **Emulator Requirements:** Mimics different hardware (e.g., Android phone on PC). Very resource-intensive.
