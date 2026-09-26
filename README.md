# Solar Powered Grass Cutter ☀️🌿

**Compact, eco-friendly grass cutting machine powered entirely by solar energy.**

No grid connection. No fuel. No emissions. Just sunlight → battery → blade.

---

## System Architecture

```
        ☀️ SOLAR PANEL
               │
               ▼
      SOLAR CHARGE CONTROLLER
               │
               ▼
           🔋 BATTERY
               │
               ▼
             FUSE
               │
               ▼
          ON/OFF SWITCH
               │
               ▼
           ⚙️ DC MOTOR
               │
               ▼
           MOTOR SHAFT
               │
               ▼
           🔪 CUTTING BLADE
            🛡️ BLADE GUARD

       🛞 FRAME + WHEELS + HANDLE
```

---

## Electrical Wiring

```
Solar Panel (+/−)
       │
       ▼
Solar Charge Controller
  BAT(+) ──► Battery (+)
  BAT(−) ──► Battery (−)

Battery (+)
  │
 Fuse
  │
ON/OFF Switch
  │
Motor (+)

Battery (−) ──────────► Motor (−)
```

> ⚠️ Actual terminal connections finalized after hardware inspection.

---

## Components

| Component | Purpose |
|-----------|---------|
| Solar Panel (~20–50W) | Converts sunlight to electrical energy |
| Solar Charge Controller | Manages safe battery charging |
| Rechargeable Battery (12V) | Stores energy |
| DC Motor (12V high-speed) | Rotates cutting blade |
| Cutting Blade (150–250mm) | Cuts grass |
| Motor Shaft | Transfers rotation to blade |
| Blade Guard | Operator safety |
| Fuse | Overcurrent protection |
| ON/OFF Switch | Operation control |
| Frame (mild steel/aluminium) | Structural support |
| Wheels (2 or 4) | Mobility |
| Handle | Operator control |

**Estimated budget:** ₹9,000 – ₹12,000

---

## Working Principle

1. Solar panel receives sunlight → converts to electrical energy
2. Charge controller manages battery charging safely
3. Battery stores energy
4. Switch ON → battery powers DC motor
5. Motor rotates blade through shaft
6. Operator moves machine via handle and wheels
7. Rotating blade cuts grass
8. Blade guard provides operator protection

---

## Development Phases

| Phase | What | Status |
|-------|------|--------|
| Phase 1 | Hardware identification — receive and record all components | 🚧 In progress |
| Phase 2 | Electrical design — wiring, fuse rating, wire sizing | 📋 Planned |
| Phase 3 | Mechanical assembly — frame → wheels → motor → blade | 📋 Planned |
| Phase 4 | Progressive testing — solar → controller → battery → motor → blade | 📋 Planned |
| Phase 5 | Final prototype and measurements | 📋 Planned |

---

## Testing Plan

Real measurements to be recorded from prototype (not assumed):

- [ ] Solar panel open-circuit voltage
- [ ] Battery voltage (full / empty)
- [ ] Charging current and time
- [ ] Motor operating voltage and current
- [ ] Runtime on full charge
- [ ] Cutting performance (grass type, blade height)
- [ ] Mechanical stability and vibration
- [ ] Safety observations

Results will be logged in [testing/test-results.md](testing/test-results.md)

---

## Applications

- 🌿 Gardens and lawns
- 🌾 Small agricultural fields
- 🏫 College and school grounds
- 🏞️ Parks and playgrounds
- 🏡 Residential gardens
- 🛣️ Roadside grass maintenance

---

## Repo Structure

```
solar-grass-cutter/
├── README.md
├── hardware/
│   ├── components.md       ← component list with actual specs (after delivery)
│   └── wiring-diagram/     ← circuit diagram files
├── testing/
│   └── test-results.md     ← real measurements from prototype
└── images/
    ├── prototype/
    └── assembly/
```

---

By Maruthi R M — ECE Student, Malnad College of Engineering, Hassan, Karnataka
[RuralSense Labs](https://github.com/maruthirm333-prog/ruralsense-labs)
