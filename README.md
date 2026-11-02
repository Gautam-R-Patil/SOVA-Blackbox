<div align="center">

# SOVA Black Box

**A 24x7 recorder for AI systems in production.**

Closed source · for companies running AI in production and OEM partners · by [TRUSCOR](https://truscor.org)

</div>

---

## What it does

Aviation needed the flight recorder. Autonomous AI needs one too.

SOVA Black Box **logs every action and failure of a live AI system, signed and checked against its real effect**, so fault can be proven later, in court if needed.

- **Signed:** each record is tamper-evident, in the open `.sova` format.
- **Effect-verified:** it records what actually changed, not only what the AI said it did.
- **Built for investigation:** records support replay and fault-finding after an incident.

## Where it fits in the SOVA stack

| Part | Role |
|---|---|
| **SOVA Black Box** | Records AI systems in production |
| [SOVA Engine](https://github.com/TRUSCOR/SOVA-Engine) | Tests AI products before and during deployment |
| [O.W.L](https://github.com/TRUSCOR/O.W.L) | The measurement instrument: checks claims against real effects |
| [TAFAAR](https://github.com/TRUSCOR/TAFAAR) | Grades evidence into the TRUSCOR Rating |
| [SOVA OSS](https://github.com/TRUSCOR/SOVA-OSS) | The free, open-source toolkit and the open `.sova` format |

## About this repository

This repository holds public information and demo material for SOVA Black Box. **The recorder's source code is private.**

## See the open part run today

```bash
git clone https://github.com/TRUSCOR/SOVA-OSS
cd SOVA-OSS
uv sync --locked
uv run sova demo sleeper
```

## Contact

[truscor.org](https://truscor.org)

---

© 2026 TRUSCOR Private Limited. All rights reserved.
