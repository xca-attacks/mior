# MIOR Proof of Concept

[![CVE-2026-0462](https://img.shields.io/badge/CVE-2026--0462-red)](https://www.cve.org/CVERecord?id=CVE-2026-0462)
[![CCS 2026](https://img.shields.io/badge/Conference-CCS%202026-blue)](https://www.sigsac.org/ccs/CCS2026/)

[MIOR](https://xca-attacks.github.io/mior) is a data fabric rerouting attack. It
requires a system configured with a patched BIOS that leaves the data fabric
unlocked.

The [host kernel patch](host-kernel.patch) provides the proof of concept for
leaving the Reverse Map Table (RMP) uninitialized. The kernel modules that
exploit this state are available in the 
[Fabricked-Attack PoC repository](https://github.com/Fabricked-Attack/PoC).

Definitions used in the POC are derived from open source releases such as
[AMD-ASPFW](https://github.com/amd/AMD-ASPFW),
[opensil](https://github.com/openSIL/openSIL) (both the "Genoa" and "Turin"
branches), [coreboot](https://github.com/coreboot/coreboot), and of course
linux.
