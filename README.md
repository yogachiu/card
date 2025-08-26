# 小卡紀錄系統
## 專案動機
許多韓團粉絲熱衷於收集專輯小卡，但收藏與交易的資訊分散，也缺少好用的管理工具。這個系統希望提供一個方便的平台，讓使用者可以輕鬆記錄自己擁有的卡片、找到想買的卡片賣家，也能整理自己的交易紀錄，幫助解決資訊零散、難以管理的困擾，讓收藏和交易變得更有效率、更有條理。
## 參與內容
- 資料庫設計
- 系統功能發想與流程規劃
- 使用者、管理者介面程式撰寫
- 系統測試
## 技術
- Microsoft SQL Server：資料庫系統，負責儲存與管理會員、卡片資訊與交易紀錄
- ASP.NET MVC：採用 ASP.NET 的 MVC 架構開發網站，負責處理用戶請求，並與資料庫整合

## 系統功能
### Demo影片：https://drive.google.com/file/d/1WVOU066-1dhY4blxXctC7CDZkX80Fl1V/view?usp=sharing

### 分為會員 / 管理者介面：  
### <mark> 會員介面 </mark>
- 登入/登出：
  ![image](https://github.com/user-attachments/assets/08f611e7-f870-4243-b592-a2a2a096833e)
  
- 註冊：
  ![image](https://github.com/user-attachments/assets/4bca0ca2-7bb9-4af7-8a80-9955af6738ca)
  
- 會員可查看、新增所屬卡片：
  ![image](https://github.com/user-attachments/assets/ef7a54fe-bc5d-4059-98b4-9d1c005a1d3b)
  ![image](https://github.com/user-attachments/assets/d5b01144-1c93-46ef-95d0-f6b0726fc858)

- 會員可查看、新增交易紀錄：
  ![image](https://github.com/user-attachments/assets/b87ac44a-f29b-455d-a634-88e074a59c90)
  ![image](https://github.com/user-attachments/assets/8d796b5b-45f9-454c-844f-2b3b9c8cfe5b)

- 查詢：會員可查詢心儀卡片，系統會顯示擁有這張卡片的會員資料，使用者可以去連絡擁有這些卡片的會員：
  ![image](https://github.com/user-attachments/assets/6e8cb5d4-2559-447f-a9e0-c29b5bb43157)
  ![image](https://github.com/user-attachments/assets/fabf1c96-d820-44dd-98b8-9b3b43a77319)
  
- 使用者：會員可查看、編輯個人資料：
  ![image](https://github.com/user-attachments/assets/ed4095ec-cbf6-4313-ac23-feed3a1a4a65)
  ![image](https://github.com/user-attachments/assets/19919a30-298a-4f2d-abb0-bec95254e68c)
### <mark> 管理者介面 </mark>
- 以管理者的身分登入後會顯示所有會員的資料(每五筆資料一頁)<br>管理者可以查看、編輯、刪除使用者資料：
  ![image](https://github.com/user-attachments/assets/82c8e9c5-66c9-407a-9324-4f576e256773)

- 新增使用者資料：管理者可以指派管理權限(isManager)
  ![image](https://github.com/user-attachments/assets/c6fd2883-7294-4aaf-b7ea-87308ba9e871)

- 管理者可查看、修改個人資料
  ![image](https://github.com/user-attachments/assets/f6ea378b-4ca9-4ac0-b4dc-c631e3af5053)
  ![image](https://github.com/user-attachments/assets/3c2a1c8d-4720-4c8c-a698-514c8a1a9172)

- 點選會員詳細資料下面的按鈕，可查看該會員所屬卡與交易紀錄（不具編輯功能）
  ![image](https://github.com/user-attachments/assets/b61506bf-dde4-4923-b114-1192a8002486)
  ![image](https://github.com/user-attachments/assets/c32eb070-58d4-4ce8-a36c-90602f1e3789)

- 卡片資訊：顯示目前系統中所有的卡片資料
  ![image](https://github.com/user-attachments/assets/da258cea-cd85-4ea8-b6a3-e51ede1cef2a)
- 管理者可修改、新增、刪除卡片資料
  ![image](https://github.com/user-attachments/assets/21ed22b1-19d8-43ec-b62e-1c9afb70f3c0)
  ![image](https://github.com/user-attachments/assets/a65c20dc-7002-484e-a5c8-4b73124ed9a5)
  ![image](https://github.com/user-attachments/assets/dee1c397-1d1f-41b3-8278-3cf6b464f2ae)

## 專案心得
這是我們的第一個資料庫專案，從零開始，我們必須將課堂上所學的知識加以整合與應用，才能逐步建構出一個符合預期功能的完整系統。專案初期，我們遇到的第一個挑戰是資料庫設計：如何建立一個有邏輯又清楚的資料庫？資料表之間應該如何建立合理的關聯？這些設計上的決定對系統的運作有很大的影響，因此我們花了不少時間進行討論與調整。系統功能的設計，我們主要聚焦在核心功能的呈現，包括：會員與管理者介面、登入與註冊以及會員、小卡與交易紀錄的CRUD操作等。為了讓使用者操作更順暢，我們也設計了基本的輸入驗證機制，提升資料正確性與使用體驗。  

這個專案讓我深刻體會到，資料庫設計需要對整體系統有足夠的理解與敏銳度。功能與資料是密切相關的，我們在發想功能的過程中，經常需要回頭調整資料結構，因為初期難以全面預測所有需求。這讓我學到，資料庫設計需要經驗的累積，透過不斷實作，才能更快速、更精準地掌握資料表設計與關聯建立的方法，讓資料能精準對應到系統需求。此外，這個專案也讓我更深刻體會到團隊合作的力量。遇到問題時，大家一起討論、解決，確保專案順利推進，也讓我在過程中學到很多。雖然這是一個功能相對簡單的系統，但在此專案中，我們實際走過完整的資料庫設計與功能開發流程，也累積了寶貴的實作經驗，為未來更複雜的專案打下基礎。

