# 1Now Design System Guide · v1.5
**For employees using Claude:** Attach this file to any Claude conversation when working on design or development tasks for 1Now. Claude will use this as the single source of truth for all visual decisions.

**Live visual reference:** https://arslanrajpoot9-pixel.github.io/1now-design-system/

---

## How to use this file with Claude

- **Designers:** Attach this file and ask Claude to review designs, write copy, or describe components.
- **Developers:** Attach this file and ask Claude to write HTML/CSS/React code using the exact class names and tokens below.
- **Marketers:** Attach this file when creating email templates, social posts, or ad creatives.

Always say: *"Use the 1Now Design System"* and Claude will apply these rules automatically.

---

## 00 · Brand Identity

**Product name:** 1Now  
**Tagline:** Make more money  
**Brand color:** `#FE7743` (Orange)  
**Font:** Inter only — no other typefaces permitted  
**Icon library:** Tabler Icons (`ti ti-*` classes)

---

## 01 · Color Tokens

### Primary (Orange)
| Token | Value | Usage |
|---|---|---|
| `--p` | `#FE7743` | Brand orange — buttons, active states, links |
| `--p-hover` | `#E8663A` | Button hover |
| `--p-active` | `#D45C32` | Button pressed |
| `--p-light` | `#FFF0EB` | Orange tinted backgrounds, badge bg |
| `--p-mid` | `#FDC5AD` | Orange tinted borders |
| `--p2` | `#FDB899` | Secondary orange accent |

### Secondary (Dark / Contrast)
| Token | Value | Usage |
|---|---|---|
| `--contrast` | `#3D3D3A` | Turo/contrast brand color |
| `--s` | `#121212` | Dark surface (Carisma AI, dark cards) |
| `--s-surface` | `#1A1A1A` | Dark card surface |
| `--s-border` | `#2A2A2A` | Dark card border |

### Backgrounds
| Token | Value | Usage |
|---|---|---|
| `--bg` | `#F7F7F5` | App background |
| `--page-bg` | `#ECECE8` | Page-level background |
| `--page-bg-deep` | `#E8E7E2` | Deeper page background |
| `--surface` | `#FFFFFF` | Card / panel surface |
| `--hover` | `#F0EFEA` | Hover state background |
| `--active-bg` | `#E8E7E2` | Active / pressed background |

### Borders
| Token | Value | Usage |
|---|---|---|
| `--border` | `#E7E7E2` | Default card/input border |
| `--border2` | `#D0D0CB` | Stronger border, button secondary |

### Text
| Token | Value | Usage |
|---|---|---|
| `--t1` | `#1F1F1D` | Primary text — headings, values |
| `--t2` | `#6C6C68` | Secondary text — labels, subtitles |
| `--t3` | `#9A9A95` | Muted text — hints, timestamps |
| `--t4` | `#C2C2BE` | Disabled / placeholder text |

### Semantic Colors
| Token | Hex | Usage |
|---|---|---|
| `--success` | `#2D7A4F` | Success text/icon |
| `--success-bg` | `#EDFAF3` | Success background |
| `--success-text` | `#1C6B40` | Success message text |
| `--warning` | `#8C5A00` | Warning text/icon |
| `--warning-bg` | `#FFF8EB` | Warning background |
| `--warning-text` | `#7A5000` | Warning message text |
| `--error` | `#B52B2B` | Error text/icon |
| `--error-bg` | `#FEF0F0` | Error background |
| `--error-text` | `#8B1E1E` | Error message text |
| `--info` | `#1A5DA8` | Info text/icon |
| `--info-bg` | `#EEF4FF` | Info background |
| `--info-text` | `#1A4E99` | Info message text |

### Orange Scale (Heat maps only)
| Step | Hex | Note |
|---|---|---|
| h1 (lightest) | `#FFF0EB` | |
| h2 | `#FFD9C8` | |
| h3 | `#FFB899` | |
| h4 | `#FF9166` | |
| h5 (brand) | `#FE7743` | ★ Brand color — midpoint |
| h6 | `#E55A26` | |
| h7 (darkest) | `#C4400E` | |

