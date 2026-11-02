<div align="center">

# SOVA Black Box

**A 24x7 recorder for AI systems in production.**

<p>
  <img src="https://img.shields.io/badge/STATUS-CLOSED%20SOURCE-172B4D?style=for-the-badge" alt="Closed source" />
  <img src="https://img.shields.io/badge/FORMAT-.sova%20OPEN-00B8D9?style=for-the-badge" alt="Open format" />
  <img src="https://img.shields.io/badge/FOR-PRODUCTION%20%26%20OEM-6554C0?style=for-the-badge" alt="For production" />
  <a href="https://truscor.org"><img src="https://img.shields.io/badge/TRUSCOR-PROJECT%20HOME-0B8793?style=for-the-badge" alt="TRUSCOR" /></a>
</p>

</div>

---

## Aviation needed the flight recorder

It did not get one because flying was unsafe. It got one because when something
went wrong, nobody could prove what happened — and an industry that cannot
assign fault cannot improve, insure, or be trusted with human lives.

Autonomous AI is in that period now. A system takes an action, money moves, a
record changes, a customer is harmed. Afterwards there is a log nobody signed,
a model that has since been updated, and two parties with incompatible accounts
of the same event.

**SOVA Black Box is the recorder for that problem.**

## What it does

It logs every action and failure of a live AI system, **signed and checked
against its real effect**, so fault can be proven later — in court if it comes
to that.

| | |
|---|---|
| **Signed** | Every record is tamper-evident, written in the open `.sova` format. |
| **Effect-verified** | It records what actually changed, not only what the AI reported doing. |
| **Built for investigation** | Records support replay and fault-finding after an incident, not just dashboards during one. |
| **Continuous** | 24x7, in production, not a test window. |

The distinction that matters: an agent's own report of its actions is a claim.
The Black Box records the claim **and** the effect, separately, so the two can
be compared by someone who was not there.

## Where it sits in the stack

| Layer | Role |
|---|---|
| **SOVA Black Box** | Records AI systems in production |
| [SOVA Engine](https://github.com/TRUSCOR/SOVA-Engine) | Tests AI products before and during deployment |
| [O.W.L](https://github.com/TRUSCOR/O.W.L) | The measurement instrument: checks claims against real effects |
| [TAFAAR](https://github.com/TRUSCOR/TAFAAR) | Grades evidence into the TRUSCOR Rating (300-900) |
| [SOVA OSS](https://github.com/TRUSCOR/SOVA-OSS) | The free, open-source toolkit and the open `.sova` format |

## About this repository

This repository holds public information and demo material for SOVA Black Box.
**The recorder's source code is private.** Nothing here is taken from it.

## See the open layer run today

The `.sova` format the recorder writes is open, and so is a working demo of it.
No model, API key or network required:

```bash
git clone https://github.com/TRUSCOR/SOVA-OSS
cd SOVA-OSS
uv sync --locked
uv run sova demo sleeper
```

## Contact

For production deployments and OEM partnerships: **[truscor.org](https://truscor.org)**

---

<div align="center">

© 2026 TRUSCOR Private Limited. All rights reserved.<br/>
<em>Where intelligence meets accountability.</em>

</div>
