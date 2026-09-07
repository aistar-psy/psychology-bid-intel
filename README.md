# 🧠 心理招标情报周报 · psychology-bid-intel

GB 端心理健康招投标 / 采购意向 / 商机速递站点，**每周一自动更新**（自动化任务 `automation-1788750000365`）。

## 🌐 访问

GitHub Pages：**https://aistar-psy.github.io/psychology-bid-intel/**

| 页面 | 内容 |
|---|---|
| `index.html` | 首页速览：KPI 仪表盘 + 本周头条 + P0 商机 + 趋势观察 + 历史归档 |
| `YYYY-MM-DD.html` | 各期周报详情（P0/P1/P2 分级、采购意向 TOP、省份分布、业务分类、政策动态、词库增补、动作清单） |
| `intents-YYYY-MM-DD.html` | 当期采购意向自动扫描明细（通道 A 标题命中 / 通道 B 公告落地） |

## 📁 结构

```
psychology-bid-intel/
├── index.html              # 首页速览（每期需追加历史归档链接）
├── assets/style.css        # 共享样式（勿改页面内联样式）
├── YYYY-MM-DD.html         # 每期周报详情
├── intents-YYYY-MM-DD.html # 每期采购意向扫描明细
└── README.md
```

## 🔄 更新方式（每周一自动化任务）

1. 扫描产出 md 报告 → 生成同日期 `YYYY-MM-DD.html` + `intents-YYYY-MM-DD.html`
2. 更新 `index.html`：
   - 替换「本期速览 / 本周头条 / P0 / 趋势观察 / 主动作」为当期内容
   - 在「历史归档」顶部插入新期卡片链接
3. commit & push 到 `main`（Pages 自动发布）

## 📊 数据口径

- **省份优先级**：吉林 / 上海（闵行）/ 海南 / 江西（吉安·吉水）> 全国
- **词库版本**：V1.3（8 词族 147 词根，关注业主 81 单位 × 6 归口线）
- **商机分级**：P0 极对口（本周对接）/ P1 强烈跟进（高匹配+大额）/ P2 关注（行业风向+竞品）
- **来源**：ccgp.gov.cn 采购意向公开库（WebSearch 聚合路径，受 WAF 自动降级）+ 各省政府采购门户 + 行业聚合站

---
© 2026 aistar-psy
