# Udara-Deshan
# 📡 Two-Way Digital Paging System  
### Communication Design Project – Semester 3

This project presents the design and implementation of a bidirectional digital paging system using BladeRF SDR hardware.  
The system integrates reliable RF communication, acknowledgement mechanisms, and a simple messaging-style graphical interface.

---

## 🔍 Project Overview

The system enables two users to exchange short text messages wirelessly through Software Defined Radio (SDR) technology.  
It combines physical layer modulation techniques with data-link layer reliability mechanisms.

---

## 🚀 Key Functionalities

• Bidirectional RF Communication using BladeRF  
• QPSK (Quadrature Phase Shift Keying) modulation  
• Stop-and-Wait ARQ protocol for reliability  
• CRC32-based frame error detection  
• Dual-frequency operation:
  - 2.4 GHz ISM band → Message transmission  
  - 1.2 GHz band → Acknowledgement channel  
• Real-time messaging GUI interface  

---

## 🧱 Frame Structure

### 📦 Message Frame
- Preamble  
- Source & Destination Address  
- Sequence Number  
- Payload  
- CRC32  

### ✅ Acknowledgement Frame
- Preamble  
- Addresses  
- Sequence Number  
- ACK Flag  
- CRC32  

---

## 🖥️ User Interface

The graphical interface is designed similar to a lightweight chat application:

• Text-only messaging  
• Real-time send/receive display  
• Simple and minimal design  
• Reliable delivery confirmation  

---

## ⚙️ System Workflow

1. User enters text message in GUI  
2. Message is packetized into structured frames  
3. Frames are QPSK modulated  
4. Transmission via BladeRF (2.4 GHz)  
5. Receiver demodulates and validates using CRC32  
6. ACK sent back through 1.2 GHz channel  

---

## 🛠 Technologies Used

- BladeRF SDR Platform  
- Python-based signal processing  
- GNU Radio  
- CRC32 error detection  
- Stop-and-Wait ARQ protocol  

---

## 🎓 Learning Outcomes

Through this project, we gained:

• Practical experience in SDR communication  
• Understanding of modulation techniques (QPSK)  
• Implementation of ARQ reliability mechanisms  
• Frame-based protocol design  
• GUI development for communication systems  

---

## 🔮 Future Improvements

- Forward Error Correction (FEC)
- Secure encrypted messaging
- Multimedia/file transmission support
- Higher data rate optimization

---

## 👨‍💻 Team Members

- Dulith Kavinda  
- Achintha Bandara  
- Hasindu Gunasekara  
- Udara Deshan  

Faculty of Electronic & Telecommunication Engineering