> **Rule:** Use dark text `#1a1a18` on h1–h4. Use white `#ffffff` on h5–h7.

---

## 02 · Typography

**Font:** `Inter` only. Optical sizing 14–32. All numbers use `font-variant-numeric: tabular-nums`.

### Type Scale
| Size | Weight | Usage |
|---|---|---|
| 32px / 700 / −0.02em | Bold | Hero metric (e.g. `$256,598`) |
| 24px / 600 / −0.015em | Semibold | KPI value |
| 20px / 700 | Bold | Page title, modal title |
| 16px / 600 | Semibold | Card title, section header |
| 14px / 500 | Medium | Table cell, nav label, button |
| 14px / 400 | Regular | Body copy, helper text |
| 13px / 400 | Regular | Secondary / subtitle |
| 12px / 400 | Regular | Captions, timestamps |
| 11px / 600 / UPPERCASE / +0.08em | Semibold | Overline labels ONLY |

### Weight Rules
| Weight | Name | Usage |
|---|---|---|
| 300 | Light | Large display numbers only |
| 400 | Regular | Body, captions, timestamps |
| 500 | Medium | Buttons, table cells, nav items |
| 600 | Semibold | KPIs, labels, overlines |
| 700 | Bold | Page titles, hero metrics |

> **Rules:**
> - Interactive elements never below weight **500**
> - Numbers always `tabular-nums`
> - Sentence case everywhere. UPPERCASE only for overline labels (11px, tracked)
> - Title Case for proper nouns only

---

## 03 · Spacing & Elevation

### Spacing Scale (4px base grid — no arbitrary values)
| Token | Value | Usage |
|---|---|---|
| `--s1` | 4px | Icon gaps, micro spacing |
| `--s2` | 8px | Element gap, inline spacing |
| `--s3` | 12px | Card internal gaps |
| `--s4` | 16px | Button padding, card gaps |
| `--s5` | 20px | Grid gaps, card padding |
| `--s6` | 24px | Section gaps |
| `--s8` | 32px | Large section separation |
| `--s10` | 40px | Page-level breathing room |
| `--s12` | 48px | — |
| `--s16` | 64px | — |

> ⛔ Arbitrary values (7px, 22px, 18px) are **prohibited**. If the grid doesn't fit, the layout is wrong.

### Border Radius
| Token | Value | Usage |
|---|---|---|
| `--r1` | 4px | Tags, small chips |
| `--r2` | 8px | Buttons, inputs, alerts |
| `--r3` | 12px | Cards, modals, kanban |
| `--r4` | 16px | Chart cards, hero card |
| `--r5` | 20px | Sidebar, DS tiles |
| `--rp` | 999px | Badges, live dots (pill) |

### Elevation / Shadows
| Token | Usage |
|---|---|
| `--shadow-sm` | Hover states, selected rows |
| `--shadow-md` | Dropdowns, popovers |
| `--shadow-lg` | Modals |
| `--shadow-float` | Floating sidebar — signature shadow |
| `--shadow-tooltip` | Tooltips |
| `--focus` | 3px orange focus ring — keyboard nav |

> **Rule:** Default cards use border only — no shadow. Add shadow only on hover or for floating elements.

---

## 04 · The Edge (v1.5)

The Edge is a **3px orange top border** — a signature visual device.

```css
--edge-width: 3px;
--edge-color: #FE7743;

/* Applied as: */
border-top: 3px solid #FE7743;
```

**Applied to:** Hero card · Floating sidebar top only.

> ⛔ **Never apply to:** KPI cards, chart cards, table containers, buttons, or any secondary element.
> **Principle:** The edge only works because it appears **once**. If every card has it, no card has it.

