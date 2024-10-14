# Google Maps 評論爬蟲程式

這個程式可以從 Google Maps 上爬取特定地點的評論資訊。

Strip Fork From [omkarcloud google-maps-reviews-scraper](https://github.com/omkarcloud/google-maps-reviews-scraper) 

## 安裝

1. 確保您已安裝 Python 3.6 或更高版本。

2. 克隆此存儲庫或下載源代碼。

3. 在專案目錄中,使用以下命令安裝所需的依賴套件:

   ```
   pip install -r requirements.txt
   ```

## 使用方法

1. 打開 `query_reviews.py` 文件。

2. 找到 `__main__` 部分,修改 `google_map_url` 變數為您想爬取評論的 Google Maps 地點網址。

3. 如果需要,可以修改 `n_reviews` 參數來指定要爬取的評論數量。

4. 在命令列中執行以下指令:

   ```
   python query_reviews.py
   ```

5. 程式將開始爬取評論,並將結果保存在當前目錄下的 `outputs.csv` 文件中。

## 注意事項

- 請遵守 Google 的服務條款和爬蟲政策。
- 過於頻繁的請求可能導致您的 IP 被暫時封鎖。
- 本程式僅供學習和研究使用,請勿用於商業目的。

## 輸出說明

爬取的評論將以 CSV 格式保存,包含以下欄位:

- retrieval_date: 爬取日期
- rating: 評分 (1-5 星)
- relative_date: 評論發布的相對日期
- user_name: 評論者名稱
- text: 評論內容
- ...（其他欄位）

## 疑難排解

如果遇到問題,請檢查:

1. 網路連接是否正常
2. Google Maps 網址是否正確
3. 是否已正確安裝所有依賴套件

如果問題持續,請提交 issue 或聯繫開發者。
