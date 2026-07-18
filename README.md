# AI Landscape Copilot · 原生植物景觀規劃

> Free, browser-based AI landscape design tool for Taiwan — generates a layered native-plant landscape from your space, light, water budget, goals, plus optional criteria like existing plants and household constraints. Photorealistic preview, watercolor 3D isometric art view, top-down plan, year-round bloom and care calendars, install guide, sustainability metrics, per-design workspace with interactive layout editor, plant doctor, AI Q&A, and a 245-species plant dictionary.
>
> 為台灣的陽台、頂樓、庭院打造的免費 AI 景觀規劃工具：5 分鐘從光照、水分、空間生成台灣原生植物復層配置 — 含 AI 實景參考、水彩藝術 3D 視角、俯瞰平面圖、花期與養護月曆、施工指南、每個設計獨立的工作台（可互動排版、植物醫生、AI 問答）、以及 245 種植物字典。

**[Live · 線上版本](https://anren1117-lang.github.io/landscape-copilot/)** · MIT License

---

## What it does

### 5-step wizard captures your context

1. **Space type** — 陽台 / 頂樓 / 庭院 / 室內, plus L-shape or round shape support
2. **Space details** — actual address (Nominatim geocoding) + width × depth + orientation. Includes an inline area estimator (📐 common objects / 👣 walking paces / ◻️ floor tiles).
3. **Sunlight** — full / part / shade
4. **Water budget** — low / medium / high
5. **Goals** — pollinator / screen / edible / low-maintenance, plus an **Advanced** disclosure for existing plants, household (kids / pets / allergies), budget tier, privacy needs, native ratio target, wildlife focus, maintenance intensity, and aesthetic style

### Result page — 10 tabs

| Tab | What it shows |
|---|---|
| **實景參考 · Realistic** | 3 AI-generated photorealistic landscape previews via pollinations.ai (free, no API key) |
| **俯瞰平面圖 · Plan** | Top-down SVG using your real width × depth, with orientation-aware sun marker |
| **3D 視角 · 3D View** | 30° isometric SVG drawn as a botanical illustration plate in its geometry: lobed Bezier crowns full of individual green leaves with midveins, tapered trunks with root flare + bark striations, hatched-ink shadows, drawn balustrades on balcony walls, tile-grid floors, lily pads with V-notches + radial veins for water plants, alternating long/short sun rays, drawn clouds with rim strokes + soft undersides, and a "Ho, A. · pl. NNN · YYYY" plate signature. A 🎨 **Art view** toggle cycles 4 filter variants over the geometry — watercolor, ink wash, cyanotype, woodblock (木刻) |
| **復層配置 · Layered Design** | Vertical section diagram — canopy → shrub → ground → water → climber |
| **花期月曆 · Bloom Calendar** | 12-month grid of bloom × fruit timing across recommended plants |
| **養護月曆 · Care Calendar** | Auto-generated month-by-month tasks: prune, fertilize, pest watch, seasonal warnings |
| **施工指南 · Build Plan** | 8-phase install sequence + soil-recipe calculator + Taiwan-specific hazard preparedness (颱風 / 淹水 / 乾旱 / 寒流) |
| **採購清單 · Shopping List** | Editable per-plant qty with NT$ subtotals + 5-year cost-of-ownership projection |
| **植物字典 · Plant Dictionary** | 245 plants, filterable by tier / native vs introduced / fragrance / pet-safe / 🥗 edible / 🏹 indigenous / search |

### Per-design workspace

Every saved design gets its own dashboard:

- **🎨 Interactive layout editor** — drag plants around your space; auto-init uses tier-based drift planting (canopy at the back, ground cover in front, same species clustered around focal centers)
- **🧠 Why this design** — panel showing the structural rules, top-3 focal plants with reasons, and constraints derived from your inputs (existing plants avoided, pet-toxic suppressed, etc.)
- **📋 Today's list** — auto-seeded from this month's care calendar
- **💰 Budget editor** — auto plant + element cost + user line items + target progress bar
- **📸 Plant Doctor** — upload a leaf photo, get an AI diagnosis
- **💬 AI Q&A** — design-scoped conversation with pollinations.ai
- **📔 Garden journal** — per-design growth log
- **📤 Share** — copy link / LINE share / QR code (all self-contained in the URL hash)

## Plant database

**245 species** including 24 non-plant landscape elements (paths, planters, benches, water features, etc.) covering:

- Taiwan endemic conifers (紅檜 Formosan Cypress, 台灣肖楠, 樟葉楓)
- Native canopy (樟樹, 茄苳, 楓香, 台灣欒樹, 雀榕, 楊梅, 苦楝, 烏心石)
- Coastal natives (海桐, 黃槿, 水黃皮, 草海骨, 福木, 馬鞍藤)
- Edible fruit trees (龍眼, 荔枝, 芒果, 木瓜, 番石榴, 楊桃, 釋迦, 蓮霧)
- Taiwan endemic orchids (蝴蝶蘭 Phalaenopsis — Taiwan is the global breeding mother)
- Iconic street trees (鳳凰木, 阿勃勒, 大花紫薇, 火焰木, 印度紫檀)
- Indoor classics (黃金葛, 虎尾蘭, 龜背芋, 蔓綠絨, 白鶴芋, 馬拉巴栗)
- Succulents (蘆薈, 龍舌蘭, 玉露, 石蓮花, 翡翠木, 仙人掌)
- Edible vegetables and herbs (九層塔, 紫蘇, 香茅, 龍葵, 韭菜, 蝶豆花)
- Mediterranean herbs (薰衣草, 迷迭香, 鼠尾草)
- Indigenous-tradition plants (each carries the tribe or region of the note)

Each plant carries: bilingual name + Latin, tier, sun/water/height/spread, bloom + fruit months, native flag + origin, years to mature, fragrance level, pet-safety, common pests, water L/week + CO₂ kg/year estimates, sourcing hints, companion plants, ethnobotanical / cultural significance where applicable, and specific Taiwan wildlife it attracts (台灣藍鵲, 五色鳥, 大鳳蝶, 蜻蜓, etc.).

Every plant drawer carries a **📚 Sources & citations** block that credits each data category to its origin (Taiwan Biodiversity Atlas for names + native status, government forestry/agriculture atlases for fruit and vegetable species, Council of Indigenous Peoples records for tribal ethnobotany, 2024–2026 Taipei/Yilan nursery quotes for prices, published water-use and carbon-sequestration models for L/week + CO₂). A **📋 Copy citation** button inside that block writes a formatted academic-style citation (`Ho, A. (2026). AI Landscape Copilot: 〈plant name〉. 〈live URL〉`) to the clipboard for use in papers, blog posts, or grant applications.

## Design language

The whole app extends a **botanical illustration book** aesthetic: parchment cream palette (`#F1E6CB`) with sepia accents (`#7A5F42`), italic serif for chapter titles and captions, upright sepia serif small-caps for eyebrows, forest gradient for primary actions and active states, sepia gradient for warm secondary actions. Watercolor imagery (corner ornaments, botanical banner, space patterns, tier silhouettes, home wallpaper) is generated once via pollinations.ai and committed to `assets/` so the runtime is fully self-contained.

The 3D scene is drawn as illustration in its **geometry**, not just applied as a filter overlay. Turn every art filter off and each canopy visibly reads as 20 individual drawn leaves with midveins and radial venation inside a lobed Bezier silhouette. Trunks taper with root flare and bark striations; shadows are hatched ink strokes not soft blurs; balcony walls are drawn balustrades with pickets; pots have rim + striations + inner shadow; water plants render as botanical lily pads with V-notches, radial vein lines, and a 5-petal starburst flower; ground cover renders as scattered leaf clumps; wildflowers are 5-petal starbursts with golden centers. The classic bottom-right plate signature (`Ho, A. · pl. NNN · YYYY`) uses a stable per-design hash so the same design always shows the same plate number.

## Tech

- **Single HTML file** (`index.html`), no build step, runs offline (except address geocoding + AI image / Q&A / Plant Doctor)
- Pure vanilla JS — no framework
- 16 watercolor asset images (~220 KB) in `assets/`
- Real geocoding via **OpenStreetMap Nominatim** (free, no key)
- Realistic preview + AI Q&A + Plant Doctor via **pollinations.ai** (free, no key)
- Hosted on **GitHub Pages**
- Design + layout persisted to `localStorage`; portable via a `#d=` URL hash

## Local development

Just open `index.html` in any browser. No build step.

```bash
open index.html
```

## License

MIT
