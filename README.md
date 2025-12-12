English Version | [中文版](README-zh_CN.md)

---

# PH-AC Release 3.0

PH-AC is an open-source 7-button + 2-encoder arcade controller based on RP2040, optimized for rhythm/music games. Release 3.0 preserves the 7-button + 2-encoder layout while adding 3D/PCB/CAD resources, customizable RGB key lighting, and additional GPIO breakouts for easier DIY mods and mass production.

## Project Structure
```
PH60 Rev.2
├── Case_Model_Rev2                 # Case 3D model files
├── LICENSE                         # Project license
├── PCB_Model_Rev2                  # PCB 3D model files
├── PCB_Rev2                        # PCB design files
├── Plate                           # Plate files
├── Preview                         # Preview images
├── Production                      # Production files
├── README-zh_CN.md                 # Chinese README
└── README.md                       # English README
```

Rev3 is mainly aimed at organizing 3D, PCB and production resources and pairs with our new firmware PHAC_Firmware:

https://github.com/ph-design/phac_firmware

Detailed hardware descriptions, assembly instructions, firmware configuration, and maintenance recommendations have been migrated to the official wiki:

https://wiki.phdesign.cc/PHAC/

The hardware project is mature and will not receive further updates.

## Preview

<p align="center">
	<img src="./pic/main.jpg" alt="PH-AC front view" width="480" />
	<img src="./pic/encoder.jpg" alt="PH-AC PCB" width="320" />
	<img src="./pic/back_with_feet.jpg" alt="PH-AC case" width="320" />
</p>

---

## Release Highlights

- **Rev3 Hardware**: Added per-key RGB lighting and external GPIO breakouts so you can add almost anything you want.
- **Production Files & BOM**: Files prepared for JLCPCB; generate other formats from the KiCad sources if needed.
- **Firmware Evolution**: Rev3 uses our own [PHAC_firmware](https://github.com/ph-design/phac_firmware), which is more suited for arcade-style games than QMK, though older QMK-based firmware remains usable.

## Maintenance Notes

- Avoid applying excessive force to the encoders to prolong their life.
- The top cover fits 4.5mm low-profile encoders; standard-height encoders may interfere with the pins.
- The PCB does not include additional encoder debouncing circuitry; we recommend using high-quality PEC11L encoders and light lubrication.
- If encoder bounce or backdrive occurs, apply a small drop of 400cs silicone oil to the bottom and repeatedly press/rotate the knob to distribute the lubricant.

## License & Community

- License: Creative Commons BY-NC-SA 4.0.
- Documentation & support: https://wiki.phdesign.cc/PHAC/

Thanks to everyone who contributed, tested, and provided feedback — this was our debut project. This is only the beginning: we look forward to seeing what you create, modify, or remix from here. Inject your ideas, share your builds, and help the project live on through community creativity.