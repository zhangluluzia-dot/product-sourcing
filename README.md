# Product Sourcing

A reusable, cross-industry Codex skill for finding and verifying products, materials, components, equipment, and suppliers across Chinese and international sources.

## What it does

- Searches Taobao, Tmall, JD.com, 1688, Pinduoduo, Amazon, specialist distributors, manufacturer sites, and other user-named sources.
- Handles retail products, wholesale supply, replacement parts, materials, equipment, packaging, private label, OEM, and ODM requests.
- Matches exact specifications, dimensions, materials, compatibility, performance, visual references, budget, quantity, destination, and deadline.
- Verifies the selected model or variant instead of trusting the lowest search-card price.
- Compares MOQ, samples, tooling, quantity tiers, supplier confidence, lead time, landed cost, warranty, support, and delivery risk.
- Produces quick shortlists, deep comparisons, substitute recommendations, supplier shortlists, and spreadsheet-ready procurement rows.

The skill is read-only by default. It never places orders, submits payment, changes a cart, contacts sellers, or accepts commercial terms without explicit user authorization.

## Industry coverage

- Furniture, fixtures, finishes, interiors, and construction materials
- Consumer goods, office products, appliances, and electronics
- Industrial components, tools, equipment, and replacement parts
- Packaging, printing, private label, OEM, and ODM
- Hospitality, foodservice, and commercial equipment

Industry-specific profiles preserve technical depth while the shared workflow handles evidence, supplier verification, cost, logistics, and risk consistently.

## Install in Codex

Ask Codex:

```text
Use $skill-installer to install https://github.com/zhangluluzia-dot/product-sourcing
```

Or clone it manually:

```powershell
git clone https://github.com/zhangluluzia-dot/product-sourcing "$HOME\.codex\skills\product-sourcing"
```

Restart Codex after installation if the skill does not appear immediately.

## Example requests

```text
Find five dining chairs on Taobao or Tmall that match this reference image. The width must be under 520 mm, the budget is RMB 900 per chair, and delivery to Shanghai must be possible within three weeks.
```

```text
Find qualified suppliers for this stainless-steel component. Compare the drawing requirements, material grade, tolerance capability, MOQ, sample process, production lead time, quality evidence, and landed cost for 2,000 units.
```

```text
Compare suppliers for custom printed retail packaging. Verify substrate, dimensions, print process, finish, tooling, MOQ, sample stages, defect allowance, production time, and shipping risk.
```

```text
Find an authorized or technically compatible substitute for this discontinued motor. Keep voltage, shaft dimensions, mounting, output, operating environment, and delivery deadline as hard constraints.
```

## 中文简介

Product Sourcing 是一个跨行业的 Codex 采购 Skill，可以搜索和比较中国及国际平台上的商品、材料、零部件、设备和供应商。它适用于零售采购、批量采购、替代品寻找、包装定制、贴牌生产、OEM/ODM 和供应商筛选。

它会根据技术规格、尺寸、材质、兼容性、参考图、预算、数量和交期进行筛选，并核对准确型号、MOQ、样品、模具费、阶梯价、供应商可信度、生产周期、到岸成本、保修和交付风险。默认只进行搜索与比较，不会未经允许下单、付款、修改购物车、联系供应商或接受商业条款。

## Package structure

```text
product-sourcing/
|-- SKILL.md
|-- agents/openai.yaml
`-- references/
    |-- comparison-schema.md
    |-- industry-profiles.md
    `-- marketplace-notes.md
```

## License

MIT

