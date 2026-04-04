# Savantis hardened the BTC `INVEST` release lane to stay on one code path

Verified config and fallback changes now keep checked-in defaults and styleless helper paths on `INVEST`, while repo-backed runtime smoke remains blocked on missing canonical artifacts and macro data.

Savantis narrowed the first BTC `INVEST` release lane to one explicit code path.

## What Was Verified

- Checked-in runtime defaults now keep `selected_style: INVEST` with `active_styles: [INVEST]` instead of widening into `SWING` or `SCALP`.
- Brain-registry and styleless fallback behavior now stays on the `INVEST` lane instead of silently defaulting back to `SWING`.
- Focused compile and assertion checks were recorded for the release-default contract, and code-side regression coverage was added for that contract.
- The remaining gap for this release lane is runtime-artifact validation, not another known multi-style code leak.

## Evidence Basis

- Checked-in runtime defaults were tightened to keep the first release lane on `INVEST`.
- Fallback behavior and styleless helper paths were tightened so they no longer drift back to `SWING`.
- Focused verification and regression coverage were recorded for the release-default contract.

## Scope And Conditions

This note applies only to code-side hardening of the BTC `INVEST` release lane. It does not prove repo-backed runtime boot, artifact hydration, end-to-end trade execution, or any result outside the BTC `INVEST` lane.

## What Remains Uncertain

Repo-backed runtime smoke is still blocked because the validation workspace does not contain the documented canonical BTC Moirai artifacts and the broader smoke path also stops on missing macro data. That means Savantis has reduced hidden lane drift in code, but has not yet proved runtime readiness on the repo-backed validation path.

## Why This Matters

This is a real engineering-trust improvement because the first release lane now fails closer to the true remaining blocker instead of hiding style drift behind broader defaults. In plain language: Savantis is making the system more honest about what is verified now and what still needs proof before broader claims are safe.
