# Unified Naming Convention
aka UNC, is an organization between executor developers to provide a unified scripting API for our scripters.

## Status

UNC is an **active, community-driven standard**. Established in 2022 and maintained through the Byfron/Hyperion era, it is still the compatibility benchmark used by the modern executor landscape — Solara, Wave, Xeno, Swift, Delta, Codex, Volt, MacSploit and more all report a *UNC score* measured against this specification.

This repository is the **2026 revision**. It has been brought in line with the current executor ecosystem and current Luau, and the retired notice published in 2024 has been removed. The standard is a living document — proposals and corrections are accepted through pull requests and reviewed by the maintainers.

## Why?
Over the years scripting has gotten more and more complex to support multiple executors. This is because of the many unique naming conventions various executors use.

Consider the following scenario. You want to know if a function belongs to the executor or not. In order for this code to be cross compatible with all executors code like this is needed:
```lua
local is_executor_closure = is_solara_closure or is_wave_closure or is_xeno_closure or is_swift_closure or is_delta_closure or is_codex_closure or is_volt_closure or is_macsploit_closure
```
This is reality for scripters who want cross compatibility in their scripts. Scripters shouldn't have to do such laborious work just to attain cross compatibility. The UNC seeks to solve this problem using naming conventions everyone agrees upon and follows.

One variant of a script should naturally work on all script executors which have their environment properly fitted to the UNC.

## How?
The UNC provides standards for naming conventions as well as API functionality. The standard is written in markdown on this GitHub. Edits or additions are done through pull requests. Edits and additions are manually approved by the UNC council and discussed by everyone.

## Supporting UNC
As a product owner, your support of UNC by following the API will result in a far smoother experience for scripters, as they are able to work on scripts that they can confidently say will work on **most** products.

You do not need to implement every function to support UNC. If you support the subset you do have, you support UNC. The portion of the standard your executor implements is commonly reported as its *UNC score*, which the community uses as a compatibility benchmark.

## Checking your environment

You can run the UNC environment checking script to see how well your executor environment supports the UNC standard. Find the script [here.](UNCCheckEnv.lua) The script runs a test for every function in the standard and prints a pass/fail summary to the console.

## Revision history

- **2026** — Re-activation revision. Retired notice removed, documentation updated for the modern executor ecosystem and current Luau.
- **2024** — Original publication.

## Contributing
Go [here](CONTRIBUTING.md) for a guide on contributing.
