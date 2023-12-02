# KiCad-DRC

Design Rules for KiCad 7.0, implemented as Custom Rules in PCB Editor `File > Board_Setup... > Design Rules > Custom Rules`), and stored in the `.kicad_dru` file.

These rules use some features only available in KiCad 7.0.

Each design rule is validated for PASS/FAIL the associated PCB (`.kicad_pcb`).

## Manufacturer Rules

Currently this project provides rule files for the following manufacturers:

### JLCPCB

- [Official Capabilities](https://jlcpcb.com/capabilities/pcb-capabilities)
- ~~Official Design Rules~~

The JLCPCB [rule file](JLCPCB/JLCPCB.kicad_dru) is found at: `JLCPCB/JLCPCB.kicad_dru`.

### PCBWay

- [Official Capabilities](https://www.pcbway.com/capabilities.html)
- [Official Design Rules](https://www.pcbway.com/pcb_prototype/PCB_Design_Rule_Check.html)

The PCBWay [rule file](PCBWay/PCBWay.kicad_dru) is found at: `PCBWay/PCBWay.kicad_dru`.

## Use in your KiCad 7 project

Simply pick the manufacturer of your choice and copy the corresponding `<MANUFACTURER>/<MANUFACTURER>.kicad_dru`(e.g. `JLCPCB/JLCPCB.kicad_dru`) file into your KiCad 7 project folder, and rename it to match your project name, e.g. `your-project.kicad_dru`.

The Design Rules will automatically be included in the KiCad PCB Editor (`File`>`Board Setup...`>`Design Rules`>`Custom Rules`), and be included when performing a [Design Rules Check (DRC)](https://docs.kicad.org/7.0/en/pcbnew/pcbnew.html#design_rule_checking) (`Ìnspect`>`Design Rules Checker`).

For more info on how to use custom design rules in KiCad 7.0+ see the correpsonding [KiCAD documentation](https://docs.kicad.org/7.0/en/pcbnew/pcbnew.html#custom_design_rules).
