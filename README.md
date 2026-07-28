<p align="center">
  <img src="https://img.shields.io/badge/STATUS-OBSERVING-00D9FF?style=for-the-badge&labelColor=0D1117" />
  <img src="https://img.shields.io/badge/MOUNT-TRACKING-00D9FF?style=for-the-badge&labelColor=0D1117" />
  <img src="https://img.shields.io/badge/DOMAIN-ASTRO%20%2F%20AEROSPACE-00D9FF?style=for-the-badge&labelColor=0D1117" />
  <img src="https://img.shields.io/badge/SITE-ANKARA%2039.9%C2%B0N-00D9FF?style=for-the-badge&labelColor=0D1117" />
</p>

```diff
+ [LOG] Dome opened. Mount slewing to target...
+ [LOG] Plate solve OK — RA 05h35m17s / DEC -05°23'28" locked.
! [WARN] Seeing 3.4" and rising. Increasing guide exposure.
- [ERR] Cloud sensor tripped at 78%. Sequence paused.
+ [LOG] Calibration frames applied. Signal is clean. Welcome in.
```

# Welcome to the observation deck

Astronomer and data scientist based in Ankara. I spend most of my time in the narrow strip
where celestial mechanics, signal processing and shipping actual software overlap — writing
the code that turns a night of raw photons into something you can reason about.

Most of what lives in these repos started as a problem I had at 3 a.m. under a bad sky: a mount
that wouldn't guide, a catalog query that took too long, a frame stack that refused to calibrate.
The solutions aren't always elegant, but they are tested against reality. If you spot something
that can be done better, fork it, open a PR, or file an issue — I'm always up for a better method.

- **Observation** — you cannot correct what you have not measured. Bias, dark, flat: the boring
  frames are the ones that decide whether the science survives.
- **Propulsion** — a model that never leaves the notebook has zero thrust. Build it, launch it,
  read the telemetry, iterate.

> *Every photon that lands on the sensor has been travelling for centuries to get here.
> The least I can do is calibrate it properly.*

## Current Ops

- **Aperio** — native iOS app (Swift / SwiftUI) for professional astronomers: high-precision
  ephemeris engine, multi-catalog enrichment (SIMBAD, VizieR, Gaia, 2MASS, AllWISE),
  weather-aware observability scoring, telescope control over ASCOM Alpaca / NINA.
- **Kreikon Observatory** — Python automation stack for remote observing: scheduling,
  plate solving, autoguiding, automated calibration and reduction pipelines.
- **Learning next** — ASCOM Alpaca as a cross-platform REST layer, and Raspberry Pi based
  observatory controllers.

## General Info

- **Fun fact**: I build rockets on the ground and photograph the things they aim for.
  Teknofest veteran — M-class solid motor, carbon fiber airframe, custom flight computer.
- **Off-screen**: electric guitar, airsoft, and far too many clear-sky forecasts.
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

## Instruments, tools and stuff

### Languages

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Swift](https://img.shields.io/badge/Swift-F05138?style=for-the-badge&logo=swift&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=black)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white)

### Astronomy & Imaging

![Astropy](https://img.shields.io/badge/Astropy-DE4E2B?style=for-the-badge&logo=python&logoColor=white)
![photutils](https://img.shields.io/badge/photutils-0B3D91?style=for-the-badge)
![SIMBAD](https://img.shields.io/badge/SIMBAD-1B2A4A?style=for-the-badge)
![VizieR](https://img.shields.io/badge/VizieR-1B2A4A?style=for-the-badge)
![Gaia](https://img.shields.io/badge/Gaia_DR3-003247?style=for-the-badge)
![ASTAP](https://img.shields.io/badge/ASTAP-2E3440?style=for-the-badge)
![Siril](https://img.shields.io/badge/Siril-4C566A?style=for-the-badge)
![PixInsight](https://img.shields.io/badge/PixInsight-1A1A2E?style=for-the-badge)
![INDI](https://img.shields.io/badge/INDI-005F73?style=for-the-badge)
![KStars](https://img.shields.io/badge/KStars_%2F_Ekos-1D99F3?style=for-the-badge&logo=kde&logoColor=white)
![PHD2](https://img.shields.io/badge/PHD2-2B2D42?style=for-the-badge)
![ASCOM Alpaca](https://img.shields.io/badge/ASCOM_Alpaca-6A4C93?style=for-the-badge)
![NINA](https://img.shields.io/badge/N.I.N.A.-3A506B?style=for-the-badge)

### Data Science & ML

![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-8CAAE6?style=for-the-badge&logo=scipy&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

### Mobile & App Development

![Swift](https://img.shields.io/badge/SwiftUI-0071E3?style=for-the-badge&logo=swift&logoColor=white)
![Xcode](https://img.shields.io/badge/Xcode-147EFB?style=for-the-badge&logo=xcode&logoColor=white)
![iOS](https://img.shields.io/badge/iOS-000000?style=for-the-badge&logo=apple&logoColor=white)
![Core Data](https://img.shields.io/badge/Core_Data-2F4858?style=for-the-badge&logo=apple&logoColor=white)

### Hardware & Embedded

![Raspberry Pi](https://img.shields.io/badge/Raspberry_Pi-A22846?style=for-the-badge&logo=raspberrypi&logoColor=white)
![Arduino](https://img.shields.io/badge/Arduino-00979D?style=for-the-badge&logo=arduino&logoColor=white)
![Teensy](https://img.shields.io/badge/Teensy-B31942?style=for-the-badge)
![KiCad](https://img.shields.io/badge/KiCad-314CB0?style=for-the-badge&logo=kicad&logoColor=white)
![XBee](https://img.shields.io/badge/XBee_Telemetry-004B87?style=for-the-badge)

### Rocketry & CAD

![OpenRocket](https://img.shields.io/badge/OpenRocket-E4572E?style=for-the-badge)
![Fusion 360](https://img.shields.io/badge/Fusion_360-F58220?style=for-the-badge&logo=autodesk&logoColor=white)
![SolidWorks](https://img.shields.io/badge/SolidWorks-D71920?style=for-the-badge&logo=dassaultsystemes&logoColor=white)
![MATLAB](https://img.shields.io/badge/MATLAB-0076A8?style=for-the-badge&logo=mathworks&logoColor=white)

### Platforms & Tooling

![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![macOS](https://img.shields.io/badge/macOS-000000?style=for-the-badge&logo=apple&logoColor=white)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white)
![LaTeX](https://img.shields.io/badge/LaTeX-008080?style=for-the-badge&logo=latex&logoColor=white)

## Telemetry

<p>
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=korhankara98&show_icons=true&theme=github_dark&hide_border=true&icon_color=00D9FF&title_color=00D9FF" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=korhankara98&layout=compact&theme=github_dark&hide_border=true&title_color=00D9FF" />
</p>

---

<sub>`[LOG] Session closed. Data archived. Clear skies.`</sub>