### Alert Left-Border System
Alerts use a **3px left border** in semantic color (same thickness, different axis):
- Warning: `border-left: 3px solid var(--warning)`
- Error: `border-left: 3px solid var(--error)`
- Info: `border-left: 3px solid var(--info)`

---

## 05 · Buttons

```html
<!-- Sizes -->
<button class="btn btn-sm">Small</button>       <!-- h:28px -->
<button class="btn">Default</button>             <!-- h:36px -->
<button class="btn btn-lg">Large</button>        <!-- h:44px -->
<button class="btn btn-xl">XL</button>           <!-- h:52px, r3 -->

<!-- Variants -->
<button class="btn btn-primary">Primary</button>
<button class="btn btn-secondary">Secondary</button>
<button class="btn btn-ghost">Ghost</button>
<button class="btn btn-danger">Danger</button>

<!-- States -->
<button class="btn btn-primary" disabled>Disabled</button>
<button class="btn btn-primary btn-loading"><i class="ti ti-refresh"></i> Loading</button>
```

| Class | Background | Border | Text |
|---|---|---|---|
| `btn-primary` | `--p` orange | `--p` | White |
| `btn-secondary` | `--surface` white | `--border2` | `--t1` |
| `btn-ghost` | Transparent | None | `--t2` |
| `btn-danger` | `--error` | `--error` | White |

> Disabled state: `opacity: 0.4`, `pointer-events: none`

---

## 06 · Inputs & Forms

```html
<!-- Basic input -->
<label class="inp-label">Label</label>
<input class="inp" placeholder="Placeholder" />
<span class="inp-hint">Helper text</span>
<span class="inp-error">Error message</span>

<!-- States via class -->
<input class="inp state-focus" />
<input class="inp state-error" />
<input class="inp state-disabled" />

<!-- With icon -->
<div class="inp-group">
  <i class="ti ti-search inp-icon"></i>
  <input class="inp" placeholder="Search..." />
</div>

<!-- Select -->
<div class="custom-select">
  <select class="inp">
    <option>Option 1</option>
  </select>
</div>
```

**Specs:** height 36px · padding 0 12px · border `--border` · radius `--r2` · focus: `--p` border + `--focus` shadow

---

## 07 · Cards & KPIs

### Basic Card
```html
<div class="card">Content</div>
```
Specs: `--surface` bg · `--border` border · `--r3` radius · 20px padding

### KPI Card
```html
<div class="kpi">
  <div class="kpi-ol"><i class="ti ti-currency-dollar"></i> Total Revenue</div>
  <div class="kpi-val">$35,340</div>
  <div class="kpi-delta up"><i class="ti ti-arrow-up"></i> +12%</div>
  <div class="kpi-sub">vs last month</div>
</div>
```
| Class | Usage |
|---|---|
| `kpi-ol` | Overline label (11px, uppercase, icon) |
| `kpi-val` | Main value (24px/600, tabular-nums) |
| `kpi-delta up` | Positive delta (green) |
| `kpi-delta dn` | Negative delta (red) |
| `kpi-sub` | Subtitle (12px, --t3) |

### Hero Card (uses The Edge)
```html
<div class="hero-card">
  <div class="hero-card-edge"></div>
  <div class="hero-card-body">Content</div>
</div>
```

---

## 08 · Alerts

```html
<div class="alert alert-success"><i class="ti ti-circle-check"></i> Message</div>
<div class="alert alert-warning"><i class="ti ti-alert-triangle"></i> Message</div>
<div class="alert alert-error"><i class="ti ti-x-circle"></i> Message</div>
<div class="alert alert-info"><i class="ti ti-info-circle"></i> Message</div>
```

---

## 09 · Badges & Tags

### Badges (pill shape)
```html
<span class="bdg" style="background:var(--success-bg);color:var(--success-text)">
  <span class="bdg-dot" style="background:var(--success)"></span>Active
</span>
```

### Tags (square-ish)
```html
<span class="tag">Default</span>
<span class="tag tag--primary">Primary</span>
<span class="tag tag--success">Success</span>
<span class="tag tag--error">Error</span>
<span class="tag tag--info">Info</span>
<span class="tag tag--turo">Turo</span>
```

