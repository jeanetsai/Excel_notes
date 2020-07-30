# Excel_notes 教學檔案
IF, COUNTIF, VLOOKUP and other functions, pivot tables

字串記得加雙引號，絕對參照可使用F4作為快捷鍵

IF_FUNCTION
=IF(C7>=60,"STRING P","STRING F") 
巢狀IF(條件,成立,IF(條件,成立,不成立))

VLOOKUP_FUNCTION
=VLOOKUP(關鍵字欄位,資料範圍絕對參照,含有此關鍵字的欄數由第一欄開始, 查詢模式FALSE精準比對TRUE模糊比對)

COUNTIF
=COUNTIF(C2:C14,"電腦")
=COUNTIF(資料範圍, 條件或關鍵字欄位)

COUNTIFS
=COUNTIFS(C2:C14,"電腦",D2:D14.">1000") 用電腦且消費大於1000
=COUNTIFS(資料範圍1, 條件或關鍵字欄位1,資料範圍2, 條件或關鍵字欄位2)

SUMIFS
=SUMIFS(加總範圍,資料範圍1, 條件或關鍵字欄位1,資料範圍2, 條件或關鍵字欄位2)

PIVOTS
插入樞紐分析表，將要看的列和欄打勾或拖曳到列和欄。
如需查看某一業務員業績，則將業務員拖曳至左上報表篩選 (fliters)。
日期1月 2月 3月 ... 等資訊，可以選某一頁右鍵=>群組=>group by 季，則能變成第一季，第二季等
#若原始資料更動，要記得手動重新整理 (或 alt+F5)。
匯入Power BI 前如果不是表格，記得要圈選並"格式化為表格"。
參考資料: https://www.youtube.com/channel/UCdEpz2A4DzV__4C1x2quKLw
針對連續的日期變數，可以按其中一格右鍵=>group群組=>同時選年+季+月=>就會自動分類成年/季/月
=>也可以按天數分，群組=>選擇日=>鍵入天數=14天。
任選幾個欄位=>群組=>就能組成群組。
樞紐分析圖: 
插入=>樞紐分析圖，或點樞紐分析表任一處=>alt+f1。

GOAL SEEK
資料=>假設狀況分析(What if analysis)
=>目標搜尋 GoalSeek

SOLVER 規劃求解
檔案右鍵=>自訂快速存取工具列=>增益集=>規劃求解增益集=>規劃求解=>加入目標儲存格以及條件限制

