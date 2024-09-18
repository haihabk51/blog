---
title: thêm pdf vào web như nào đây
aliases:
  - thêm pdf vào web như nào đây
tags:
  - pdf
date: 
share: 
category:
---
Hừm, 
Có cái web rồi lại nghịch nghịch embed cái file pdf xem sao.
Tưởng dễ mà không có thể đơn giản hơn.


Bước 1- là bạn up file lên google drive nhé.
Bước 2: lấy cái link nhưng chữ cuối cùng của link là chữ view.-> mình sửa lại thành preview và paste vào cấu trúc embeded thôi là xong rồi.
![](https://i.imgur.com/fQeiMwv.png)
Cấu trúc embed như nào?

Thì đây: Thay link vào là xong nhé
![](https://i.imgur.com/Jkn364r.png)

```
<iframe src="https://drive.google.com/file/d/1osXjAxtuNgW-ePlylnPoMJAkR4f09y3h/preview" width="100%" height="800px" frameborder="0"></iframe>
```