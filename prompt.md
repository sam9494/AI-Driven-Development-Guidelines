目標：從prototype產出系統架構圖
目的：從全面需求中確定整體架構走向

這是PM 用ai studio做的prototype
在目前完全沒有系統的情況下
我是一個後端工程師，想要產生讓AI主導開發的方式
我要分別做什麼步驟
我的目標階段為
1. 了解並設計系統架構
2. 找出幾個小功能做出POC在測試環境用docker可以build起來，並在測試環境上可以demo
3. 用最低的成本deploy到生產環境
4. 根據市場環境改變資源 或是 實做下一個功能

幫我釐清我的步驟是否有缺乏，並幫我補充每一項的細節，有任何疑問或是建議請提出

--- 

目標：產生一個POC的任務清單
目的：在產生implementation plan前，產生一個給任務清單確認無誤

幫我先產生給非工程師看的任務清單
目標：AI 智能履歷
路徑：
1. 選擇google快速登入
2. 選擇理想的工作場景
3. 選擇技能
4.設定排班空檔
5. 進到首頁
6. 點擊Ai智能履歷


---
目標：產生implementation plan 方便之後實做
目的：implementation plan 不能太大，不然人沒辦法review，ai 跑歪也浪費token

根據 @AI智能履歷-用戶流程任務清單.md   和 @architecture_rationale.md 
產生給工程師看的implementation plan

先聚焦在步驟1
格式：
  實做的微服務
  異動資料表
  核心物件


  ---
目標：把專案的架構標準化
目的：在初步把架構標準化，減少未來要重構的成本

  幫我建立我的重構checklist
Result Pattern
Repository Pattern
CQRS (via MediatR)
Domain Events
Global Exception Handling:
Rich Domain Model


---
目標：把任務清單變成按照步驟implement plan
目的：把任務拆小，讓人可以review，讓ai可以控制輸出
輸出成implementation plan

@AI智能履歷-用戶流程任務清單.md 
把步驟 3：選擇技能 輸出成implementation plan
叫做【步驟 3：選擇技能implement_plan.md】
放在 @doc/AI-Resume-PocV2/backend_implementation_plan 

---
目標：poc畫面可以接api
目的：驗證後端產生的api至少可以滿足poc的需求

幫我依照 #file:UserService 有的api 對 #file:prototype 的前端做api串接計劃。
預計會有 #file:AI智能履歷-用戶流程任務清單.md 步驟 1：註冊帳號和步驟 2：選擇理想的工作場景
我要串接就好
不要管錯誤處理和資訊安全的東西
我只是要嘗試後端的api可以滿足poc的畫面
不需要多餘的東西
重新產生plan
先列出你的串接計劃到api_integration_plan.md
