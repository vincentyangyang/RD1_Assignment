# RD1_-Assignment

經長時間比對  
氣象局的資料很不統一且更新時間也不一致，API中的內容跟網站上的資料也有一些出入  
比如提供雨量的API中沒有“前一小時雨量”的資料，“一週天氣預報”API提供的資料內容也和網站上顯示的不同  
所以有些資料我用API直接抓，有些則是直接用python爬蟲爬回來  
  
檔案‘insertToSql.php’可直接執行getWeek.py檔，抓取一週天氣的網頁資料及detail並放入資料庫  
檔案'getData.php'是抓取未來兩天天氣並放入資料庫  
檔案‘getRain.py‘可寫排程執行，這個檔案是爬雨量資料回來(資料有1000多筆，需要一段時間執行)  
  
檔案'index.php'為主畫面  
使用前請務必先建立資料庫，詳見'sql.txt'
