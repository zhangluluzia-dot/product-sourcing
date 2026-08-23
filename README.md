# FF&E Product Sourcing

A reusable Codex skill for sourcing furniture, fixtures, equipment, finishes, and interior materials across Chinese and international marketplaces.

## What it does

- Searches Taobao, Tmall, JD.com, 1688, Pinduoduo, Amazon, Wayfair, IKEA, and other user-named retailers.
- Matches products against reference images, dimensions, materials, colors, budget, quantity, destination, and delivery deadline.
- Verifies the exact product variant instead of trusting the lowest search-card price.
- Compares known landed cost, seller confidence, delivery risk, return terms, and unresolved questions.
- Produces quick shortlists, deep comparisons, substitute recommendations, and spreadsheet-ready procurement rows.

The skill is read-only by default. It never places orders, submits payment, contacts sellers, or adds items to a cart without explicit user authorization.

## Install in Codex

Ask Codex:

```text
Use $skill-installer to install https://github.com/YOUR_GITHUB_USERNAME/ffe-product-sourcing
```

Or clone it manually:

```powershell
git clone https://github.com/YOUR_GITHUB_USERNAME/ffe-product-sourcing "$HOME\.codex\skills\ffe-product-sourcing"
```

Restart Codex after installation if the skill does not appear immediately.

## Example requests

```text
Find five dining chairs on Taobao or Tmall that match this reference image. The width must be under 520 mm, the budget is RMB 900 per chair, and delivery to Shanghai must be possible within three weeks.
```

```text
Compare these 1688 sofa listings. Verify the selected fabric and size, calculate the known cost for 12 units, and flag MOQ, production-time, packaging, and freight uncertainties.
```

```text
Find a Wayfair or Amazon substitute for this unavailable bedside table. Keep the width, finish, budget, and delivery deadline as hard constraints.
```

## 中文简介

FF&E Product Sourcing 是一个面向室内设计与采购工作的 Codex Skill。它可以搜索淘宝、天猫、京东、1688、拼多多、Amazon、Wayfair 等平台，根据参考图、尺寸、材质、颜色、预算、数量和交期筛选商品，并核对准确规格、到手成本、卖家可信度、退换条件与交付风险。

它默认只进行搜索和比较，不会未经允许下单、付款、联系卖家或加入购物车。

## Package structure

```text
ffe-product-sourcing/
|-- SKILL.md
|-- agents/openai.yaml
`-- references/
    |-- comparison-schema.md
    `-- marketplace-notes.md
```

## License

MIT

