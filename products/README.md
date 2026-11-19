# Products

My own device configs. The example configs from upstream stay in the repo root.

## In use

| File | Device | Purpose |
|---|---|---|
| `esp32c3-backup-power-system.yaml` | `bps` (ESP32-C3) | Anenji inverter over Modbus and JK BMS over BLE on one board. The only device that runs now. |

## Tools

| File | Purpose |
|---|---|
| `esp32c3-anenji.protocol-test.yaml` | Small config to test the Anenji Modbus protocol. Flash it only for a test: it uses the device name `anenji`, not `bps`. |

## Archive

Not flashed anywhere. Kept as history and reference.

| File | What it was | Why archived |
|---|---|---|
| `archive/esp32c3-anenji.full-general.yaml` | Inverter-only config, device `anenji` | The inverter part of `bps` grew from it. The separate `anenji` device does not run any more. |
| `archive/esp32c3-anenji.full.yaml` | Earlier inverter-only config | Replaced by `full-general`. |
| `archive/esp32c3-anenji-jkble-hybrid.example.yaml` | Hybrid example from another author (ESP-IDF, other BMS) | Reference only. `bps` is my own hybrid. |

## Removed

- `esp32c3-anenji.full-second.yaml`: an abandoned experiment.
- `esp32c3-anenji.example.yaml`: the same file as `esp32-example-anenji.yaml`
  in the repo root.
- `bk7231m-anenjk.example.yaml`: the same file as `bk7231m-example-anenji.yaml`
  in the repo root.

## Related

The BMS-only configs live in the `esphome-jk-bms` fork, under
`products/archive/`. `bps` replaced them too.
