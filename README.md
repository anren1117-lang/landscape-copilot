# AI Landscape Copilot · 原生植物景觀規劃

> Free, browser-based AI landscape design tool for Taiwan — generates a layered native-plant landscape from your space, light, water budget, and goals. Photorealistic preview, 3D isometric view, top-down plan, year-round bloom and care calendars, install guide, sustainability metrics, 140+ plant dictionary.
>
> 為台灣的陽台、頂樓、庭院打造的免費 AI 景觀規劃工具：5 分鐘從光照、水分、空間生成台灣原生植物復層配置 — 含 AI 實景參考、3D 等角視角、俯瞰平面圖、花期月曆、養護月曆、施工指南、5 年成本估算、災害準備、140+ 種植物字典。

**[Live · 線上版本](https://anren1117-lang.github.io/landscape-copilot/)** · MIT License

---

## What it does

A 5-step wizard captures your context:

1. **Space type** — 陽台 / 頂樓 / 庭院 / 室內
2. **Space details** — actual address (Nominatim geocoding) + width × depth + orientation. Includes an inline area estimator (📐 common objects / 👣 walking paces / ◻️ floor tiles).
3. **Sunlight** — full / part / shade
4. **Water budget** — low / medium / high
5. **Goals** — pollinator / screen / edible / low-maintenance

Then generates a result page with 9 tabs:

| Tab | What it shows |
|---|---|
| **實景參考 · Realistic** | 3 AI-generated photorealistic landscape previews via pollinations.ai (free, no API key) |
| **俯瞰平面圖 · Plan** | Top-down SVG using your real width × depth, with orientation-aware sun marker |
| **3D 視角 · 3D View** | 30° isometric SVG with cylindrical trunks, crown ellipses, ground shadows |
| **復層配置 · Layered Design** | Vertical section diagram — canopy → shrub → ground → water → climber |
| **花期月曆 · Bloom Calendar** | 12-month grid of bloom × fruit timing across recommended plants |
| **養護月曆 · Care Calendar** | Auto-generated month-by-month tasks: prune, fertilize, pest watch, seasonal warnings |
| **施工指南 · Build Plan** | 8-phase install sequence + soil-recipe calculator + Taiwan-specific hazard preparedness (颱風 / 淹水 / 乾旱 / 寒流) |
| **採購清單 · Shopping List** | Editable per-plant qty with NT$ subtotals + 5-year cost-of-ownership projection |
| **植物字典 · Plant Dictionary** | 140+ plants, filterable by tier / native vs introduced / fragrance / pet-safe / search |

## Plant database

**140+ species** covering:

- Taiwan endemic conifers (紅檜 Formosan Cypress, 台灣肖楠, 樟葉楓)
- Native canopy (樟樹, 茄苳, 楓香, 台灣欒樹, 雀榕, 楊梅, 苦楝, 烏心石)
- Coastal natives (海桐, 黃槿, 水黃皮, 草海桐, 福木, 馬鞍藤)
- Edible fruit trees (龍眼, 荔枝, 芒果, 木瓜, 番石榴, 楊桃, 釋迦, 蓮霧)
- Taiwan endemic orchids (蝴蝶蘭 Phalaenopsis — Taiwan is the global breeding mother)
- Iconic street trees (鳳凰木, 阿勃勒, 大花紫薇, 火焰木, 印度紫檀)
- Indoor classics (黃金葛, 虎尾蘭, 龜背芋, 蔓綠絨, 白鶴芋, 馬拉巴栗)
- Succulents (蘆薈, 龍舌蘭, 玉露, 石蓮花, 翡翠木, 仙人掌)
- Edible vegetables and herbs (九層塔, 紫蘇, 香茅, 龍葵, 韭菜, 蝶豆花)
- Mediterranean herbs (薰衣草, 迷迭香, 鼠尾草)

Each plant carries:

- Bilingual name + Latin
- Tier (canopy / shrub / ground / water / climber)
- Sun, water, height, spread requirements
- Bloom + fruit months
- Native flag + origin
- Years to mature, fragrance level, pet-safety
- Common pests / diseases
- Water L/week + CO₂ kg/year estimates
- Sourcing hints (花市 / 林試所 / 特生中心 / 海岸復育苗圃 / etc.)
- Companion plants
- Ethnobotanical / cultural significance (where applicable)
- Specific Taiwan wildlife it attracts (台灣藍鵲, 五色鳥, 大鳳蝶, 蜻蜓, etc.)

## Tech

- **Single HTML file**, no build step, runs offline (except address geocoding and AI preview)
- Pure vanilla JS — no framework
- Real geocoding via **OpenStreetMap Nominatim** (free, no key)
- Realistic preview via **pollinations.ai** (free, no key)
- Hosted on **GitHub Pages**

## Local development

Just open `index.html` in any browser. No build step.

```bash
open index.html
```

## License

MIT
