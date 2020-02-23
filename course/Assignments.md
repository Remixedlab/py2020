# Assignment #1 0920
如果你會寫第一題或第二題的話，那你就把這題用ipynb所另存成的.html檔給交上來就好。就不用做第三題。如果你第一、二題都做不出來的話，那就請完成第三題的練習。
1. 請把下列表格中的資料用dicationary與list表示後，指給（Assign）給一個變數。

id|area|district|price
---|---|---|---
a13248|18.5|信義區|17890000
a13249|21.3|信義區|20000000
a13250|32.1|信義區|36820000

2. 請用for-loop產生費氏數列的前50項並進行加總。

3. 請上Datacamp完成[Intro to Python for Data Science](https://www.datacamp.com/courses/intro-to-python-for-data-science)的練習。並用螢幕截圖擷取完成該單元的畫面（會獲得一個簡單的證書）成為.png或.jpg檔，上傳該圖檔即可。

# Assignment #2 0927
1. 自政府開放資料下載一個json檔，分別將其轉為層套的list或dictionary。針對該資料集：
    1. 說明你下載了哪個資料集的檔案，列出該資料集的名稱與超鏈結。
    2. 用程式列印出，該資料集包含幾筆資料。
    3. 用程式列印出，該資料集的主要資料表有哪些「變項」。這邊所指的「變項」為統計的「變項」。例如ubike的資料就有中文站名、英文站名等等。列印出的形式不拘。
    4. 嘗試用上週與本週所教的「計數counting」運算，統計其中一個變數。
2. 讀取json檔案的方法
```
with open("data/your_file.json", "r", encoding="UTF-8") as f:
    jdata = json.load(f)
print(type(jdata))
```
# Assignment #3 1004
1. 自政府開放資料下載一個CSV檔，分別將其轉為二層的list。針對該資料集：
    1. 說明你下載了哪個資料集的檔案，列出該資料集的名稱與超鏈結。
    2. 用程式列印出，該資料集包含幾筆資料。
    3. 用程式列印出，該資料集的主要資料表有哪些「變項」。這邊所指的「變項」為統計的「變項」。
    4. 嘗試用上週與本週所教的「計數counting」運算，統計其中一個變數。
2. 針對AQX的資料，依照[行政院環保署的標準](https://taqm.epa.gov.tw/taqm/tw/b0201.aspx)，讀取AQI的值，並在每一個站台的dictionary中，塞入一個新的key為"color"，用if-else判斷AQI所落在區間，指派顏色給每一個站台，而"color"會對應至該AQI應呈現的顏色（Green, Yellow, Orange, Red, Purple, Maroon）。
3. (option)將ubike data讀取後，轉為兩層的list所表示的格式，第0個list為欄位名稱。
4. (option)上網查詢要如何將這兩個list存為`.csv`檔。

# Assignment #4 1011
* 找到Dcard、104查詢頁面、或Pchome查詢頁面的json檔案網址並觀察其頁面遞增規則，抓取最少10個頁面的資料。並存為.pickle、.json檔各一份。
* 僅需完成一個網站即可。不用每個都做。

# Assignment #5 1018
(如果第一題做不出來就請做第二題就好，但建議你盡量自我嘗試)
1. 爬取自由時報的搜尋結果頁面，請自行下關鍵字，確認該關鍵字有至少1000則以上的新聞回應，並儲存為.pickle檔。
2. 爬取ptt某個版約2000篇文章，並儲存為.pickle檔。
3. 利用學期一開始教的計數、`count()`函式或使用pandas把591租屋網的資料或上述ptt所抓取的資料進行簡單的計數（例如解決最近誰最常po文？幾點po文最多？類似的問題。）
