# NP OSCE Leader V1.3.1 — GA4 Analytics

GA4 Measurement ID: `G-VB3DB6S6EB`

## 會送出的網站事件
- `app_open`
- `mode_select`
- `track_select`
- `case_style_select`
- `random_case`
- `case_start`
- `station_enter`
- `case_review`
- `case_complete`
- `case_timeout`

## case_complete parameters
- case_id
- track
- category
- mode
- selected_style
- case_style
- core_score
- communication_bonus
- history_hits / history_total
- pe_hits / pe_total
- investigation_hits / investigation_total
- management_hits / management_total
- diagnosis_correct
- core_miss_count
- low_value_count
- pinned_note_count
- timed_out

## 不會送到 GA4
- 姓名
- Email
- 自由輸入 History 問句
- Scratchpad 內容
- Communication 自由文字
- 病人資料

此 GA4 Property 僅供 NP OSCE Leader 使用，不與 ICU Communication Platform 或 ACLS Code Leader 共用。
