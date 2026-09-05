# NOTICE — Third-Party Software

**D1 Save Forge** (this repository and the web tool it builds) embeds parts of
the following third-party software, compiled to WebAssembly. The web tool is
and will remain **free of charge and non-commercial**, as required by the
Sustainable Use License below.

## Modified software notice

The [DevilutionX](https://github.com/diasurgical/devilutionX) engine in
`vendor/DevilutionX` has been **MODIFIED** for this project: a headless
save-editor ABI (`editor/packages/engine/src/`), headless link shims/stubs,
and a curated preload set. See `editor/packages/engine/build_core.sh`.

## Diablo trademark

"Diablo" is a trademark of Blizzard Entertainment. This project is an
unofficial fan tool for save files of the open-source DevilutionX
re-implementation; it is not affiliated with or endorsed by Blizzard
Entertainment. Game assets (MPQ archives, art, music) are NOT distributed
here; the embedded data tables are the reconstructions shipped by the
DevilutionX project itself.

## Never-embed rule (ratified 2026-09-01)

The WebAssembly data payload embeds ONLY the DevilutionX txtdata stat/class
tables listed in `editor/packages/engine/build_core.sh` and the one SIL-OFL
font credited below. NEVER embedded, under any circumstance: narrative text
tables (`assets/txtdata/text/`), sound, sprite art, MPQ archives, Blizzard
logos or any other game asset. Anything added to the preload set must
respect this rule (research and rationale:
`docs/research/2026-09-01-txtdata-licensing/`).

---

## DevilutionX — Sustainable Use License

Applies to the engine source in `vendor/DevilutionX` and to the compiled
`d1_core.wasm` / `d1_core.js` / `d1_core.data` artifacts derived from it.

> Key terms: use, modification and distribution are permitted **only** for
> non-commercial purposes and free of charge; licensing notices must be
> preserved; modified copies must carry a prominent modification notice
> (given above).

# Sustainable Use License

Version 1.0

## Acceptance

By using the software, you agree to all of the terms and conditions below.

## Copyright License

The licensor grants you a non-exclusive, royalty-free, worldwide,
non-sublicensable, non-transferable license to use, copy, distribute, make
available, and prepare derivative works of the software, in each case subject
to the limitations below.

## Limitations

You may use or modify the software only for your own internal business
purposes or for non-commercial or personal use.
You may distribute the software or provide it to others only if you do so free
of charge for non-commercial purposes.
You may not alter, remove, or obscure any licensing, copyright, or other
notices of the licensor in the software. Any use of the licensor's trademarks
is subject to applicable law.

## Patents

The licensor grants you a license, under any patent claims the licensor can
license, or becomes able to license, to make, have made, use, sell, offer for
sale, import and have imported the software, in each case subject to the
limitations and conditions in this license. This license does not cover any
patent claims that you cause to be infringed by modifications or additions to
the software. If you or your company make any written claim that the software
infringes or contributes to infringement of any patent, your patent license
for the software granted under these terms ends immediately. If your company
makes such a claim, your patent license ends immediately for work on behalf of
the company.

## Notices

You must ensure that anyone who gets a copy of any part of the software from
you also gets a copy of these terms.
If you modify the software, you must include in any modified copies of the
software a prominent notice stating that you have modified the software.

## No Other Rights

These terms do not imply any licenses other than those expressly granted in
these terms.

## Termination

If you use the software in violation of these terms, such use is not licensed,
and your license will automatically terminate. If the licensor provides you
with a notice of your violation, and you cease all violation of this license
no later than 30 days after you receive the notice, your license will be
reinstated retroactively. However, if you violate these terms after such
reinstatement, any additional violation of these terms will cause your license
to terminate automatically and permanently.

## No Liability

As far as the law allows, the software comes as is, without any warranty or
condition, and the licensor will not be liable to you for any damages arising
out of these terms whether or not the licensor has been advised of the
possibility of such damages.

## Definitions

The "licensor" is the entity offering these terms.

The "software" is the software the licensor makes available under these terms,
including any portion of it.

"You" refers to the individual or entity agreeing to these terms.

"Your company" is any legal entity, sole proprietorship, or other kind of
organization that you work for, plus all organizations that have control over,
are under the control of, or are under common control with that organization.
Control means ownership of substantially all the assets of an entity, or the
power to direct its management and policies by vote, contract, or otherwise.
Control can be direct or indirect.

"Your license" is the right to use the software under these terms.

"Use" means anything you do with the software requiring your license.

"Trademark" means trademarks, service marks, and similar rights.

---

## mpqfs — MIT License

MPQ filesystem library linked into the core
(`vendor/DevilutionX/build-em/_deps/mpqfs-src`).

> MIT License — Copyright (c) 2025 mpqfs contributors. Permission is hereby
> granted, free of charge, to any person obtaining a copy of this software and
> associated documentation files (the "Software"), to deal in the Software
> without restriction, including without limitation the rights to use, copy,
> modify, merge, publish, distribute, sublicense, and/or sell copies of the
> Software, and to permit persons to whom the Software is furnished to do so,
> subject to the following conditions: The above copyright notice and this
> permission notice shall be included in all copies or substantial portions of
> the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY
> KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
> MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
> EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
> OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
> ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
> DEALINGS IN THE SOFTWARE.

## Lua — MIT License

Lua 5.4 interpreter linked into the core.

> Copyright © 1994–2025 Lua.org, PUC-Rio. Permission is hereby granted, free
> of charge, to any person obtaining a copy of this software and associated
> documentation files (the "Software"), to deal in the Software without
> restriction, including without limitation the rights to use, copy, modify,
> merge, publish, distribute, sublicense, and/or sell copies of the Software,
> and to permit persons to whom the Software is furnished to do so, subject to
> the same conditions and disclaimer as the MIT text above.

## SheenBidi — Apache License 2.0

Unicode bidi algorithm linked into the core. Licensed under the Apache
License, Version 2.0 (the "License"); you may not use this file except in
compliance with the License. You may obtain a copy of the License at
<http://www.apache.org/licenses/LICENSE-2.0>. Unless required by applicable
law or agreed to in writing, software distributed under the License is
distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
KIND, either express or implied. See the License for the specific language
governing permissions and limitations under the License.

## zlib / bzip2 — via Emscripten ports

Compression libraries linked through Emscripten's system ports, used by the
MPQ reader. zlib is licensed under the zlib license; bzip2 under its own
permissive BSD-style license. Both are unmodified.

## Fonts — SIL Open Font License 1.1

The embedded font `assets/fonts/12-00.clx` is generated from the
[devilutionx-assets](https://github.com/diasurgical/devilutionx-assets)
repository (bundled PCX sources, converted with their pcx2clx tooling).
Those fonts are **Noto** and **Unifont**, licensed under the
[SIL Open Font License, Version 1.1](https://openfontlicense.org/open-font-license-official-text/);
gamepad symbols are from greatdocbrown's gamepad UI pack. The full license
text is available at the link above and as `LICENSE-SIL.txt` in the
devilutionx-assets repository. This font is NOT a Blizzard asset.
