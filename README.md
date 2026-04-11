# ATTESTORIUM

Primitive ID: PRIM-006  
Package: @verifrax/attestorium  
Binary: attestorium

Verifrax primitive — attestation primitive for deterministic irreversible systems.

---

## Proof artifacts

This repository is part of the VERIFRAX proof perimeter.

- **ARTIFACT-0006**
- **ARTIFACT-0005**
- **ARTIFACT-0004**
- **ARTIFACT-0003**
- **ARTIFACT-0002**
- **ARTIFACT-0001**

**Canonical public proof surface:** https://proof.verifrax.net  
**Canonical proof publication repository:** https://github.com/Verifrax/proof  
**Canonical evidence root:** https://github.com/Verifrax/VERIFRAX

## Terminal planes

- **[ANAGNORIUM](https://github.com/Verifrax/ANAGNORIUM)** — terminal recognition
- **[REGRESSORIUM](https://github.com/Verifrax/REGRESSORIUM)** — terminal recourse

## Status

Current release status: pre-stable primitive release line.

Canonical release target:

package version: 0.1.0  
tag: v0.1.0

ATTESTORIUM is part of the Verifrax primitive layer and follows the canonical primitive governance, naming, version, and packaging rules.

---

## Purpose

ATTESTORIUM witnesses and attests to a verification result after origin, custody, time, boundary, and verification have already been fixed.

Once an artifact has a stable origin, preserved custody, explicit time boundary, enforced operating boundary, and deterministic verification result, the system still needs a formal witnessing layer that can state that this result was observed and attested under defined conditions. ATTESTORIUM exists to produce that attestation layer.

It does not establish origin. It does not preserve custody. It does not fix temporal order. It does not enforce boundaries. It does not verify correctness by itself. It does not judge or terminate. Its role is narrower: witness and attest to an already-determined verification state.

---

## What This Primitive Does

- attests to a deterministic verification outcome
- creates a witness-bearing record suitable for downstream judgment
- emits attestation output that preserves observed verification state

---

## What This Primitive Does Not Do

- does not establish first origin
- does not preserve custody continuity
- does not fix temporal ordering
- does not enforce operational boundaries
- does not perform primary verification itself
- does not judge validity
- does not terminate lifecycle

---

## Behavioral Contract

Invocation model:

executable: attestorium  
package: @verifrax/attestorium  
runtime: CLI-first

The primitive operates on an artifact whose origin, custody, time, boundary, and verification surfaces are already fixed.

If no stable verification result exists, ATTESTORIUM must not fabricate an attestation.

Exit codes:

0 — attestation completed successfully  
non-zero — invocation failed or contract violated

---

## Usage

Install:

npm install -g @verifrax/attestorium

Execute:

attestorium artifact.json

stdin example:

cat artifact.json | attestorium

---

## Determinism Guarantees

For identical canonical input, ATTESTORIUM must produce identical attestation output.

No hidden environmental state may influence the result.

ATTESTORIUM assumes an already-bounded and already-verified prior state and does not substitute for origin, custody, time, boundary, verification, judgment, or termination primitives.

---

## Security Model

ATTESTORIUM protects against ambiguity in whether a verification result was actually witnessed and attested.

Its security value is to preserve a deterministic witness layer over a completed verification result. It does not itself decide final judgment and does not terminate lifecycle state.

---

## Relationship to Other Primitives

Canonical primitive order:

1 originseal  
2 archicustos  
3 kairoclasp  
4 limenward  
5 validexor  
6 attestorium  
7 irrevocull  
8 guillotine

Repositories:

https://github.com/Verifrax/originseal  
https://github.com/Verifrax/archicustos  
https://github.com/Verifrax/kairoclasp  
https://github.com/Verifrax/limenward  
https://github.com/Verifrax/validexor  
https://github.com/Verifrax/attestorium  
https://github.com/Verifrax/irrevocull  
https://github.com/Verifrax/guillotine

---

## Installation

npm install -g @verifrax/attestorium

command -v attestorium

Repository:
- GitHub: https://github.com/Verifrax/attestorium
- Package: @verifrax/attestorium
- Binary: attestorium

---

## License

MIT

## Adjacent sovereign surfaces

This repository is part of the Verifrax sovereign stack and remains bounded relative to:

- **[ANAGNORIUM](https://github.com/Verifrax/ANAGNORIUM)** for terminal recognition
- **[REGRESSORIUM](https://github.com/Verifrax/REGRESSORIUM)** for terminal recourse
