# SSDT-GPU-SPOOF

Renaming RX 550 (Lexa) to RX 560 (`1002:67ff`)

## Note

It works fine on Catalina but has no hardware acceleration on Monterey.

It was then fixed by disabling this SSDT and adding a Dictionary to DeviceProperties

| Key | Type | Value |
| --- | --- | --- |
| device-id | Data | FF670000 |
| model | String | AMD Radeon RX 550 |
| no-gfx-spoof | Data | 01000000 |