---

## 10 · Tables

```html
<div class="tbl-wrap">
  <table class="tbl">
    <thead>
      <tr>
        <th>Name</th>
        <th class="r">Amount</th>
      </tr>
    </thead>
    <tbody>
      <tr><td>Row</td><td class="r">$100</td></tr>
      <tr class="row-sel"><td>Selected</td><td class="r">$200</td></tr>
      <tr class="row-total"><td>Total</td><td class="r">$300</td></tr>
      <tr class="row-sub"><td>Sub-row</td><td class="r muted">Detail</td></tr>
    </tbody>
  </table>
</div>
```

**Row modifier classes:**
- `row-sel` — selected row (orange tint)
- `row-total` — total/summary row (bold, grey bg)
- `row-sub` — indented sub-row
- `row-sub--active` — left border: orange
- `row-sub--pending` — left border: --p-mid
- `row-sub--cancelled` — left border: --contrast

---

## 11 · Toast Notifications (v1.5)

Dark background, bottom-center or top-right. Max-width 380px. Auto-dismiss 4s.

```html
<!-- Success -->
<div style="display:flex;align-items:center;gap:10px;padding:12px 14px;background:#1F1F1D;border-radius:8px;max-width:380px">
  <i class="ti ti-circle-check" style="color:#5FD39F"></i>
  <span style="font:500 13px Inter;color:#fff;flex:1">Booking confirmed · #79848</span>
  <span style="font:400 11px Inter;color:rgba(255,255,255,.45)">Undo</span>
</div>
```

**Toast icon colors (dark bg only — never use on light):**
| Type | Icon color |
|---|---|
| Success | `#5FD39F` |
| Error | `#FF8A80` |
| Progress/Info | `var(--p)` orange |
| Neutral | `rgba(255,255,255,0.5)` |

---

## 12 · Tabs & Navigation

### Style 1 — Pill Tabs (recommended for dashboards)
- Default: 14px/400, `--t2`, no background
- Active: 14px/600, `--t1`, white bg, `shadow-sm` + border
- Use for: dashboard page tabs, main content switching

### Style 2 — Segmented Control (2–4 options max)
- Container: `--hover` bg, `--r2`, 3px padding
- Active: white bg, `shadow-sm`, weight 600
- Default: 13px/400, `--t2`
- Use for: filter controls, report period selector

### Style 3 — Underline (legacy)
- Active: 14px/600, `--t1`, 2px `--p` bottom border
- Use only for: long content sections with many tabs

### Breadcrumb
```
Fleet / Mazda CX-30 / LXM 9080
```
- Ancestors: 13px/400, `--t3`, clickable
- Separator `/`: `--t4`
- Current (last): 13px/600, `--t1`, not clickable

---

## 13 · Modals & Overlays

```html
<div class="modal-backdrop"> <!-- rgba(31,31,29,.4) -->
  <div class="modal">
    <div class="modal-header">
      <div class="modal-title">Title</div>
      <button class="modal-close"><i class="ti ti-x"></i></button>
    </div>
    <p class="modal-body">Body text.</p>
    <div class="modal-footer">
      <button class="btn btn-secondary">Cancel</button>
      <button class="btn btn-primary">Confirm</button>
    </div>
  </div>
</div>
```

**Specs:**
- Backdrop: `rgba(31,31,29,.4)`
- Confirm modal: max-width 480px
- Form modal: max-width 720px
- Footer: right-aligned, `btn-secondary` left, primary action right

### Tooltip
- bg: `--t1` (dark) · color: white · 12px/500 · padding 6px 10px · `--r1` · `shadow-tooltip` · max-width 220px

---

## 14 · Layout & Sidebar

