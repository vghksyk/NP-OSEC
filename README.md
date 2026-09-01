# NP OSCE Leader V1.0.4 — Clinical Intent Mapping

## 自由輸入重大更新
自由輸入不再只依完整字面比對，而是加入 clinical concept mapping。

可辨識例如：
- 「停酒？」「BZD？」「戒斷？」 → alcohol / benzodiazepine withdrawal
- 「最近睡覺要墊高嗎？」 → orthopnea
- 「半夜會喘醒嗎？」 → PND
- 「體重最近有變重嗎？」 → rapid weight gain
- 「有漏吃利尿劑嗎？」 → diuretic adherence
- 「喝水會嗆嗎？」 → bulbar symptom / airway protection
- 「尿像茶嗎？」 → dark urine
- 「大便變白嗎？」 → pale stool
- 「濕尿布幾片？」 → pediatric urine output
- 「幾週生？」 → birth history

## 設計原則
- 同義說法、縮寫、短關鍵字可以辨識。
- 問錯 clinical concept 仍不會取得答案。
- 不把系統放寬到「什麼都算對」。
- unmatched 時虛擬病人回覆改為多種中性句，降低鬼打牆感。

© 2026 洪苡瑾・鄭介炬 版權所有｜未經授權請勿修改、重製、轉載或二次發布。


## 同版併入：History 點選紀錄修正
- 修正預設 History 按鈕綁定 click 後，又因 `innerHTML +=` 重建 DOM，可能導致已點問題未記錄的問題。
- 改用 `insertAdjacentHTML` 保留既有 event listener。
- IM11 acute pulmonary edema 核心病史改成完整問句：
  - orthopnea / PND
  - rapid weight gain
  - diuretic adherence
