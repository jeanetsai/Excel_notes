# Excel_notes
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

參考資料: https://www.youtube.com/channel/UCdEpz2A4DzV__4C1x2quKLw
