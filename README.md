# Excel_notes 教學檔案
IF, COUNTIF, VLOOKUP and other functions

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
#若原始資料更動，要記得手動重新整理 (或 alt+F5)

參考資料: https://www.youtube.com/channel/UCdEpz2A4DzV__4C1x2quKLw
