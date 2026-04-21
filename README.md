<div align="center">

# 🎨 auto-theme

**World-class design systems, reverse-engineered and ready to use.**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Themes](https://img.shields.io/badge/themes-63%2B-brightgreen)](./theme-presets.json)
[![Brands](https://img.shields.io/badge/brands-63-blue)](#-theme-gallery)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](./CONTRIBUTING.md)

*Stop spending days on design systems. Start with the best ones in the world.*

[Browse Themes](#-theme-gallery) · [Quick Start](#-quick-start) · [JSON Presets](#-use-the-json-presets) · [Contribute](#-contributing)

</div>

---

## 🤔 What is this?

**auto-theme** is a curated collection of **63+ design systems** from the world's most respected tech companies and brands — reverse-engineered and documented in a format that's immediately usable by developers and designers.

Each theme includes:
- 🎨 **Complete color palettes** (backgrounds, surfaces, text, borders, accents, status colors)
- 🔤 **Typography rules** (font families, weights, sizes, letter-spacing)
- 📐 **Spacing & density systems**
- 🌙 **Both light and dark mode** variants
- ⚡ **Ready-to-paste JSON config** for direct use in your project

**Save days of design research.** Instead of reverse-engineering Linear's indigo-violet system or Stripe's gradient-heavy aesthetic yourself, grab it here in seconds.

---

## ✨ Why use auto-theme?

| Without auto-theme | With auto-theme |
|---|---|
| Hours studying competitor sites | Pick a theme in 30 seconds |
| Inconsistent color choices | Battle-tested palettes from world-class design teams |
| Rebuilding dark/light mode from scratch | Both modes included |
| Guessing typography pairings | Exact font families, weights, and spacing used by the pros |
| Blank canvas paralysis | 63+ opinionated starting points |

---

## 🖼️ Theme Gallery

### AI & Dev Tools
| Brand | Accent | Style |
|-------|--------|-------|
| **Linear** | `#7170ff` Indigo-Violet | Dark-first, precision engineering |
| **Cursor** | `#8b5cf6` Purple | Dark IDE, developer-focused |
| **Vercel** | `#000000` Monochrome | Minimal black & white |
| **Raycast** | `#FF6363` Red-Orange | Vibrant dark productivity |
| **Supabase** | `#3ECF8E` Emerald | Open source green |
| **Posthog** | `#F54E00` Bold Orange | High-energy analytics |
| **Resend** | `#000000` Black | Clean email developer tool |
| **Replicate** | `#5B21B6` Deep Violet | ML platform dark |
| **Ollama** | `#FFFFFF` White | Minimal local AI |

### Design & Creative
| Brand | Accent | Style |
|-------|--------|-------|
| **Figma** | `#A259FF` Purple | Design tool vibrant |
| **Framer** | `#0099FF` Blue | Motion & web design |
| **Webflow** | `#4353FF` Royal Blue | No-code dark |
| **Miro** | `#FFD02F` Yellow | Collaborative warm |
| **Lovable** | `#FF4785` Pink | AI design playful |

### Enterprise & SaaS
| Brand | Accent | Style |
|-------|--------|-------|
| **Stripe** | `#635BFF` Indigo | Payment precision |
| **Notion** | `#000000` Black | Minimalist productivity |
| **Airtable** | `#FCB400` Yellow | Colorful database |
| **Zapier** | `#FF4A00` Orange | Automation warm |
| **Intercom** | `#286EFA` Blue | Customer success |
| **Shopify** | `#96BF48` Green | Ecommerce growth |
| **Sentry` | `#362D59` Dark Purple | Error tracking |
| **MongoDB** | `#00ED64` Green | Data bold |
| **HashiCorp** | `#000000` Black | Infrastructure dark |
| **IBM** | `#0F62FE` Blue | Enterprise classic |

### AI & LLM Providers
| Brand | Accent | Style |
|-------|--------|-------|
| **Claude** | `#D97757` Warm Orange | Anthropic warm |
| **Mistral AI** | `#FF7000` Orange | European AI bold |
| **Cohere** | `#39594D` Forest Green | Enterprise NLP |
| **Together AI** | `#0066FF` Blue | Open AI platform |
| **ElevenLabs** | `#FFDE4D` Yellow | Voice AI warm |
| **Minimax** | `#FF4040` Red | Chinese AI bold |
| **Composio** | `#6C47FF` Purple | AI tools |

### Consumer & Lifestyle
| Brand | Accent | Style |
|-------|--------|-------|
| **Spotify** | `#1DB954` Green | Music streaming |
| **Pinterest** | `#E60023` Red | Visual discovery |
| **Airbnb** | `#FF5A5F` Coral | Warm belonging |
| **Uber** | `#000000` Black | Precision mobility |
| **Revolut** | `#0075EB` Blue | Fintech modern |
| **Coinbase** | `#0052FF` Blue | Crypto clean |
| **Wise** | `#00B9FF` Cyan | Fintech fresh |

### Hardware & Automotive
| Brand | Accent | Style |
|-------|--------|-------|
| **Apple** | `#0071E3` Blue | Premium minimal |
| **Tesla** | `#E82127` Red | EV futuristic |
| **BMW** | `#1C69D4` Blue | German precision |
| **Ferrari** | `#DC0000` Racing Red | Luxury speed |
| **Lamborghini** | `#FFC700` Gold | Supercar bold |
| **Bugatti** | `#00B4B4` Teal | Ultra luxury |
| **Renault** | `#FFCC00` Yellow | French automotive |
| **PlayStation** | `#003087` Dark Blue | Gaming iconic |

### Media & Publishing
| Brand | Accent | Style |
|-------|--------|-------|
| **The Verge** | `#FF3B30` Red | Tech journalism |
| **Wired** | `#000000` Black | Cyberpunk editorial |
| **Nike** | `#000000` Black | Athletic power |
| **Meta** | `#0866FF` Blue | Social tech |
| **Nvidia** | `#76B900` Green | GPU tech |
| **SpaceX** | `#FFFFFF` White | Space minimal |

---

## 🚀 Quick Start

### Option 1: Use the JSON Presets (Recommended)

Copy `theme-presets.json` into your project and load your preferred theme:

```js
import themes from './theme-presets.json'

// Get a specific theme
const linearTheme = themes.find(t => t.id === 'linear')

// Access dark mode colors
const { background, accent, textPrimary } = linearTheme.dark

// Access light mode colors
const lightColors = linearTheme.light
```

### Option 2: Read the Design System Docs

Each brand has a detailed markdown file in the root directory:

```
design-linear.md       → Linear's full design system
design-stripe.md       → Stripe's gradient & color system
design-notion.md       → Notion's minimal typography
design-cursor.md       → Cursor's dark IDE palette
...
```

### Option 3: Use the Lightweight Configs

The `configs/` directory contains compact, copy-paste-ready configurations:

```
configs/design-linear-config.md
configs/design-stripe-config.md
...
```

---

## 📦 Use the JSON Presets

The `theme-presets.json` file is the core of auto-theme. Each entry follows this structure:

```json
{
  "id": "linear",
  "name": "Linear",
  "description": "Precision engineering dark theme",
  "category": "dark",
  "preview": {
    "bg": "#08090a",
    "surface": "#0f1011",
    "accent": "#7170ff",
    "text": "#f7f8f8",
    "border": "#23252a"
  },
  "light": {
    "background": "#f7f8f8",
    "surface": "#f3f4f5",
    "accent": "#5e6ad2",
    "textPrimary": "#141516",
    "textSecondary": "#4a4d55",
    "textMuted": "#8a8f98",
    "border": "#e4e5e8",
    "font": {
      "family": "\"Inter Variable\", -apple-system, sans-serif"
    }
  },
  "dark": {
    "background": "#08090a",
    "surface": "#0f1011",
    "accent": "#7170ff",
    "textPrimary": "#f7f8f8",
    "textSecondary": "#d0d6e0",
    "textMuted": "#8a8f98",
    "border": "#23252a"
  }
}
```

### Integrate with Tailwind CSS

```js
// tailwind.config.js
import themes from './theme-presets.json'

const theme = themes.find(t => t.id === 'linear').dark

export default {
  theme: {
    extend: {
      colors: {
        bg: theme.background,
        surface: theme.surface,
        accent: theme.accent,
        'text-primary': theme.textPrimary,
        'text-muted': theme.textMuted,
        border: theme.border,
      }
    }
  }
}
```

### Integrate with CSS Variables

```js
// Apply a theme as CSS variables
function applyTheme(themeId, mode = 'dark') {
  const themes = require('./theme-presets.json')
  const theme = themes.find(t => t.id === themeId)[mode]
  
  const root = document.documentElement
  root.style.setProperty('--bg', theme.background)
  root.style.setProperty('--surface', theme.surface)
  root.style.setProperty('--accent', theme.accent)
  root.style.setProperty('--text-primary', theme.textPrimary)
  root.style.setProperty('--text-muted', theme.textMuted)
  root.style.setProperty('--border', theme.border)
}

applyTheme('stripe', 'dark')
```

---

## 📁 Repository Structure

```
auto-theme/
├── README.md
├── theme-presets.json          # 63+ complete theme presets (light + dark)
│
├── design-airbnb.md            # Full design system analysis
├── design-apple.md
├── design-claude.md
├── design-cursor.md
├── design-figma.md
├── design-linear.md
├── design-notion.md
├── design-stripe.md
├── design-tesla.md
├── ...                         # 63 brand design systems total
│
└── configs/                    # Compact copy-paste configs
    ├── design-airbnb-config.md
    ├── design-linear-config.md
    └── ...                     # 70 lightweight configs
```

---

## 🎯 What's in Each Design File?

Every `design-{brand}.md` file contains a deep analysis including:

1. **Visual Theme & Atmosphere** — The overall aesthetic and design philosophy
2. **Color Palette & Roles** — Every color with its semantic role
3. **Typography Rules** — Font families, weights, sizes, spacing
4. **Component Patterns** — How buttons, cards, inputs are styled
5. **Motion & Animation** — Transition timings and easing functions
6. **Dark/Light Mode** — How the theme adapts across modes

Example from `design-linear.md`:
> *"Linear's website is a masterclass in dark-mode-first product design — a near-black canvas (#08090a) where content emerges from darkness like starlight. The overall impression is one of extreme precision engineering..."*

---

## 🔥 Most Popular Themes

Based on community feedback, these themes are fan favorites:

| Rank | Theme | Why Devs Love It |
|------|-------|-----------------|
| 🥇 | **Linear** | The gold standard of dark UI |
| 🥈 | **Stripe** | Gradient mastery, premium feel |
| 🥉 | **Vercel** | Minimal perfection |
| 4 | **Raycast** | Productive & vibrant |
| 5 | **Notion** | Clean, focused reading |
| 6 | **Supabase** | Friendly open-source energy |
| 7 | **Cursor** | Developer IDE precision |
| 8 | **Framer** | Motion-first beauty |

---

## 🤝 Contributing

We welcome contributions! The best way to contribute is to add a new brand's design system.

### How to add a new theme

1. Fork this repository
2. Create `design-{brand}.md` with the full design analysis
3. Create `configs/design-{brand}-config.md` with the compact config
4. Add an entry to `theme-presets.json`
5. Open a Pull Request

### Theme file template

```markdown
# Design System Inspired by {Brand}

## 1. Visual Theme & Atmosphere
[Describe the overall aesthetic...]

## 2. Color Palette & Roles
### Background Surfaces
- **Primary Background** (`#xxxxxx`): ...

### Text & Content
...

## 3. Typography Rules
...

## 4. Component Patterns
...
```

---

## 📊 Theme Count by Category

| Category | Count |
|----------|-------|
| AI & Dev Tools | 15 |
| Enterprise & SaaS | 14 |
| AI & LLM Providers | 8 |
| Design & Creative | 5 |
| Consumer & Lifestyle | 8 |
| Hardware & Automotive | 8 |
| Media & Publishing | 5 |
| **Total** | **63+** |

---

## 📄 License

MIT License — free to use in personal and commercial projects.

---

<div align="center">

**If this saved you time, please give it a ⭐**

*Built with love for developers who care about design*

</div>

---

## 🙏 Acknowledgements

The design system analyses and theme data in this repository are sourced from and inspired by the amazing work of:

- **[getdesign.md](https://getdesign.md/)** — A curated platform for exploring world-class design systems, providing deep visual analysis and color breakdowns of top products and brands.
- **[awesome-design-md](https://github.com/VoltAgent/awesome-design-md)** — An open-source collection of design system documentation in Markdown format, maintained by the VoltAgent team.

Huge thanks to these projects for making design knowledge accessible to every developer. 🎨
