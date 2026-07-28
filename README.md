<p align="center">
  <img src="https://img.shields.io/badge/STATUS-INTEGRATING-3FB950?style=for-the-badge&labelColor=0D1117&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0id2hpdGUiPjxwYXRoIGQ9Ik0xIDEyczQtNyAxMS03IDExIDcgMTEgNy00IDctMTEgN1MxIDEyIDEgMTJ6Ii8%2BPGNpcmNsZSBjeD0iMTIiIGN5PSIxMiIgcj0iMy4yIiBmaWxsPSIjMEQxMTE3Ii8%2BPC9zdmc%2B" />
  <img src="https://img.shields.io/badge/MOUNT-TRACKING-00D9FF?style=for-the-badge&labelColor=0D1117&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgc3Ryb2tlPSJ3aGl0ZSIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiPjxjaXJjbGUgY3g9IjEyIiBjeT0iMTIiIHI9IjciLz48Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSIyLjUiLz48cGF0aCBkPSJNMTIgMXY0TTEyIDE5djRNMSAxMmg0TTE5IDEyaDQiLz48L3N2Zz4%3D" />
  <img src="https://img.shields.io/badge/DOMAIN-ASTRO%20%2F%20AEROSPACE-A371F7?style=for-the-badge&labelColor=0D1117&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgc3Ryb2tlPSJ3aGl0ZSIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiPjxwYXRoIGQ9Ik0xMiAyYzMuNSAzIDUgNyA1IDExbC01IDQtNS00YzAtNCAxLjUtOCA1LTExeiIvPjxwYXRoIGQ9Ik03IDEzbC0zIDUgNC0xTTE3IDEzbDMgNS00LTEiLz48Y2lyY2xlIGN4PSIxMiIgY3k9IjkiIHI9IjEuOCIgZmlsbD0id2hpdGUiLz48L3N2Zz4%3D" />
  <img src="https://img.shields.io/badge/TARGET-UNKNOWN-D29922?style=for-the-badge&labelColor=0D1117&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0id2hpdGUiPjxwYXRoIGQ9Ik0xMiAybDIuNyA2LjlMMjIgOS42bC01LjUgNC41TDE4LjMgMjIgMTIgMTguMSA1LjcgMjJsMS44LTcuOUwyIDkuNmw3LjMtLjd6Ii8%2BPC9zdmc%2B" />
</p>

```diff
+ [LOG] Dome opened. Mount slewing to target...
+ [LOG] Plate solve OK — target V1096 Her locked.
+ [LOG] RA 17h 28m 44.996s / DEC +43° 48' 12.905"  (first light, first star)
! [WARN] Seeing 3.4" and rising. Increasing guide exposure.
- [ERR] Cloud sensor tripped at 78%. Sequence paused.
+ [LOG] Calibration frames applied. Signal is clean. Welcome in.
```

# Welcome to the observation deck

<img align="right" alt="GIF" src="images/moonlight-kirokaze.gif" />

I'm an astronomer based in Türkiye, working toward astrophysics and data science.
I spend most of my time in the narrow strip
where celestial mechanics, signal processing and shipping actual software overlap — writing
the code that turns a night of raw photons into something you can reason about.

The work splits roughly in two. On one side there is precision: ephemerides, coordinate
transforms, plate solving, refraction — the arithmetic that has to be correct before anything
downstream is worth doing. On the other side there is volume: catalog cross-matching,
photometry across thousands of frames, the kind of problem where the answer only shows up
after the data has been cleaned properly. Both halves are more interesting than they sound.

The rest of it is hardware, and hardware is where the theory goes to get humbled. A mount that
refuses to guide. A camera that silently drops frames. A single-board computer sitting in a cold
box at the far end of a long cable, three hours from the nearest keyboard. Most observatory
software is written for the nights when everything works. I am more interested in the other
nights, because those are the ones that actually cost you data.

So most of what lives in these repos started as a problem I had at 3 a.m. under a bad sky.
The solutions aren't always elegant, but they are tested against reality rather than against
an assumption of it. If you spot something that can be done better, fork it, open a PR, or file
an issue — I'm always up for a better method, and I would rather be corrected than consistent.

Two ideas run underneath nearly all of it:

- **Observation** — you cannot correct what you have not measured. Bias, dark, flat: the boring
  frames are the ones that quietly decide whether the science survives.
- **Propulsion** — a model that never leaves the notebook has zero thrust. Build it, launch it,
  read the telemetry, iterate, and let the failure modes teach you something.

<br clear="right" />

<sub>Artwork: <a href="https://www.behance.net/gallery/37020725/Moonlight-gif-animation">&quot;Moonlight&quot; by Kirokaze</a> — used with permission.</sub>

> *Every photon that lands on the sensor has been travelling for centuries to get here.
> The least I can do is calibrate it properly.*

