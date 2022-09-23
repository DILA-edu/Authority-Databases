
==================
經錄 JSON 欄位說明
==================

* `authorityID：經錄資料庫規範碼`
   * `Data type：String`
* `vol：冊號`
   * `Data type：String`
   * `有可能跨冊，例如 A097..A098`
* `type`
   * `Data type：String`
   * `textbody：本文`
   * `non-textbody: 非本文，例如佛典編號 TXa001 編纂說明 不是佛典本文
* `orig_category：原書分類`
   * `Data type：String`
   * `例如 T0001 大正藏 原書分類為：阿含部`
* `category：部類`
   * `Data type：String`
   * `可能多值，例如："寶積部類,淨土宗部類"`
* `title：經名`
   * `Data type：String`
* `alt：替代典籍`
   * `Data type：String`
   * `與其他典籍全部或部分重複，CBETA 未重複收錄`
   * `例如 B0083 的 alt 欄位為：JB118`
* `juans：卷數`
   * `Data type：Integer`
* `cjk_chars：中文字數`
   * `Data type：Integer`
   * `字數統計規則 <https://docs.google.com/document/u/1/d/e/2PACX-1vSi7xmhAfkLRvduqzW5S6PXfmaz0abUVnZ-sLUfdP3STFEnLpl1nrJOrFkNIVpYhRdC_TG_3UWL-D-4/pub>`_
* `en_words：英數字數`
   * `Data type：Integer`
   * `字數統計規則 <https://docs.google.com/document/u/1/d/e/2PACX-1vSi7xmhAfkLRvduqzW5S6PXfmaz0abUVnZ-sLUfdP3STFEnLpl1nrJOrFkNIVpYhRdC_TG_3UWL-D-4/pub>`_
* `byline：作譯者行`
   * `Data type：String`
* `dynasty：朝代`
   * `Data type：String`
   * `如果 byline 有多個朝代，dynasty 欄位只記錄年代最晚的`
   * `把這個作品認為是後人將前人的作品，作了一次的確認與編修，所產生的符合當代人理解的作品`
   * `前人的朝代，把它們認為是底本參考來源資訊，而不必影響該文獻的朝代紀錄`
* `time_from, time_to：成書年代`
   * `Data type：Integer`
   * `如果不清楚具體年代，採用朝代的起迄年`
   * `如果《法寶總目錄》有較具體的年代，就採用`
   * `有可能只有 time_from, 沒有 time_to`
* `contributors：貢獻者`
   * `Data type：Array`
   * `name：貢獻者姓名`
   * `id：貢獻者 Authority ID`
* `places：翻譯地點`
   * `Data type：Array`
   * `name：翻譯地點之地名`
   * `id：地名 Authority ID`
   
Maintainer
==========

Winxd Lee winxd@dila.edu.tw


