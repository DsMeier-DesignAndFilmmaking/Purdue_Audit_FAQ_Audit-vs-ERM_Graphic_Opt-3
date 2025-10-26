# Font Implementation Guide

## Font Families Required

This project uses two distinct font families:

### 1. United Sans Condensed (Headlines Only)
- **Usage**: Container headlines ("INTERNAL AUDIT" and "RISK MANAGEMENT")
- **Weights**: Regular (400), Bold (700)

### 2. Acumin Pro (All Other Text)
- **Usage**: Body text, section headers, content text, VS element
- **Weights**: Light (300), Regular (400), Bold (700)

## Font Files Required

### United Sans Condensed Files:
- `UnitedSansCondensed-Regular.woff2`
- `UnitedSansCondensed-Regular.woff`
- `UnitedSansCondensed-Regular.ttf`
- `UnitedSansCondensed-Bold.woff2`
- `UnitedSansCondensed-Bold.woff`
- `UnitedSansCondensed-Bold.ttf`

### Acumin Pro Files:
- `AcuminPro-Light.woff2`
- `AcuminPro-Light.woff`
- `AcuminPro-Light.ttf`
- `AcuminPro-Regular.woff2`
- `AcuminPro-Regular.woff`
- `AcuminPro-Regular.ttf`
- `AcuminPro-Bold.woff2`
- `AcuminPro-Bold.woff`
- `AcuminPro-Bold.ttf`

## Font Sources

### Acumin Pro:
- **Adobe Fonts**: Available with Adobe Creative Cloud subscription
- **Fontspring**: Commercial licensing available
- **Adobe Typekit**: Web font service option

### United Sans Condensed:
- **Commercial Font Foundries**: Purchase from authorized distributors
- **Font Licensing**: Ensure proper web use licensing

## Directory Structure:
```
comparison-chart/
├── fonts/
│   ├── UnitedSansCondensed-Regular.woff2
│   ├── UnitedSansCondensed-Regular.woff
│   ├── UnitedSansCondensed-Regular.ttf
│   ├── UnitedSansCondensed-Bold.woff2
│   ├── UnitedSansCondensed-Bold.woff
│   ├── UnitedSansCondensed-Bold.ttf
│   ├── AcuminPro-Light.woff2
│   ├── AcuminPro-Light.woff
│   ├── AcuminPro-Light.ttf
│   ├── AcuminPro-Regular.woff2
│   ├── AcuminPro-Regular.woff
│   ├── AcuminPro-Regular.ttf
│   ├── AcuminPro-Bold.woff2
│   ├── AcuminPro-Bold.woff
│   └── AcuminPro-Bold.ttf
├── index.html
├── style.css
└── FONT_IMPLEMENTATION.md
```

## Implementation Complete

The CSS has been updated with:
- ✅ Separate `@font-face` declarations for both font families
- ✅ CSS variables for consistent font usage
- ✅ United Sans Condensed applied to container headlines only
- ✅ Acumin Pro applied to all other text elements
- ✅ Proper fallback fonts for both families
- ✅ Font display optimization with `font-display: swap`

## Font Usage Summary:
- **Headlines**: United Sans Condensed (INTERNAL AUDIT, RISK MANAGEMENT)
- **All Other Text**: Acumin Pro (section headers, body text, VS element, etc.)

Once the font files are added to the `fonts/` directory, both font families will be applied correctly across the project.