### App Layout
```
page-bg (--page-bg)
└── layout-demo
    ├── sb (sidebar — 220px, floating, shadow-float, edge top)
    │   ├── sb-header (logo + workspace selector)
    │   ├── sb-nav (groups + items)
    │   └── sb-bottom (user avatar + info)
    └── content-area (flex:1, white, rounded)
        ├── topbar (52px, breadcrumb + search + actions)
        └── page-content (28px padding, scrollable)
```

### Sidebar Classes
```html
<div class="sb sb-top">
  <div class="sb-header">
    <div class="sb-logo"><div class="sb-logo-icon"><i class="ti ti-bolt"></i></div><span class="sb-logo-name">1Now</span></div>
    <div class="sb-ws"><div class="sb-ws-dot">...</div><span class="sb-ws-name">Workspace</span></div>
  </div>
  <nav class="sb-nav">
    <div class="sb-group-label">Main</div>
    <div class="sb-item active"><i class="ti ti-home"></i> Dashboard</div>
    <div class="sb-item"><i class="ti ti-calendar"></i> Bookings <span class="sb-badge">3</span></div>
    <div class="sb-divider"></div>
  </nav>
  <div class="sb-bottom">
    <div class="sb-user">
      <div class="sb-avatar">AR</div>
      <div class="sb-user-info">
        <div class="sb-user-name">Arslan</div>
        <div class="sb-user-email">arslan@1now.ai</div>
      </div>
    </div>
  </div>
</div>
```

### Topbar Classes
```html
<div class="topbar">
  <div class="topbar-breadcrumb">
    <span>Fleet</span><span class="sep">/</span><span class="current">Dashboard</span>
  </div>
  <div class="topbar-search"><i class="ti ti-search search-icon"></i><input placeholder="Search..."/></div>
  <div class="topbar-actions">
    <button class="topbar-btn"><i class="ti ti-bell"></i><span class="notif-dot"></span></button>
    <div class="topbar-avatar">AR</div>
  </div>
</div>
```

---

## 15 · Interaction States

| State | Visual |
|---|---|
| Default | Border only |
| Hover | `--hover` background (`#F0EFEA`) |
| Active/Pressed | `--active-bg` background (`#E8E7E2`) |
| Focus | 3px orange ring — `--focus` shadow |
| Disabled | `opacity: 0.4`, `cursor: not-allowed`, `pointer-events: none` |
| Skeleton/Loading | Shimmer animation — `class="skel"` |

---

## 16 · Charts

**Color usage in charts:**
- 1Now data: `#FE7743` (orange) — solid bars, solid lines
- Turo data: `#3D3D3A` (contrast) — dashed lines
- Area fill: orange gradient (0.18 → 0 opacity)
- Grid lines: `#F0EFEA`
- Axis labels: `#9A9A95`, 10px, Inter

**Chart container:**
```html
<div class="chart-container">
  <div class="chart-header">
    <div><div class="chart-title">Revenue</div><div class="chart-sub">Jan–Jun 2026</div></div>
    <div class="chart-controls">
      <button class="chart-ctrl active">6M</button>
      <button class="chart-ctrl">12M</button>
    </div>
  </div>
  <div class="chart-legend">
    <div class="chart-legend-item"><div class="chart-legend-dot" style="background:#FE7743"></div>1Now</div>
  </div>
  <!-- SVG chart here -->
</div>
```

**Tooltip spec (dark):** bg `#1F1F1D` · white text · 12px · padding 6px 10px · `--r1` · `shadow-tooltip`

---

## 17 · Kanban Cards

```html
<div class="kanban">
  <div class="kanban-id">#79848</div>
  <div class="kanban-name">John Smith</div>
  <div class="kanban-company">Turo · 3 days</div>
  <div class="kanban-email">john@email.com</div>
  <div class="kanban-tags">
    <span class="tag tag--success">Active</span>
    <span class="tag tag--info">Paid</span>
  </div>
</div>
```

---

## 18 · Empty States & Skeletons