---

## Current Ops

- **Aperio** — native multi-device app for professional astronomers: high-precision
  ephemeris engine, multi-catalog enrichment (SIMBAD, VizieR, Gaia, 2MASS, AllWISE),
  weather-aware observability scoring, telescope control over ASCOM Alpaca / NINA.
- **Kreiken Observatory** — Python automation stack for remote observing: scheduling,
  plate solving, autoguiding, automated calibration and reduction pipelines.
- **Learning next** — ASCOM Alpaca as a cross-platform REST layer, and Raspberry Pi based
  observatory controllers.

---

## General Info

- **Fun fact**: I build rockets on the ground and photograph the things they aim for.
- **Off-screen**: Electric guitar, airsoft, and far too many clear-sky forecasts.
- **Languages**: Türkçe (native) · English
- **How to reach me**:
  [![Proton Mail](https://img.shields.io/badge/Proton_Mail-6D4AFF?style=for-the-badge&logo=protonmail&logoColor=white)](mailto:korhankara98@pm.me)
  [![Website](https://img.shields.io/badge/korhankara.com-0D1117?style=for-the-badge&logo=safari&logoColor=00D9FF)](https://korhankara.com)

<p align="center">
  <img src="https://img.shields.io/badge/CLEAR%20SKIES-CERTIFIED-00D9FF?style=for-the-badge&labelColor=1B1F24" />
  <img src="https://img.shields.io/badge/CALIBRATED-WITH%20FLATS-00D9FF?style=for-the-badge&labelColor=1B1F24" />
  <img src="https://img.shields.io/badge/POWERED%20BY-PHOTONS%20%26%20COFFEE-FFB400?style=for-the-badge&labelColor=1B1F24" />
  <img src="https://img.shields.io/badge/DEBUGGED%20AT-3%20AM-FF5C5C?style=for-the-badge&labelColor=1B1F24" />
  <img src="https://img.shields.io/badge/CONTAINS%20NO-LIGHT%20POLLUTION-7B68EE?style=for-the-badge&labelColor=1B1F24" />
  <img src="https://img.shields.io/badge/ROCKET-TESTED-E4572E?style=for-the-badge&labelColor=1B1F24" />
</p>

---

## Instruments, tools and stuff

### Operating Systems

![Arch Linux](https://img.shields.io/badge/Arch_Linux-1793D1?style=for-the-badge&logo=archlinux&logoColor=white)
![Ubuntu](https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)
![Fedora](https://img.shields.io/badge/Fedora-294172?style=for-the-badge&logo=fedora&logoColor=white)
![Debian](https://img.shields.io/badge/Debian-A81D33?style=for-the-badge&logo=debian&logoColor=white)
![Tails](https://img.shields.io/badge/Tails-56347C?style=for-the-badge&logo=tails&logoColor=white)
![macOS](https://img.shields.io/badge/macOS-000000?style=for-the-badge&logo=apple&logoColor=white)

### Languages

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Swift](https://img.shields.io/badge/Swift-F05138?style=for-the-badge&logo=swift&logoColor=white)
![R](https://img.shields.io/badge/R-276DC3?style=for-the-badge&logo=r&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white)

### Astronomy & Imaging

![Astropy](https://img.shields.io/badge/Astropy-DE4E2B?style=for-the-badge&logo=python&logoColor=white)
![photutils](https://img.shields.io/badge/photutils-0B3D91?style=for-the-badge&logo=python&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)
![SIMBAD](https://img.shields.io/badge/SIMBAD-1B3A6B?style=for-the-badge&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgc3Ryb2tlPSJ3aGl0ZSIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiPjxlbGxpcHNlIGN4PSIxMiIgY3k9IjUiIHJ4PSI4IiByeT0iMyIvPjxwYXRoIGQ9Ik00IDV2N2MwIDEuNyAzLjYgMyA4IDNzOC0xLjMgOC0zVjUiLz48cGF0aCBkPSJNNCAxMnY3YzAgMS43IDMuNiAzIDggM3M4LTEuMyA4LTN2LTciLz48L3N2Zz4%3D)
![VizieR](https://img.shields.io/badge/VizieR-20486F?style=for-the-badge&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgc3Ryb2tlPSJ3aGl0ZSIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiPjxlbGxpcHNlIGN4PSIxMiIgY3k9IjUiIHJ4PSI4IiByeT0iMyIvPjxwYXRoIGQ9Ik00IDV2N2MwIDEuNyAzLjYgMyA4IDNzOC0xLjMgOC0zVjUiLz48cGF0aCBkPSJNNCAxMnY3YzAgMS43IDMuNiAzIDggM3M4LTEuMyA4LTN2LTciLz48L3N2Zz4%3D)
![Gaia DR3](https://img.shields.io/badge/Gaia_DR3-0A5E7C?style=for-the-badge&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0id2hpdGUiPjxwYXRoIGQ9Ik0xMiAybDIuNyA2LjlMMjIgOS42bC01LjUgNC41TDE4LjMgMjIgMTIgMTguMSA1LjcgMjJsMS44LTcuOUwyIDkuNmw3LjMtLjd6Ii8%2BPC9zdmc%2B)
![ASTAP](https://img.shields.io/badge/ASTAP-14576B?style=for-the-badge&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgc3Ryb2tlPSJ3aGl0ZSIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiPjxjaXJjbGUgY3g9IjEyIiBjeT0iMTIiIHI9IjciLz48Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSIyLjUiLz48cGF0aCBkPSJNMTIgMXY0TTEyIDE5djRNMSAxMmg0TTE5IDEyaDQiLz48L3N2Zz4%3D)
![Siril](https://img.shields.io/badge/Siril-2E5A7D?style=for-the-badge&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0id2hpdGUiPjxwYXRoIGQ9Ik0xMiAybDIuNyA2LjlMMjIgOS42bC01LjUgNC41TDE4LjMgMjIgMTIgMTguMSA1LjcgMjJsMS44LTcuOUwyIDkuNmw3LjMtLjd6Ii8%2BPC9zdmc%2B)
![PixInsight](https://img.shields.io/badge/PixInsight-232A4D?style=for-the-badge&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgc3Ryb2tlPSJ3aGl0ZSIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiPjxwYXRoIGQ9Ik0xMiAyTDIgOGwxMCA2IDEwLTZ6Ii8%2BPHBhdGggZD0iTTIgMTRsMTAgNiAxMC02Ii8%2BPC9zdmc%2B)
![INDI](https://img.shields.io/badge/INDI-006D77?style=for-the-badge&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgc3Ryb2tlPSJ3aGl0ZSIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiPjxwYXRoIGQ9Ik05IDJ2Nk0xNSAydjYiLz48cGF0aCBkPSJNNiA4aDEydjNhNiA2IDAgMCAxLTEyIDB6Ii8%2BPHBhdGggZD0iTTEyIDE3djUiLz48L3N2Zz4%3D)
![KStars](https://img.shields.io/badge/KStars_%2F_Ekos-1D99F3?style=for-the-badge&logo=kde&logoColor=white)
![PHD2](https://img.shields.io/badge/PHD2-2B4162?style=for-the-badge&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgc3Ryb2tlPSJ3aGl0ZSIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiPjxjaXJjbGUgY3g9IjEyIiBjeT0iMTIiIHI9IjciLz48Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSIyLjUiLz48cGF0aCBkPSJNMTIgMXY0TTEyIDE5djRNMSAxMmg0TTE5IDEyaDQiLz48L3N2Zz4%3D)
![ASCOM](https://img.shields.io/badge/ASCOM_Alpaca-5B4B8A?style=for-the-badge&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgc3Ryb2tlPSJ3aGl0ZSIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiPjxjaXJjbGUgY3g9IjEyIiBjeT0iNCIgcj0iMi41Ii8%2BPGNpcmNsZSBjeD0iNCIgY3k9IjE5IiByPSIyLjUiLz48Y2lyY2xlIGN4PSIyMCIgY3k9IjE5IiByPSIyLjUiLz48cGF0aCBkPSJNMTEgNi40TDUuNSAxNi44TTEzIDYuNGw1LjUgMTAuNE02LjUgMTloMTEiLz48L3N2Zz4%3D)
![NINA](https://img.shields.io/badge/N.I.N.A.-34568B?style=for-the-badge&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgc3Ryb2tlPSJ3aGl0ZSIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiPjxwYXRoIGQ9Ik0zIDE1bDExLTYuNSAyLjYgNC41TDUuNiAxOS41eiIvPjxwYXRoIGQ9Ik0xNiA4LjVsMy41LTIgMiAzLjUtMy41IDIiLz48cGF0aCBkPSJNOSAxN3Y1TTEzIDE1LjVWMjIiLz48L3N2Zz4%3D)

### Data Science & ML

![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-8CAAE6?style=for-the-badge&logo=scipy&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

### Mobile & App Development

![SwiftUI](https://img.shields.io/badge/SwiftUI-0071E3?style=for-the-badge&logo=swift&logoColor=white)
![Xcode](https://img.shields.io/badge/Xcode-147EFB?style=for-the-badge&logo=xcode&logoColor=white)
![iOS](https://img.shields.io/badge/iOS-000000?style=for-the-badge&logo=apple&logoColor=white)
![Core Data](https://img.shields.io/badge/Core_Data-2F4858?style=for-the-badge&logo=apple&logoColor=white)

### Hardware & Embedded

![Raspberry Pi](https://img.shields.io/badge/Raspberry_Pi-A22846?style=for-the-badge&logo=raspberrypi&logoColor=white)
![Arduino](https://img.shields.io/badge/Arduino-00979D?style=for-the-badge&logo=arduino&logoColor=white)
![Teensy](https://img.shields.io/badge/Teensy-3E7C5A?style=for-the-badge&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgc3Ryb2tlPSJ3aGl0ZSIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiPjxyZWN0IHg9IjYiIHk9IjYiIHdpZHRoPSIxMiIgaGVpZ2h0PSIxMiIgcng9IjEuNSIvPjxwYXRoIGQ9Ik0xMCAydjRNMTQgMnY0TTEwIDE4djRNMTQgMTh2NE0yIDEwaDRNMiAxNGg0TTE4IDEwaDRNMTggMTRoNCIvPjwvc3ZnPg%3D%3D)
![KiCad](https://img.shields.io/badge/KiCad-314CB0?style=for-the-badge&logo=kicad&logoColor=white)
![XBee](https://img.shields.io/badge/XBee_Telemetry-0B6E8F?style=for-the-badge&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgc3Ryb2tlPSJ3aGl0ZSIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiPjxwYXRoIGQ9Ik0xMiAxMnYxMCIvPjxwYXRoIGQ9Ik04LjUgOC41YTUgNSAwIDAgMSA3IDBNNSA1YTEwIDEwIDAgMCAxIDE0IDAiLz48Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSIxLjYiIGZpbGw9IndoaXRlIi8%2BPC9zdmc%2B)

### Rocketry & CAD

![OpenRocket](https://img.shields.io/badge/OpenRocket-E4572E?style=for-the-badge&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgc3Ryb2tlPSJ3aGl0ZSIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiPjxwYXRoIGQ9Ik0xMiAyYzMuNSAzIDUgNyA1IDExbC01IDQtNS00YzAtNCAxLjUtOCA1LTExeiIvPjxwYXRoIGQ9Ik03IDEzbC0zIDUgNC0xTTE3IDEzbDMgNS00LTEiLz48Y2lyY2xlIGN4PSIxMiIgY3k9IjkiIHI9IjEuOCIgZmlsbD0id2hpdGUiLz48L3N2Zz4%3D)
![SolidWorks](https://img.shields.io/badge/SolidWorks-D71920?style=for-the-badge&logo=dassaultsystemes&logoColor=white)
![MATLAB](https://img.shields.io/badge/MATLAB-0076A8?style=for-the-badge&logo=mathworks&logoColor=white)

### Security & Privacy

![Proton Mail](https://img.shields.io/badge/Proton_Mail-6D4AFF?style=for-the-badge&logo=protonmail&logoColor=white)
![Proton VPN](https://img.shields.io/badge/Proton_VPN-6D4AFF?style=for-the-badge&logo=protonvpn&logoColor=white)
![Tor Browser](https://img.shields.io/badge/Tor_Browser-7D4698?style=for-the-badge&logo=torbrowser&logoColor=white)
![Bitwarden](https://img.shields.io/badge/Bitwarden-175DDC?style=for-the-badge&logo=bitwarden&logoColor=white)
![GnuPG](https://img.shields.io/badge/GnuPG-0093DD?style=for-the-badge&logo=gnuprivacyguard&logoColor=white)

### Browsers & Internet

![Brave](https://img.shields.io/badge/Brave-FB542B?style=for-the-badge&logo=brave&logoColor=white)
![Helium](https://img.shields.io/badge/Helium-2D6CDF?style=for-the-badge&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgc3Ryb2tlPSJ3aGl0ZSIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiPjxjaXJjbGUgY3g9IjEyIiBjeT0iMTIiIHI9IjEwIi8%2BPHBhdGggZD0iTTIgMTJoMjBNMTIgMmExNSAxNSAwIDAgMSAwIDIwYTE1IDE1IDAgMCAxIDAtMjB6Ii8%2BPC9zdmc%2B)
![Firefox](https://img.shields.io/badge/Firefox-FF7139?style=for-the-badge&logo=firefoxbrowser&logoColor=white)
![DuckDuckGo](https://img.shields.io/badge/DuckDuckGo-DE5833?style=for-the-badge&logo=duckduckgo&logoColor=white)

### Platforms & Tooling

![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white)
![Cursor](https://img.shields.io/badge/Cursor-000000?style=for-the-badge&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0id2hpdGUiPjxwYXRoIGQ9Ik01IDJsMTQgOS02LjUgMS40TDkgMjB6Ii8%2BPC9zdmc%2B)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![LaTeX](https://img.shields.io/badge/LaTeX-008080?style=for-the-badge&logo=latex&logoColor=white)

---

<p align="center">
  <sub><code>[LOG] Session closed. Data archived. Clear skies.</code></sub>
</p>
