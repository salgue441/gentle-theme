<h1 align="center">
  <br>
  Gentle Theme
  <br>
</h1>

<h4 align="center">An accessible, eye-friendly theme family for Visual Studio Code</h4>

<p align="center">
  <a href="#-features">Features</a> •
  <a href="#-variants">Variants</a> •
  <a href="#-installation">Installation</a> •
  <a href="#-color-palette">Palette</a> •
  <a href="#-accessibility">Accessibility</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/VS%20Code-1.60+-blue?style=flat-square&logo=visual-studio-code" alt="VS Code Version">
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square" alt="License">
  <img src="https://img.shields.io/badge/Accessibility-WCAG%20AA-purple?style=flat-square" alt="WCAG AA Compliant">
</p>

---

## Why Gentle Theme?

Designed from the ground up for **developers who spend long hours coding**, especially those with:

- **Light sensitivity** or eye strain
- **Neurodivergent needs** (ADHD, autism, sensory processing differences)
- **Preference for calm, non-distracting interfaces**

Every color choice is intentional—no pure whites that glare, no pure blacks that fatigue, no oversaturated colors that overstimulate.

---

## Features

| Feature | Description |
|---------|-------------|
| **No Pure White/Black** | Backgrounds use warm off-whites and soft dark grays to reduce contrast strain |
| **Warm Color Temperature** | Reduced blue light throughout all variants |
| **Consistent Saturation** | Syntax colors use similar saturation levels to avoid visual "loudness" |
| **WCAG AA Compliant** | All text meets minimum 4.5:1 contrast ratio |
| **Semantic Consistency** | Same color meanings across all 6 variants |
| **Semantic Highlighting** | Full support for VS Code's semantic token API |

---

## Variants

### Light Themes

| Theme | Background | Best For |
|-------|------------|----------|
| **Gentle Light** | `#FDFCFA` warm white | Daytime coding, well-lit rooms |
| **Gentle Light Warm** | `#FAF8F5` cream/sepia | Light sensitivity, reduced blue light |

### Dark Themes

| Theme | Background | Best For |
|-------|------------|----------|
| **Gentle Dark** | `#1C1E22` soft charcoal | Evening coding, standard dark preference |
| **Gentle Dark Warm** | `#1F1D1A` warm charcoal | Cozy aesthetic, reduced blue light |

### Midnight Themes

| Theme | Background | Best For |
|-------|------------|----------|
| **Gentle Midnight** | `#0D0F12` near-black | OLED screens, very dark rooms |
| **Gentle Midnight Warm** | `#100E0C` warm near-black | OLED screens, warm aesthetic |

---

## Installation

### From VS Code Marketplace

1. Open **Extensions** sidebar (`Ctrl+Shift+X` / `Cmd+Shift+X`)
2. Search for `Gentle Theme`
3. Click **Install**
4. Press `Ctrl+K Ctrl+T` / `Cmd+K Cmd+T` to open theme selector
5. Choose your preferred variant

### Manual Installation

```bash
# Clone into VS Code extensions folder
cd ~/.vscode/extensions
git clone https://github.com/your-username/gentle-theme.git

# Restart VS Code
```

### From VSIX

```bash
# Build the package
npm install -g @vscode/vsce
vsce package

# Install
code --install-extension gentle-theme-1.0.0.vsix
```

---

## Color Palette

### Syntax Highlighting

Colors are consistent across all variants (adjusted for light/dark):

| Element | Light | Dark | Meaning |
|---------|-------|------|---------|
| **Keywords** | Purple | Lavender | Control flow, storage |
| **Strings** | Forest Green | Soft Green | Text literals |
| **Functions** | Steel Blue | Sky Blue | Callable code |
| **Types/Classes** | Teal | Cyan | Type definitions |
| **Numbers** | Amber | Gold | Numeric literals |
| **Comments** | Muted Gray | Dim Gray | Documentation |
| **Variables** | Dark/Light Gray | — | Identifiers |
| **Constants** | Warm Orange | — | Immutable values |

### UI Colors

| Element | Purpose |
|---------|---------|
| **Selection** | Soft blue highlight |
| **Find Match** | Warm amber highlight |
| **Errors** | Desaturated red |
| **Warnings** | Warm yellow |
| **Info** | Calm blue |
| **Success/Added** | Soft green |

---

## Accessibility

### Design Principles

1. **Reduced Visual Noise**
   - Subtle UI borders
   - Consistent background hierarchy
   - No harsh transitions between panels

2. **Predictable Color Semantics**
   - Same colors mean the same things
   - Errors are always warm red
   - Success is always green
   - Info is always blue

3. **Comfortable Contrast**
   - Text passes WCAG AA (4.5:1 minimum)
   - Not maximum contrast (which causes fatigue)
   - Optimized for extended reading

4. **Color Vision Accessibility**
   - Colors chosen to remain distinguishable for common color vision deficiencies
   - Meaning reinforced through context, not color alone

### Recommended Settings

Pair with these VS Code settings for optimal comfort:

```json
{
  "editor.fontFamily": "'JetBrains Mono', 'Fira Code', 'Cascadia Code', monospace",
  "editor.fontSize": 14,
  "editor.lineHeight": 1.6,
  "editor.letterSpacing": 0.3,
  "editor.cursorBlinking": "solid",
  "editor.cursorSmoothCaretAnimation": "on",
  "editor.smoothScrolling": true,
  "editor.bracketPairColorization.enabled": true,
  "editor.guides.bracketPairs": true,
  "workbench.list.smoothScrolling": true,
  "window.autoDetectColorScheme": true
}
```

### For Light Sensitivity

If you experience discomfort even with Gentle themes:

1. Use the **Warm** variants (more blue light reduction)
2. Reduce monitor brightness to 40-60%
3. Enable OS-level blue light filter (Night Shift / Night Light)
4. Consider a matte screen protector

---

## Customization

Override any color in your `settings.json`:

```json
{
  "workbench.colorCustomizations": {
    "[Gentle Dark]": {
      "editor.background": "#1A1C20"
    }
  },
  "editor.tokenColorCustomizations": {
    "[Gentle Dark]": {
      "comments": "#707888"
    }
  }
}
```

---

## Compatibility

Works with:

- Visual Studio Code 1.60+
- VSCodium
- Cursor
- Windsurf
- Other VS Code forks

---

## Contributing

Found an accessibility issue or have a suggestion? Please open an issue or PR.

When contributing, please keep in mind:

- All colors must pass WCAG AA contrast requirements
- Avoid pure black (`#000000`) and pure white (`#FFFFFF`)
- Test with color blindness simulators
- Consider neurodivergent users in design decisions

---

## License

MIT

---

<p align="center">
  Made with care for developers who need a gentler coding experience.
</p>
