# Fork and GPL-2.0 notice

This repository is a fork of
[jetm/mediatek-mt7927-dkms](https://github.com/jetm/mediatek-mt7927-dkms).
It remains licensed as **GPL-2.0-only** under the unmodified
[LICENSE](LICENSE) file.

## Changes in this fork

Changes made on 2026-07-16 are documentation-only:

- `README.md`: fork identification plus Fedora/Nobara recovery guidance.
- `FC44_MT7927_RECOVERY_LOG.md`: local operational recovery record.
- `FORK_NOTICE.md`: this notice.

The driver source, patches, build scripts, existing copyright notices, and
license identifiers are retained. Do not remove or replace notices in source
files or imported patches.

## If distributing a modified build or RPM

GPL-2.0 requires a distributor of object code to provide the complete
corresponding source under GPL-2.0. For a release from this fork, that means:

1. Tag or otherwise identify the exact fork commit used to build the RPM.
2. Publish the matching source, including patches, firmware-extraction/build
   scripts, packaging files, and this `LICENSE`, under GPL-2.0.
3. Make the source available from the same release location as the RPM, or
   include a valid GPL-2.0 source offer where applicable.
4. State that the release is modified and comes with no warranty, as the
   GPL-2.0 license says.

No binary release is published from this fork at present. A public source
repository alone is not enough for a later binary release unless it identifies
and provides the exact corresponding source for that binary.

This is an operational compliance checklist, not legal advice.
