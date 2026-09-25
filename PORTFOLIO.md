![工作坊完成徽章](https://img.shields.io/badge/GitHub_Copilot_實戰工作坊-已完成-1F883D?style=for-the-badge&logo=githubcopilot&logoColor=white)
# 今日待辦 Web App

這是一個在 GitHub Copilot 實戰工作坊中完成的待辦清單 Web App。專案從基本的待辦管理開始，逐步加入主題切換、篩選與批次清理功能，並保留使用者在瀏覽器中的資料。

## 線上展示

https://sammtcbn.github.io/github-copilot-bootcamp2006/

## 功能

- 新增待辦事項，空白內容不會被加入。
- 勾選待辦事項為已完成，完成項目會顯示刪除線並淡化。
- 刪除單筆待辦事項。
- 清除所有已完成項目，操作前會顯示瀏覽器確認對話框。
- 沒有已完成項目時，「清除已完成」按鈕會停用。
- 顯示整體未完成項目數量。
- 使用「全部」、「未完成」、「已完成」篩選待辦事項。
- 篩選結果為空時顯示對應提示文字。
- 支援淺色與深色模式切換。
- 沒有手動選擇主題時，會跟隨作業系統的深淺色設定。
- 記住使用者選擇的主題偏好。
- 使用 `localStorage` 保存待辦資料，重新整理後資料仍會保留。
- 支援手機螢幕的響應式版面。

## 技術

- 使用純 HTML、CSS 與原生 JavaScript。
- 不使用任何框架、套件或外部 CDN。
- CSS 顏色透過 `:root` 的 CSS 變數管理，包含淺色與深色主題。
- 使用 `localStorage` 保存待辦資料與主題偏好。
- 使用 `textContent`、`createElement` 等原生 DOM API 產生清單內容。

## 開發方式

- 使用 GitHub Copilot Agent Mode，從需求開始建立待辦清單的頁面結構、樣式與互動邏輯。
- 透過 MCP 讀取 Microsoft Learn 文件，參考 `prefers-color-scheme` 與網頁無障礙色彩對比的官方建議。
- 透過 GitHub MCP 讀取 issue，依照 issue 描述規劃修改、建立分支、驗證功能、提交並開 Pull Request。
- 使用 `.github/prompts` 中的 `fix-issue.prompt.md` 建立固定的 agentic workflow，讓 issue 修正遵循讀取、確認、修改、驗證、提交與開 PR 的流程。

## 我學到什麼

- 學會使用 CSS 變數與 `prefers-color-scheme` 設計可切換且可跟隨系統設定的主題。
- 理解如何用篩選狀態控制畫面顯示，同時維持完整資料與整體未完成數量的正確性。
- 熟悉使用 `localStorage` 保存前端資料，讓頁面重新整理後仍能還原狀態。
- 練習透過 MCP 查詢官方文件與 GitHub issue，將需求轉換成可驗證的開發工作。
- 了解 Agent Mode 與 agentic workflow 如何協助規劃、修改、測試與交付小型功能。