# Electrical Wiring

## Circuit Diagram (schematic description)

```
Solar Panel (+)  ──► Solar Charge Controller PV(+)
Solar Panel (-)  ──► Solar Charge Controller PV(-)

Solar Charge Controller BAT(+) ──► Battery (+)
Solar Charge Controller BAT(-)  ──► Battery (-)

Battery (+)
    │
   Fuse
    │
 ON/OFF Switch
    │
 DC Motor (+)

Battery (-) ──────────────────► DC Motor (-)
```

## Load Circuit Rules

| Rule | Reason |
|------|--------|
| All 12V current through screw terminals | Breadboard strips only handle ~1A; motor draws up to 5A+ |
| Fuse between battery (+) and switch | Overcurrent protection for motor and wiring |
| Wire size: minimum 1.5mm² for load | Motor startup current can be 3–5× running current |
| Solar charge controller between panel and battery | Prevents battery overcharge and over-discharge |

## Component Connections

### Solar Charge Controller
| Controller Terminal | Connects to |
|--------------------|-------------|
| PV+ | Solar panel (+) |
| PV− | Solar panel (−) |
| BAT+ | Battery (+) |
| BAT− | Battery (−) |
| LOAD+ | Optional load output |
| LOAD− | Optional load output |

### Motor Circuit
| Point | Connects to |
|-------|-------------|
| Battery (+) | Fuse → Switch → Motor (+) |
| Battery (−) | Motor (−) |

> ⚠️ Final wiring diagram will be finalized after inspecting actual component terminal positions.
