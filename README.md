# AVR32DA32 Evaluation Board

Altium Designer hardware sources for two revisions of an AVR32DA32 evaluation
board. The original project filenames and local schematic/PCB libraries are
preserved.

| Revision | Altium project |
| --- | --- |
| v1 | [avr32da32_evalboard](v1/avr32da32_evalboard/avr32da32_evalboard.PrjPcb) |
| v2 | [avr32da32_board_V2](v2/avr32da32_board_V2/avr32da32_board_V2.PrjPcb) |

## Open a design

Open the `.PrjPcb` for the intended revision in Altium Designer. Each revision
includes its `.SchDoc`, `.PcbDoc` and the supplied `.SchLib`/`.PcbLib` files.
Confirm the project's library search paths on your machine before editing.

The directories named `Project Outputs for ...` contain the existing Gerber,
drill, manufacturing and report files referenced by the Altium projects. They
are historical exports, not a new design-rule or fabrication approval. Regenerate
them from the intended PCB revision before a new fabrication run.

## Scope

This repository contains the AVR32DA32 board designs. It excludes the neighboring
SAMD21 projects, Altium-generated previews/history/logs and the original
Altium-managed Git metadata. The source Altium repositories are preserved
separately, including their existing remotes and uncommitted changes.

The v2 PCB snapshot includes the local PCB edits present at export time. Hardware
sources are copied without changing their contents. No firmware is bundled here;
the rotary-cylinder application's AVR32DA32 firmware is maintained with that
application. Use the chosen board's schematic to verify power, UPDI, UART and
header connections before programming or attaching peripherals.
