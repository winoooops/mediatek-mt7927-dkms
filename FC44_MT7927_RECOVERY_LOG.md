# Fedora 44 / Nobara MT7927 recovery log

Date: 2026-07-16

## Result

- System: Nobara 44, kernel `7.1.3-200.nobara.fc44.x86_64`.
- Hardware: MediaTek MT7927 PCIe Wi-Fi (`14c3:7927`).
- Installed upstream release: `mediatek-mt7927-dkms-2.13-1.fc44.noarch`.
- DKMS confirms v2.13 installed for the running kernel.
- Loading `mt7925e` restored the `wlp9s0` Wi-Fi interface and network connectivity.

## Important module name

`mt7927` is the hardware/combo-module name, not the Linux Wi-Fi module name.

```bash
sudo modprobe mt7925e
```

## What was cleaned up

The obsolete v2.11 DKMS registration was removed from the old Fedora 43
kernels. This prevents it from failing to build against Fedora 44.

If systemd still displays the historical boot-time DKMS failure, clear and
recheck it with:

```bash
sudo systemctl reset-failed dkms.service && sudo systemctl start dkms.service
```

This log is local operational context for this fork; it is not an upstream bug report.
