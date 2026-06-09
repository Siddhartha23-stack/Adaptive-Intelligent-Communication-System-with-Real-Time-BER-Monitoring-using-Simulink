# Adaptive-Intelligent-Communication-System-with-Real-Time-BER-Monitoring-using-Simulink


> A Simulink-based adaptive system that selects the best digital modulation 
> technique in real time using Bit Error Rate (BER) analysis over an AWGN channel.

---

## 📌 Overview

This project implements an adaptive communication system that simultaneously 
evaluates **BPSK, DBPSK, 2-PAM, and 4-FSK** modulation schemes under varying 
noise conditions and intelligently selects the most reliable one based on 
real-time BER performance.

---

## 🛠️ Tools & Technologies

- MATLAB & Simulink
- Communication Toolbox
- AWGN Channel Model
- Bernoulli Binary Generator

---

## 🔧 System Architecture

| Stage | Component |
|---|---|
| Data Source | Bernoulli Binary Generator |
| Modulation | BPSK, DBPSK, 2-PAM, 4-FSK |
| Channel | AWGN (Eb/N₀ varied from 2–10 dB) |
| Demodulation | Respective demodulators |
| Decision | Lowest BER selection engine |

---

## 📊 Results

| Modulation | Eb/N0=2 | Eb/N0=4 | Eb/N0=6 | Eb/N0=8 | Eb/N0=10 |
|---|---|---|---|---|---|
| DBPSK | 0.503 | 0.495 | 0.515 | 0.499 | 0.5127 |
| BPSK  | 0.504 | 0.496 | 0.514 | 0.499 | 0.5127 |
| PAM   | 0.505 | 0.4945| 0.509 | 0.498 | 0.5125 |
| FSK   | 0.497 | 0.4937| 0.508 | 0.504 | 0.4921 |

✅ **BPSK consistently achieves the lowest BER**, making it the most 
reliable scheme under AWGN conditions.

---

## 🚀 How to Run

1. Clone this repository
```bash
   git clone https://github.com/yourusername/adaptive-ber-communication-simulink.git
```
2. Open MATLAB and navigate to the `simulink/` folder
3. Open `adaptive_comm_system.slx`
4. Run the simulation and observe BER outputs in the display blocks

---

## 👥 Team

| Name | Roll No |
|---|---|
| N. Siddhartha | 24071A04H4 |
| P. Nithin Reddy | 24071A04H7 |
| P. Sai Manaswi | 24071A04H5 |
| U. Hema Lakshmini | 24071A04K1 |

> Supervised by **Dr. T. Srinivas** & **Mrs. M. Bhagya Lakshmi**  
> VNRVJIET, Hyderabad | A.Y. 2025–26

---

## 📚 References

- Simon Haykin – *Communication Systems*, Wiley
- B.P. Lathi – *Modern Digital and Analog Communication Systems*
- John G. Proakis – *Digital Communications*, McGraw-Hill
- MATLAB & Simulink Communication Toolbox Documentation

---

## 📄 License

This project is for academic purposes only.
