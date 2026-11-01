# 11/15 讓心放鬆，找回幸福的力量

2026/11/15（日）14:30–16:30，14:00入場。東橋里活動中心，臺南市永康區東橋十街158號。
講師：周明輝院長。報名：郭小姐0953-056-201。主辦：社團法人台灣法輪大法學會。

## 網站

網站入口：index.html；設定：config.js。已套用新的 GAS /exec 網址，沿用 Meta Pixel。
原始活動海報：assets/images/1115-original.jpg。
未經確認的免費、茶席安排及舊場次細分流程已移除。

## GAS 更新（必要）

GitHub 中的 GAS 程式不會自動同步到 Apps Script。
1. 開啟「20261115幸福茶席報名名單」→ 擴充功能 → Apps Script。
2. 用 gas/Code.gs 完整取代原 Code.gs；用 gas/Analytics.gs 完整取代原 Analytics.gs（沒有則新增）。不要把兩份程式重複貼入。
3. 儲存，執行 setupRegistrationSheet，完成 Google 授權。
4. 要啟用流量報表，執行 setupAnalyticsDashboard；會建立每分鐘更新觸發條件。
5. 部署 → 管理部署作業 → 選目前提供給網站的部署 → 編輯 → 版本選「新版本」→ 部署。保留原 /exec 網址。
6. 開啟 /exec 應顯示 service:1115-happiness-registration、eventId:2026-11-15-happiness-tainan、registrationClosed:false。
7. 用網站送出測試報名，確認新試算表收到資料。完成前不要宣稱報名功能已驗證。

程式已固定連到新試算表，避免舊 SPREADSHEET_ID 設定造成誤寫。
網站只有在後端回覆正確活動編號與開放狀態時才允許送出；後端未更新時會顯示電話報名。

## 檢查紀錄

已執行 JavaScript 語法檢查與本機模擬測試：活動編號隔離、新試算表選擇、報名寫入、重送冪等、報名查核、人數限制。
本機測試不會寫入正式報名名單；真實報名驗證需先更新 GAS 部署。
