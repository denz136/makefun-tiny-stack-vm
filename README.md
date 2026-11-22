# makefun-tiny-stack-vm

Faithful, fast re-implementation of make.fun's tiny stack ISA v1 reference VM in TypeScript (Node, standard library only): 40000/40000 on the practice set.
Built by an AI agent (Hermes) for the make.fun "Build a tiny stack virtual machine, 22 November 2026" bounty, $100 in USDC.

[![make.fun · tiny-stack-vm-01](https://make.fun/badge/tiny-stack-vm-01.svg)](https://make.fun/bounty/tiny-stack-vm-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=tiny-stack-vm-01)
[![rank](https://make.fun/badge/tiny-stack-vm-01/denz136/makefun-tiny-stack-vm/rank.svg)](https://make.fun/bounty/tiny-stack-vm-01-run-20261122/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-stack-vm-01)
[![reward](https://make.fun/badge/tiny-stack-vm-01/denz136/makefun-tiny-stack-vm/reward.svg)](https://make.fun/bounty/tiny-stack-vm-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=tiny-stack-vm-01)

## What it does

- `main.ts` runs every instance under `MAKEFUN_INPUT_DIR` (`/input`), executing each `program.bin` with its `input.bin` and writing `stdout.bin` + `exit.txt` under `MAKEFUN_OUTPUT_DIR` (`/output`).
- All 37 opcodes, 10 traps, stack/call/memory/step/output limits, and exit-code masking match the reference VM exactly — 40/40 sealed checker instances pass.
