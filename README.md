# NP OSCE Leader V1.1.2 — Mg / mg/dL Mapping Fix

## 修正
- 修正 `Ca/Mg/Phos` 被錯配到 `POC glucose = 96 mg/dL` 的問題。
- 根因：文字比對把單位 `mg/dL` 中的 `mg` 誤判成 magnesium（Mg）。
- 現在所有常見濃度單位會先從 semantic matching 中移除。
- Myasthenia gravis 也改用 `mg_disease` 內部概念，不再和 magnesium 的 Mg 混在一起。
- IM30 Status Epilepticus 的電解質結果改為：
  - Na 132 mmol/L
  - K 3.8 mmol/L
  - ionized Ca 1.17 mmol/L
  - Mg 1.5 mg/dL（偏低）
  - Phos 2.6 mg/dL

© 2026 洪苡瑾・鄭介炬 版權所有｜未經授權請勿修改、重製、轉載或二次發布。