### Empty State
```html
<div style="text-align:center;padding:32px 20px;border:1px solid var(--border);border-radius:var(--r3)">
  <div style="width:48px;height:48px;border-radius:var(--r3);background:var(--hover);display:flex;align-items:center;justify-content:center;margin:0 auto 16px">
    <i class="ti ti-calendar-off" style="font-size:22px;color:var(--t4)"></i>
  </div>
  <div style="font:600 15px Inter;color:var(--t1);margin-bottom:6px">No bookings yet</div>
  <div style="font:400 13px Inter;color:var(--t3);margin-bottom:16px">Create your first booking to get started.</div>
  <button class="btn btn-primary">Create booking</button>
</div>
```

### Skeleton / Loading
```html
<div class="skel" style="height:20px;width:60%;margin-bottom:8px"></div>
<div class="skel" style="height:16px;width:40%"></div>
```

---

## 19 · Surface Map

The design system covers **5 surfaces**:

| Surface | Description |
|---|---|
| S01 · Product UI | Dashboard, sidebar, modals, tables — main app |
| S02 · Email | Transactional emails (billing, notifications) |
| S03 · Print / PDF | Invoices, reports |
| S04 · Social | Instagram/Facebook posts (1080×1080px, dark bg, Inter 800 ALL CAPS) |
| S05 · Ad creatives | Facebook/Google paid ads |

### S04 · Social Media Quick Rules
- Background: `#121212` dark OR `#FE7743` orange — never white
- Font: Inter 800 · ALL CAPS · white text
- Key words: `#FE7743` orange highlight
- Always include: 1Now logo + "Make more money" tagline
- Format: 1:1 square (1080×1080px)

### S02 · Email Rules
- Font stack: `-apple-system, Helvetica, Arial, sans-serif` (web-safe for email clients)
- CTA button: `background:#FE7743` · white text · `border-radius:10px` · `padding:17px 24px`
- Warning callout: `border-left:3px solid #d97706` on `#fffbeb` bg
- Footer: `#f7f7f5` bg · `#6c6c68` links

---

## 20 · Carisma AI Component

Carisma is the embedded AI assistant inside 1Now. Key classes:

```html
<div class="carisma-layout">
  <div class="carisma-sb">...</div>   <!-- 240px sidebar -->
  <div class="carisma-main">
    <div class="carisma-topbar">...</div>
    <div class="carisma-welcome">     <!-- centered welcome state -->
      <div class="carisma-prompts">   <!-- 2-col prompt grid -->
        <div class="carisma-prompt">  <!-- dark bg prompt card -->
          <div class="carisma-prompt-icon">...</div>
          <div class="carisma-prompt-text">
            <div class="carisma-prompt-title">Title</div>
            <div class="carisma-prompt-agent">Agent name</div>
          </div>
        </div>
      </div>
    </div>
    <div class="carisma-input-area">
      <div class="carisma-input-bar">
        <input placeholder="Ask Carisma anything..." />
      </div>
    </div>
  </div>
</div>
```

---

## 21 · Critical Rules (Never Break)

1. **Font:** Inter only. Never use system fonts in product UI.
2. **Spacing:** 4px grid only. No arbitrary pixel values.
3. **The Edge:** 3px orange top border on Hero card and sidebar top only — never duplicated.
4. **Colors:** Use CSS variables (`var(--p)`, `var(--t1)`) — never hardcode hex in product UI.
5. **Buttons:** Never below weight 500. Disabled = opacity 0.4 only.
6. **Numbers:** Always `font-variant-numeric: tabular-nums`.
7. **Text case:** Sentence case everywhere. UPPERCASE only for 11px overline labels.
8. **Toast colors** (`#5FD39F`, `#FF8A80`): Dark background only — never on light.
9. **Modals:** Backdrop `rgba(31,31,29,.4)`. Footer right-aligned. Cancel left, confirm right.
10. **Icons:** Tabler Icons (`ti ti-*`) only.

---

*1Now Design System v1.5 · May 2026 · Generated from design-system HTML file*
