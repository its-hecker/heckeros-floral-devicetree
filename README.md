# HeckerOS Flame hardware branch

The `flame` branch starts from the current HeckerOS Coral hardware tree at
`8e19009ad632f66473ddcdb10c00595fefdb79b4`. The common source path stays
`device/google/coral`; it contains the original per-device `coral/` and `flame/`
configurations. Original hardware sources, licenses and attribution are retained.

Flame selects its own 1080x2280 display, 440 dpi density, power/thermal/audio
configuration, CHRE vendor namespace and `vendor/google/flame` blobs. Its BoardConfig
includes the same HeckerOS FaceID, Motion Sense and Suite policy as Coral. The camera
module/extraction suffix is `-flame`, retaining the original executable stem.

Both devices use the exact same Floral kernel, including the existing GameSpace
charging controls and KernelSU submodule. ROM features belong to the shared
[HeckerOS integration](https://github.com/its-hecker/HeckerOS/tree/feat/suite-polish).

Build with the [Flame local manifest](https://github.com/its-hecker/HeckerOs-Flame-localmanifest).
Use the `main` device branch for Coral. Full Flame compilation, boot and hardware
acceptance remain pending.
