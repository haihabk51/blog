---
tags:
  - excel
  - tip
aliases: 
cssclasses: 
DATE: 2024-08-27
---

 [Tham khảo nguồn link gốc](https://www.exceldemy.com/excel-vba-translate-formulalanguage/)

## Bước 1 - Mở cửa sổ VBA Nhấn ALT + F11 Cửa sổ visual Basic Editor hiện ra Hình ảnh minh họa:
## Bước 2: Copy Code của VBA vào và sử dụng thôi.
![](https://i.imgur.com/Z0QeLOw.png)
```
Function translate_text$(text_str$, src_lang$, trgt_lang$) 
    Dim s1&, s2&, url_str$, rsp$ 
    Const rslt_div$ = "<div class=""result-container"">" 
    Const url_temp_src$ = "https://translate.google.com/m?hl=[from]&sl=[from]&tl=[to]&ie=UTF-8&prev=_m&q="
    url_str = url_temp_src & WorksheetFunction.EncodeURL(text_str) 
    url_str = Replace(url_str, "[to]", trgt_lang) 
    url_str = Replace(url_str, "[from]", src_lang) 
    rsp = WorksheetFunction.WebService(url_str) 
    s1 = InStr(rsp, rslt_div) 
    If s1 Then 
        s1 = s1 + Len(rslt_div) 
        s2 = InStr(s1, rsp, "</div>") 
        translate_text = Mid$(rsp, s1, s2 - s1) 
    End If 
End Function
```
Sau đó save lại
![](https://i.imgur.com/eVg66cb.png)
Bây giờ thực hiện translate thôi. Chú thích một chút cho ai đó. 
Cột 1: Nội dung cần dịch 
Cột số 2 là MÃ ngôn ngữ nguồn. 
Cột số 3 là MÃ ngôn ngữ đích 
Cột số 4 ta gõ hàm =translate_text()
![](https://i.imgur.com/akZzaQy.png)
![](https://i.imgur.com/WfqjMT0.png)

