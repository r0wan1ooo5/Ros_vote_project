# 資料庫期末小組專題：線上投票系統  

## 動機  
台灣作為民主國家，投票系統是決策過程中不可或缺的重要工具。然而，現有的傳統投票方式往往受限於時間與地點，缺乏即時性與便利性。因此，我們計劃設計一個線上投票系統，讓使用者能夠快速進行投票與表決，提升效率並符合現代化需求。

---

## 功能簡介與特色  

1. **登入/註冊**  
   - 註冊時需輸入投票名稱、最低候選人人數、最低聯署標準、投票人數上限與最低投票率要求。  
   - 系統生成開票金鑰與登入鑰匙，確保安全性與專屬性。
![螢幕擷取畫面 2024-11-24 041908](https://github.com/user-attachments/assets/34d809db-7102-4994-9b3e-313c0da4a8d0)
![螢幕擷取畫面 2024-11-24 042014](https://github.com/user-attachments/assets/a70f6658-9674-4601-91e6-3bf46a4d88c6)


2. **參選與聯署**  
   - 顯示最低候選人數與聯署標準。
   - 使用者可點選 `Stand for Election` 成為候選人並建立聯署資料。
![image](https://github.com/user-attachments/assets/7b286ae4-ab45-443c-9eeb-c258016fb33a)

3. **聯署（Cosign）**  
   - 候選人介紹將於 `Show More` 頁面展示，包括姓名、照片及政見。  
   - 使用者需註冊並登入後方能進行聯署，聯署頁面會顯示目前聯署份數。
   - 完成聯署資格後，將進一步推動投票階段。
![螢幕擷取畫面 2024-11-24 062638](https://github.com/user-attachments/assets/9fd6a2ed-ea50-4f37-b1b5-1d2fc9e7925e)
![螢幕擷取畫面 2024-11-24 044225](https://github.com/user-attachments/assets/f399be83-9429-4054-833d-253b5589bd09)

4. **投票**  
   - 當候選人數滿足最低要求時，投票功能啟用。登入後，選民可查看候選人資訊並投票。  
   - 系統設有防呆機制，防止重複投票。
   - 開票時需輸入主辦方提供的開票金鑰，完成後即顯示結果。
![螢幕擷取畫面 2024-11-24 044701](https://github.com/user-attachments/assets/c3364e6f-ced4-4cf7-b752-e1a82583abf7)
![螢幕擷取畫面 2024-11-24 044724](https://github.com/user-attachments/assets/1ff517b6-4076-4a74-a972-e3bc6854cbf4)

5. **投票結果**  
   - 系統顯示最終得票數及當選名單，確保透明與公平。
![螢幕擷取畫面 2024-11-24 055102](https://github.com/user-attachments/assets/052eb6f3-c3d0-4d04-a7c3-921f979222d3)

---

## 瓶頸與待解決問題  

1. 我們初步設計了兩種投票模式：  
   - **公投模式**：需聯署達標後進入投票階段，並以支持率及最低投票率作為判定依據。  
   - **選舉模式**：無需聯署，直接進行候選人登記，依得票率決定當選者。  

   然而，兩種模式的實作過程中，因聯署與投票階段的時間限制及判定邏輯過於複雜，無法成功實現。我們最終改為以系統直接檢查條件是否達標，若符合標準即可開啟投票功能，簡化了流程。

2. **時間判定的挑戰**：  
   原計劃以時間設置聯署階段及投票階段的啟動與截止，但技術執行上未達預期，改以條件達成後即進入下一階段，確保穩定性。

---

## 專題成果與心得  

本專題從無到有的實作過程，讓我們學習了大量未曾接觸的技術，包括：  
- **資料庫應用**：設計結構化的資料表與其間的關聯性。  
- **前端設計**：運用 HTML/CSS 架設網站介面，並加入互動功能與動畫效果。  
- **後端邏輯**：以 PHP 進行伺服器端程式開發與資料處理，確保資料安全與功能完整性。  
- **前後端整合**：使系統能順暢執行並提供友善的使用者體驗。  

雖然過程中面臨了不少挑戰，但透過團隊合作與不斷嘗試，最終成功完成專題並展現了成果。
