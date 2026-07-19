# Ũnojñ Kore Kãnquy Keyboard Layout

An specialized keyboard layout design constructed specifically for typing the **Koreguaje Gutu** language using the Keyman Developer framework. This layout bundles the standard QWERTY structural layout alongside a smart dead-key engine mapped to provide intuitive accent control.

The package is pre-configured to utilize and bundle the **Andika** literacy font created by SIL International to ensure proper glyph visualization for unique vowels and structures.

## Keyboard Features

* **Base Configuration**: Standard QWERTY layout engine.
* **Typing Engine**: Dual-state structural dead keys triggered by the Semicolon key `;`.
* **Dynamic Chaining**: Multi-tap character sequences built natively for custom character chains (`cu`, `jñ`, etc.).
* **Typography**: Bundles native support rules for the Andika font family.

---

## Typography & Mapping Guide

To write any custom character matrix below, press and release the **Semicolon key (`;`)** first, and then type the target letter key directly after it.

### Lowercase Character Engine

| Input Sequence | Resulting Output Glyph | Description |
| :--- | :--- | :--- |
| `;` then `a` | **ã** | Small a with tilde |
| `;` then `e` | **ẽ** | Small e with tilde |
| `;` then `i` | **ĩ** | Small i with tilde |
| `;` then `o` | **õ** | Small o with tilde |
| `;` then `n` | **ñ** | Small n with tilde |
| `;` then `u` | **ù** | Small u with grave accent |
| `;` then `u` `u` | **ũ** | Small u with tilde |
| `;` then `u` `u` `u` | **ʉ** | Small u with bar (Stroke u) |
| `;` then `u` `u` `u` `u` | **ʉ̃** | Small u bar with combining tilde |
| `;` then `c` | **ch** | Consonant digraph ch |
| `;` then `c` `c` | **cu** | Structural pair cu |
| `;` then `j` | **jm** | Structural pair jm |
| `;` then `j` `j` | **jñ** | Structural pair jñ |
| `;` then `p` | **ph** | Consonant digraph ph |
| `;` then `q` | **qu** | Structural pair qu |
| `;` then `h` | **ʼ** | Modifier letter apostrophe (Glottal Stop) |

### Uppercase Character Engine (Shift Mode)

To input uppercase characters, press and release **Shift + Semicolon key (`:`)**, then type the target sequence while holding down the **Shift** modifier.

| Input Sequence | Resulting Output Glyph | Description |
| :--- | :--- | :--- |
| `:` then `Shift + A` | **Ã** | Capital A with tilde |
| `:` then `Shift + E` | **Ẽ** | Capital E with tilde |
| `:` then `Shift + I` | **Ĩ** | Capital I with tilde |
| `:` then `Shift + O` | **Õ** | Capital O with tilde |
| `:` then `Shift + N` | **Ñ** | Capital N with tilde |
| `:` then `Shift + U` | **Ù** | Capital U with grave accent |
| `:` then `Shift + U` `Shift + U` | **Ũ** | Capital U with tilde |
| `:` then `Shift + U` `Shift + U` `Shift + U` | **Ʉ** | Capital U with bar (Stroke U) |
| `:` then `Shift + U` `Shift + U` `Shift + U` `Shift + U` | **Ʉ̃** | Capital U bar with combining tilde |
| `:` then `Shift + C` | **Ch** | Titlecase digraph Ch |
| `:` then `Shift + C` `Shift + C` | **Cu** | Titlecase pair Cu |
| `:` then `Shift + C` | **Jm** | Titlecase pair Jm |
| `:` then `Shift + J` `Shift + J` | **Jñ** | Titlecase pair Jñ |
| `:` then `Shift + P` | **Ph** | Titlecase digraph Ph |
| `:` then `Shift + Q` | **Qu** | Titlecase pair Qu |
| `:` then `Shift + H` | **ʼ** | Modifier letter apostrophe (Glottal Stop) |

---

## File Structure Guide

For successful compilation, maintain these exact file placements within your project workspace root:

* `unojn_kore_kanquy.kpj`: Keyman Developer project execution profile tracking file.
* `unojn_kore_kanquy.kmn`: Keyboard layout rule definitions script file.
* `unojn_kore_kanquy.kps`: Distribution setup installer configuration rule file.
* `Andika-Regular.ttf`: Target Unicode print font file asset.

## Developer Compilation

1. Download and run Keyman Developer desktop dashboard suite.
2. Choose **Open Project** and navigate to select `unojn_kore_kanquy.kpj`.
3. Open the file `unojn_kore_kanquy.kmn` from your workspace menu.
4. Press **F7** on your machine or select **Compile Keyboard** via user toolbar to package your target layouts.
