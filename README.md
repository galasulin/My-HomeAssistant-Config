# 🏠 My Home Assistant Configuration

My personal **Home Assistant** setup — packages, Lovelace dashboards and automations for a mobile-first smart home, running in **Docker** on an **Unraid** server.

> This repository is a personalized fork of [**abeksis/My-HomeAssistant-Config**](https://github.com/abeksis/My-HomeAssistant-Config), which itself builds on the excellent [**HomeKit Infused (HKI)**](https://github.com/jimz011/homekit-infused) project by [Jimz011](https://github.com/jimz011). Full credit to the original authors — see [Credits](#-credits).

---

## 📋 Overview / סקירה

🇬🇧 A clean, opinionated Home Assistant configuration focused on a polished mobile dashboard and reliable automations. Everything is containerized for easy backup and recovery.

🇮🇱 קונפיגורציה של Home Assistant לבית חכם, עם דגש על דשבורד נייד נקי ואוטומציות יציבות. הכול רץ ב‑Docker על שרת Unraid לגיבוי ושחזור קלים.

---

## 🧱 Stack

| Layer        | Technology                                                          |
| ------------ | ------------------------------------------------------------------- |
| Platform     | Home Assistant                                                      |
| Host         | Unraid server                                                       |
| Runtime      | Docker container                                                    |
| UI framework | [HomeKit Infused (HKI)](https://github.com/jimz011/homekit-infused) |

---

## 📁 Repository structure

```
.
├── HomeAssistant_File/        # The Home Assistant config root
│   ├── configuration.yaml     # Main entry point
│   ├── configuration/         # Split YAML (automations, alarm, sensors, …)
│   ├── packages/              # Modular feature packages
│   ├── custom_components/     # Custom / HACS integrations
│   ├── homekit-infused/       # HKI dashboard base
│   ├── themes/                # Lovelace themes
│   ├── image/  &  www/        # Local assets served by HA
├── HA_Pictures/               # Screenshots & images
│   ├── HA_Screenshots/        # App screenshots
│   ├── Lovelace_Screenshots/  # Dashboard screenshots
│   ├── Images_for_packages/   # Images used inside packages
│   └── Github_Pictures/       # Images used in this README
└── README.md
```

---

## 🖼️ Screenshots

| Home dashboard | Energy / electricity |
| -------------- | -------------------- |
| ![Home](HA_Pictures/Lovelace_Screenshots/home.jpg) | ![Electricity](HA_Pictures/Lovelace_Screenshots/electricity_use.jpg) |

| Quick access | Unraid server |
| ------------ | ------------- |
| ![Quick access](HA_Pictures/Lovelace_Screenshots/Quick_access.jpg) | ![Unraid](HA_Pictures/Lovelace_Screenshots/unraid.jpg) |

---

## 🚀 Getting started

> ⚠️ This is my personal configuration. Treat it as a reference, not a drop-in install — paths, entity IDs and secrets are specific to my hardware.

1. Install [Home Assistant](https://www.home-assistant.io/installation/) (this setup runs it in Docker).
2. Review `HomeAssistant_File/configuration/` and adapt entity IDs to your own devices.
3. Copy the `packages/` you want into your config and enable packages in `configuration.yaml`.
4. Never commit secrets — keep tokens and passwords in `secrets.yaml` (git-ignored).

---

## 🙏 Credits

- [**Jimz011**](https://github.com/jimz011) — creator of HomeKit Infused, the foundation of this dashboard.
- [**abeksis**](https://github.com/abeksis) — the configuration this fork is based on.
- [**Noodlemctwoodle**](https://github.com/noodlemctwoodle) — Unraid ↔ Home Assistant integration help.

## 📚 Reference

- [HomeKit Infused documentation](https://jimz011.github.io/homekit-infused/)
- [Home Assistant documentation](https://www.home-assistant.io/docs/)

---

<sub>⭐ Star this repo if it helped you set up your own smart home.</sub>
