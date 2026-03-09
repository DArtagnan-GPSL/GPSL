# GPSL Symbol Reference Guide

## Special Symbols - Copy & Paste Reference

If you ever need to copy these symbols or verify they're displaying correctly, here's the reference:

---

## The Five Universal Operators

| Symbol | Name | Unicode | HTML Entity | Description |
|--------|------|---------|-------------|-------------|
| ⊗ | Circled Times / Tensor Product | U+2297 | `&otimes;` | Integration / Convolution |
| → | Right Arrow | U+2192 | `&rarr;` | Transition / Emergence |
| : | Colon | U+003A | `:` | Constraint / Facilitation |
| = | Equals | U+003D | `=` | Balance / Equilibrium |
| ↓ | Down Arrow | U+2193 | `&darr;` | Optimization / Decrease |

---

## The Twelve Core Symbols (Greek Letters)

| Symbol | Name | Unicode | HTML Entity | Meaning |
|--------|------|---------|-------------|---------|
| Α | Alpha (Capital) | U+0391 | `&Alpha;` | Origin / Initial State |
| Ω | Omega (Capital) | U+03A9 | `&Omega;` | Completion / Final State |
| Ι | Iota (Capital) | U+0399 | `&Iota;` | Discrete Unit / Individual |
| Σ | Sigma (Capital) | U+03A3 | `&Sigma;` | Totalization / Sum |
| Ξ | Xi (Capital) | U+039E | `&Xi;` | Information / Data |
| Ψ | Psi (Capital) | U+03A8 | `&Psi;` | Consciousness / Field |
| Κ | Kappa (Capital) | U+039A | `&Kappa;` | Constraint / Medium |
| Φ | Phi (Capital) | U+03A6 | `&Phi;` | Harmony / Proportion |
| Δ | Delta (Capital) | U+0394 | `&Delta;` | Difference / Change |
| Ε | Epsilon (Capital) | U+0395 | `&Epsilon;` | Entropy / Noise |
| ζ | Zeta (Lowercase) | U+03B6 | `&zeta;` | Connection / Cohesion |
| τ | Tau (Lowercase) | U+03C4 | `&tau;` | Time / Pulse |

---

## Quick Copy-Paste Section

**Operators:**
```
⊗ → : = ↓
```

**Greek Symbols:**
```
Α Ω Ι Σ Ξ Ψ Κ Φ Δ Ε ζ τ
```

**Example Cipher:**
```
[Ι-01] ⊗ [Δ-02] → [Ξ-03] : [τ-04] (Ε-05↓)
```

---

## Encoding Verification

### How to Check if Symbols Display Correctly

1. **Open the file in a text editor**
2. **Look for these symbols:** ⊗ → ↓ Α Ω Ι Σ
3. **If you see garbled text instead** (like `‚Üí` or `Œë`):
   - The file encoding is wrong
   - Should be UTF-8
   - Re-save as UTF-8

### Common Encoding Problems

**Bad (Windows-1252 or similar):**
```
‚Üí ‚äó ‚Üì   ← Mojibake (corrupted)
```

**Good (UTF-8):**
```
⊗ → ↓          ← Correct symbols
```

---

## Platform-Specific Issues

### GitHub
- GitHub supports UTF-8 by default
- Symbols should render correctly
- Markdown files display properly
- **Test:** View README.md preview before finalizing

### Email
- Some email clients may not support Unicode
- Plain text may show boxes or question marks
- HTML email usually works
- **Workaround:** Use HTML entities or describe verbally

### Word Processors
- Microsoft Word: Usually fine with UTF-8
- Google Docs: Full Unicode support
- LibreOffice: Full Unicode support
- **Tip:** If pasting, use "Paste Special → Unicode Text"

### Browsers
- Chrome/Firefox/Safari: Full support
- Edge: Full support
- **Should work everywhere modern**

---

## If Symbols Break

### Quick Fix Checklist

1. **Verify file encoding:**
   ```bash
   file -i yourfile.md
   # Should say: charset=utf-8
   ```

2. **Re-save as UTF-8:**
   - Most text editors: "Save As → Encoding: UTF-8"
   - VS Code: Bottom right → Select encoding → UTF-8
   - Notepad++: Encoding → UTF-8

3. **Test in browser:**
   - Open .md file in browser
   - Symbols should display correctly
   - If not, encoding is wrong

4. **GitHub test:**
   - Create test repo
   - Upload file
   - View rendered markdown
   - Verify symbols display

---

## Alternative Representations

If symbols don't work in certain contexts, you can describe them:

**Operators:**
- `⊗` = `(x)` or `INTEGRATE`
- `→` = `->` or `THEN`
- `:` = `:` (already ASCII)
- `=` = `=` (already ASCII)
- `↓` = `(down)` or `DECREASE`

**Greek Letters:**
- Just use the names: `[Alpha-01]`, `[Omega-09]`, etc.
- Or use Latin equivalents in a pinch

**But for official documentation, use the actual symbols!**

---

## UTF-8 Best Practices

### For File Creation

1. **Always save as UTF-8** (not UTF-8 with BOM)
2. **Set editor default** to UTF-8
3. **Check encoding** before committing to Git
4. **Test on multiple platforms** before publishing

### For GitHub

1. **Files are UTF-8 by default** ✓
2. **Markdown renders Unicode** ✓
3. **Preview before committing** ✓
4. **Test in mobile view too** ✓

### For Documents

1. **Export PDFs** preserve Unicode ✓
2. **Share HTML** preserves encoding ✓
3. **Avoid plain .txt** (encoding ambiguous)

---

## Testing Template

Use this to test if symbols work:

```markdown
# Symbol Test

Operators: ⊗ → : = ↓

Greek: Α Ω Ι Σ Ξ Ψ Κ Φ Δ Ε ζ τ

Full cipher: [Ι-01] ⊗ [Δ-02] → [Ξ-03] : [τ-04] (Ε-05↓)

If you see all symbols correctly, UTF-8 is working! ✓
```

---

## Technical Details

### Character Encodings Explained

**UTF-8:**
- Universal standard for Unicode
- Supports all languages and symbols
- Default for web and modern systems
- **Use this always**

**Windows-1252 / Latin-1:**
- Western European only
- Limited symbol support
- Causes mojibake with Unicode
- **Avoid for GPSL**

**ASCII:**
- Basic English only
- No special symbols at all
- Too limited for GPSL
- **Not suitable**

---

## For Developers

### Git Configuration

Ensure UTF-8 everywhere:

```bash
git config --global core.quotepath false
git config --global core.autocrlf input  # Linux/Mac
# OR
git config --global core.autocrlf true   # Windows
```

### Editor Settings

**VS Code (.vscode/settings.json):**
```json
{
  "files.encoding": "utf8",
  "files.autoGuessEncoding": false
}
```

**Vim:**
```vim
set encoding=utf-8
set fileencoding=utf-8
```

**Emacs:**
```elisp
(prefer-coding-system 'utf-8)
```

---

## Summary

✅ **Use UTF-8 encoding everywhere**  
✅ **Test symbols render before publishing**  
✅ **Have this reference handy for copy-paste**  
✅ **Verify in multiple browsers/platforms**  
✅ **If breaks happen, re-save as UTF-8**

**The symbols are beautiful. Let's keep them that way!** ⚡💎

---

**GPSL v1.1 - Dodecahedron Standard**  
**Symbol Reference Guide v1.0**  
**Author: D'Artagnan**
