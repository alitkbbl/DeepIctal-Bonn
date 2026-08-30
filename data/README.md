# Data

Raw recordings from the **Bonn University EEG Dataset** (Andrzejak et al., 2001).

## Layout

```
data/raw/
├── Z/   100 recordings — healthy subjects, eyes open
├── O/   100 recordings — healthy subjects, eyes closed
├── N/   100 recordings — epilepsy patients, interictal (hippocampal)
├── F/   100 recordings — epilepsy patients, interictal (epileptogenic zone)
└── S/   100 recordings — epilepsy patients, ictal (seizure activity)
```

Each file is a single-channel EEG recording: 4097 samples at 173.61 Hz (~23.6 s), one
integer amplitude value per line, no header.

## Class Mapping

| Class | Sets | Label |
|:------|:-----|:-----:|
| Ictal / Seizure | S | 1 |
| Normal / Interictal | Z, O, N, F | 0 |

## Source

Andrzejak, R. G., Lehnertz, K., Mormann, F., Rieke, C., David, P., & Elger, C. E. (2001).
*Indications of nonlinear deterministic and finite-dimensional structures in time series of
brain electrical activity: Dependence on recording region and brain state.*
Physical Review E, 64(6), 061907.
