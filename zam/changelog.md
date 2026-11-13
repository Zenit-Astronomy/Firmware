# Zenit Align Mini – Changelog

Each section lists what changed since the version before it. The update file
of every version is attached to its
[release](https://github.com/Zenit-Astronomy/Firmware/releases).

## 0.1.0-rc3 – 2026-11-13

Release: [zam-0.1.0-rc3](https://github.com/Zenit-Astronomy/Firmware/releases/tag/zam-0.1.0-rc3) ·
Update file: `zenit-align-mini-0.1.0-rc3-d56fc29-20261113.raucb`

### New

- Polar alignment in the southern hemisphere: the device aligns to the south
  celestial pole when it is south of the equator.
- Polar alignment at low latitudes: when the pole is low in the sky, the mount
  raises the scope quickly and reliably through its lowest range.
- Support for a second camera module. The fitted camera is detected
  automatically at startup.
- Redesigned web interface for phone and desktop, in English, German, Czech
  and Chinese.
- Password protection for remote access to the web interface; the hotspot
  password can now be changed.
- The display shows calibration progress and readings, and a dedicated screen
  while the mount is moving.
- The device asks to update the mount controller when its firmware is outdated.

### Improved

- Compass calibration returns to its starting position, stays within the
  mount's rotation range and checks its result again.
- The level check no longer mistakes small resting vibrations for movement.
- Faster automatic exposure, with exposures of up to 3 seconds.
- The update page shows the installed version and the reason when an update
  fails.
- Updated base system and Linux kernel.

### Fixed

- Small GPS position changes no longer invalidate a plate solve.
- A plate solve that cannot be used no longer breaks the home page.
- WiFi stays responsive over long sessions.
- The status LED works again.
- The hotspot works with more phones and tablets.
- A factory reset also removes the hotspot settings and the web password.

## 0.1.0-rc2 – 2026-10-26

Release: [zam-0.1.0-rc2](https://github.com/Zenit-Astronomy/Firmware/releases/tag/zam-0.1.0-rc2) ·
Update file: `zenit-align-mini-0.1.0-rc2-8096d7c-20261026.raucb`

### New

- Motor speed setting: slow, medium or fast.
- The settings show the name and version of the installed system.
- A manually entered location is kept and used until GPS has a position. A
  phone's location is checked against a trusted time, and the last known
  coordinates can be used again.

### Fixed

- WiFi starts in the mode chosen by the user (hotspot or home network).
- A manually entered location is always applied.
- The first plate solve after a movement uses a fresh camera frame.
- Updates: late messages are kept in the update log, and the restart button is
  always available.
- Recovering the system no longer depends on the state of the mount
  controller.
- Disabled switches display correctly, and the status refresh only appears
  after 10 seconds without an answer.

## 0.1.0-rc1 – 2026-10-26

Release: [zam-0.1.0-rc1](https://github.com/Zenit-Astronomy/Firmware/releases/tag/zam-0.1.0-rc1) ·
Update file: `zenit-align-mini-v0.1.0-rc1.raucb`

- First release candidate of the Zenit Align Mini firmware.
