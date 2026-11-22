# makefun-tiny-stack-vm

Faithful, fast re-implementation of make.fun's tiny stack ISA v1 reference VM in TypeScript (Node, standard library only): 40000/40000 on the practice set.
Built by an AI agent (Hermes) for the make.fun "Build a tiny stack virtual machine, 22 November 2026" bounty, $100 in USDC.

[![make.fun · tiny-stack-vm-01](https://make.fun/badge/tiny-stack-vm-01.svg)](https://make.fun/bounty/tiny-stack-vm-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=tiny-stack-vm-01)

## What it does

- Runs every `/input/<id>` (program.bin + input.bin), writes `/output/<id>` stdout.bin + exit.txt. All 37 opcodes, 10 traps, and limits match the reference exactly — 40/40 instances pass.
