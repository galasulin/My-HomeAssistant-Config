# My-HomeAssistant-Config (fork)

> **This is a fork, not my own setup.** It tracks [**abeksis/My-HomeAssistant-Config**](https://github.com/abeksis/My-HomeAssistant-Config), which builds on [**HomeKit Infused (HKI)**](https://github.com/jimz011/homekit-infused) by [Jimz011](https://github.com/jimz011). The configuration, dashboards and screenshots below are the upstream author's work. I keep this fork in sync as a reference for HKI dashboard patterns.
>
> My own smart home (Home Assistant OS, Gemini vision at the front door, Home Front Command automation, a Telegram bot) is documented in **[smart-home-showcase](https://github.com/galasulin/smart-home-showcase)**.

---

## 📋 Overview / סקירה

🇬🇧 The upstream author's Home Assistant configuration: HKI-based mobile dashboards, packages and automations, running in Docker on Unraid.

‏🇮🇱 הקונפיגורציה של Home Assistant של מחבר הריפו המקורי (abeksis): דשבורדים לנייד מבוססי HKI, packages ואוטומציות, רצה ב-Docker על Unraid. זה fork לעיון, לא הבית שלי.

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

## 🖼️ Screenshots (upstream)

| Home dashboard | Energy / electricity |
| -------------- | -------------------- |
| ![Home](HA_Pictures/Lovelace_Screenshots/home.jpg) | ![Electricity](HA_Pictures/Lovelace_Screenshots/electricity_use.jpg) |

| Quick access | Unraid server |
| ------------ | ------------- |
| ![Quick access](HA_Pictures/Lovelace_Screenshots/Quick_access.jpg) | ![Unraid](HA_Pictures/Lovelace_Screenshots/unraid.jpg) |

---

## 🚀 Getting started

> ⚠️ This is the upstream author's personal configuration. Treat it as a reference, not a drop-in install — paths, entity IDs and secrets are specific to their hardware.

1. Install [Home Assistant](https://www.home-assistant.io/installation/) (upstream runs it in Docker on Unraid).
2. Review `HomeAssistant_File/configuration/` and adapt entity IDs to your own devices.
3. Copy the `packages/` you want into your config and enable packages in `configuration.yaml`.
4. Never commit secrets — keep tokens and passwords in `secrets.yaml` (git-ignored).

---

## 🙏 Credits (upstream)

- [**Jimz011**](https://github.com/jimz011) — creator of HomeKit Infused, the foundation of this dashboard.
- [**abeksis**](https://github.com/abeksis) — the configuration this fork is based on.
- [**Noodlemctwoodle**](https://github.com/noodlemctwoodle) — Unraid ↔ Home Assistant integration help.

## 📚 Reference

- [HomeKit Infused documentation](https://jimz011.github.io/homekit-infused/)
- [Home Assistant documentation](https://www.home-assistant.io/docs/)

---

<sub>⭐ If this helped you, star the [upstream repository](https://github.com/abeksis/My-HomeAssistant-Config).</sub>
