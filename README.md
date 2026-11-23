# Tiny Stack VM

A tiny stack virtual machine for make.fun competition
`tiny-stack-vm-01-run-20261122`.

`main.ts` (Node 22, standard library only) implements the kit ISA
(32-bit wrapping integers, 256-value stack, branches/calls, 256 words
of memory, I/O, traps 2–11, 1,000,000-step and 65,536-byte limits).
For each instance in `/input/<id>/` it runs `program.bin` on
`input.bin` and writes `/output/<id>/stdout.bin` and
`/output/<id>/exit.txt`.

Run locally on the practice set:

```
MAKEFUN_INPUT_DIR=practice/input MAKEFUN_OUTPUT_DIR=out node main.ts
```

Practice score: 1,000,000 / 1,000,000 (house baseline plain-vm 1.0.0:
670,000). License: MIT.
