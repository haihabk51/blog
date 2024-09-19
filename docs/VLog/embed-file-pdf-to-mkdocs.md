---
title: Thêm pdf vào web như nào đây
aliases:
  - Thêm pdf vào web như nào đây
tags:
  - pdf
date: 
share: 
category:
---
Hừm, 
Có cái web rồi lại nghịch nghịch embed cái file pdf xem sao.

Tưởng dễ mà không có thể đơn giản hơn.( hỏi chát GPT lòi ruột nên kiểu gì chả có bạn k biết). Viết cái notes mai ai hỏi có liền hà. 

Bước 1- là bạn up file lên google drive nhé.

Bước 2: lấy cái link share- copy paste sang cửa sổ mới thì ta thấy đuôi của link nhận được có chữ ==view==
-> mình sửa lại thành preview và paste link này vào cấu trúc embeded thôi là xong rồi.

![](https://i.imgur.com/fQeiMwv.png)

Cấu trúc embed như nào?

Thì đây: Thay link vào là xong nhé
![](https://i.imgur.com/Jkn364r.png)

## Để sẵn cái code block sẵn copy thôi nè yêu không 😜

```
<iframe src="https://drive.google.com/file/d/1osXjAxtuNgW-ePlylnPoMJAkR4f09y3h/preview" width="100%" height="800px" frameborder="0"></iframe>
```

## Tương tự với file mp3 trên google drive nhé
![](https://i.imgur.com/62eokTq.png)



<iframe width="100%" height="150" scrolling="no" frameborder="no" allow="autoplay" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/198275799&color=%23ff5500&auto_play=true&hide_related=false&show_comments=true&show_user=true&show_reposts=false&show_teaser=true&visual=true"></iframe><div style="font-size: 10px; color: #cccccc;line-break: anywhere;word-break: normal;overflow: hidden;white-space: nowrap;text-overflow: ellipsis; font-family: Interstate,Lucida Grande,Lucida Sans Unicode,Lucida Sans,Garuda,Verdana,Tahoma,sans-serif;font-weight: 100;"><a href="https://soundcloud.com/alamgir-4" title="Alamgir" target="_blank" style="color: #cccccc; text-decoration: none;">Alamgir</a> · <a href="https://soundcloud.com/alamgir-4/track04" title="Track04" target="_blank" style="color: #cccccc; text-decoration: none;">Track04</a></div>