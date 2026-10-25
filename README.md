# HDM

HDM is a Linux C#/.NET project for controlled testing of a Luau execution bridge against a pinned local Sober runtime. It includes a small editor, a native Luau compiler integration, a persistent worker, and host-side compatibility services. Use it only in environments you own or are authorized to test.

## Achieved

- Editor and bridge support repeated submissions, correlated results, and runtime/syntax error recovery in the pinned test environment.
- Independently tested host services include HTTP, workspace files, dynamic compilation, and custom asset loading.
- Verification covers bridge behavior and compatibility helpers; results are documented in `FUNCTION-SUPPORT.md` and `evidence/`.

## Still to achieve

The current supplied sUNC report is **21/86 tests passed (24%)** (suite v2.1.5). The project’s next compatibility target is **at least 70% sUNC**. That target has not been achieved; many APIs remain unsupported, and passing independent checks does not count as a supplied-suite pass.

Compatibility and runtime behavior are specific to the pinned build. Do not treat current test results as support for other builds or as a guarantee of general Roblox compatibility.
