---
layout: post
title:  "Thứ tự và ánh xạ, các ánh xạ đặc biệt"
subtitle: "Các khái niệm khác về ánh xạ"
date:   2018-02-10
categories: [dai-so]
permalink:
cover:
description:
mathjax: true


---

# Mục tiêu

- ### Tính đơn điệu
- ### Thứ tự giữa các ánh xạ
- ### Các ánh xạ đặc biệt

Bài viết này tụi mình sẽ cùng tìm hiểu về các khái niệm khác về ánh xạ. Cái khái niệm này cần thiết khi tụi mình chứng minh các khái niệm liên quan đến ánh xạ. Các khái niệm này rất dễ quên, nên tách ra với phần bài viết về ánh xạ để các bạn chú ý hơn và sau này nhỡ quên có thể dễ quay lại tìm.<br/>
<br/>

# Tính đơn điệu
Cho $$(E,\preceq),(F,\preceq')$$ là hai tập hợp được sắp thứ tự.<br/>
## Ánh xạ tăng
> Ánh xạ $$f: E \rightarrow F $$ là ánh xạ tăng khi và chỉ khi: $$\forall (x, x') \in E^2, x \preceq x' \Rightarrow f(x) \preceq' f(x')$$

## Ánh xạ giảm
> Ánh xạ $$f: E \rightarrow F $$ là ánh xạ giảm khi và chỉ khi: $$\forall (x, x') \in E^2, x \preceq x' \Rightarrow f(x') \preceq' f(x)$$

## Ánh xạ đơn điệu
> Ánh xạ $$f: E \rightarrow F $$ là ánh xạ đơn điệu khi và chỉ khi: $$f$$ là ánh xạ tăng hoặc $$f$$ là ánh xạ giảm.


Điều này thì chắc các bạn đã nắm được nó, mình chỉ xin chú ý lại với các bạn những gì mình nói ở bài viết trước, tụi mình đã biết là ánh xạ là một quan hệ có tính đơn trị (mỗi phần tử ở nguồn chỉ có duy nhất một ảnh) và mình cũng đã các bạn "cách làm việc" của ánh xạ, đó là ở ánh xạ tụi mình quan tâm hơn ở việc khi tụi mình thay đổi từ phần tử này sang phần tử khác ở tập nguồn thì sẽ sự thay đổi như thế nào ở các phần tử thuộc tập đích, ở đây phần tử ở tập đích có thể "tăng", "gỉảm" hoặc không đổi. Tại sao mình đặt tăng, giảm ở trong " ", bởi vì quan hệ thứ tự ở đây có thể không giống như quan hệ thứ tự thông thường. Và từ đó tụi mình có thể tưởng tượng ánh xạ như cái "máy tính", có "đầu vào" là các phần tử ở tập nguồn, cho ra "kết quả" là các phần tử ở tập đích, sự thay đổi đầu vào dẫn đến sự thay đổi kết quả.

**Ví dụ**
- Ánh xạ $$f: \underset{x \rightarrow \lvert x \rvert}{(0,1) \rightarrow (0,1)}$$ là ánh xạ tăng, ánh xạ $$f: \underset{x \rightarrow \lvert x \rvert}{(-1,0) \rightarrow (0,1)}$$ là ánh xạ giảm theo quan hệ thứ tự thông thường.<br/>
Đồ thị của hai ánh xạ trên có thể vẽ như sau.

<center><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="400px" version="1.1" content="&lt;mxfile userAgent=&quot;Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36&quot; version=&quot;8.0.9&quot; editor=&quot;www.draw.io&quot; type=&quot;google&quot;&gt;&lt;diagram id=&quot;ca0bd605-04d8-a2e4-8210-f4e2b498fed7&quot; name=&quot;Page-1&quot;&gt;7VfLjpswFP0alpUwDoRZzjDTdlO1UhZtlw6+gDUGI+O8+vU1YPNMMslomlaaZhHZx/Y1nHPutXFwlO8/SVJmXwQF7ngu3Tv40fG8wPf1fw0cWgDfhS2QSkZbCPXAiv0CA7oG3TAK1WiiEoIrVo7BWBQFxGqEESnFbjwtEXy8a0lSmAGrmPA5+p1RlbVo6Ls9/hlYmtmdkWtG1iR+TqXYFGa/QhTQjuTEhjFTq4xQsRtA+MnBkRRCta18HwGvWbWMtes+nhjtHllCoS5Z4EGyQMvYW3vLeJ3Quw8mwpbwjaHBPKg6WF6goPc1vboXc1JVLHbwQ6ZyrgGkm5WS4hkiwYVsFmC3+XUjlsx6biIKZZTH9Yx2M6AzZfoXQh1N2nggclDyoKfseomsQtlAHYtJ4ESx7Tg8MU5Ju3DdDt8E0xt7rjW1CWMtbXW0ESqxkTGYRUPeZ3FeCKSITEHNAunG4K17qJH1Qom9/xKfkxhPNPZfq/E0UHg7ifEFEnOuC6nuPOwypmBVkrge2elSPtaaVGVbXRO2B3pW/IRxfhSfWIBwlha1t7TiIDtPbEEq2F/rCsu2PW5sRiHTH7gGHXENck8bZCTJNfz7749/H/1D/AdXlbjmfH6pvgVBFM3qGz5CruZLHn6YQE3np+5cU/n0PacpDeeS+29Vx64aGplR8MrqiCYnoO/frjwuZ/b4OvOHzgR1zhTGNMOUM9Asu+q8YvpeeW8GckYpP5X5zb2xzvPHSeZ67hsVyomC2AoxMNDiiIGWfyJRw5kS6P0osQj9Wymhu/1HRZtC/TcbfvoN&lt;/diagram&gt;&lt;/mxfile&gt;" onclick="(function(svg){var src=window.event.target||window.event.srcElement;while (src!=null&amp;&amp;src.nodeName.toLowerCase()!='a'){src=src.parentNode;}if(src==null){if(svg.wnd!=null&amp;&amp;!svg.wnd.closed){svg.wnd.focus();}else{var r=function(evt){if(evt.data=='ready'&amp;&amp;evt.source==svg.wnd){svg.wnd.postMessage(decodeURIComponent(svg.getAttribute('content')),'*');window.removeEventListener('message',r);}};window.addEventListener('message',r);svg.wnd=window.open('https://www.draw.io/?client=1&amp;lightbox=1&amp;edit=_blank');}}})(this);" viewBox="0 0 556 456" style="cursor:pointer;max-width:100%;max-height:456px;"><defs/><g transform="translate(0.5,0.5)"><path d="M 7 247 L 540.63 247" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 545.88 247 L 538.88 250.5 L 540.63 247 L 538.88 243.5 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 307 447 L 307 13.37" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 307 8.12 L 310.5 15.12 L 307 13.37 L 303.5 15.12 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><ellipse cx="307" cy="247" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="467" cy="247" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 467 87 L 310.62 243.48" fill="none" stroke="#0066cc" stroke-width="3" stroke-miterlimit="10" pointer-events="none"/><g transform="translate(278.5,250.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="16" height="22" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 20px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 16px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">O</div></div></foreignObject><text x="8" y="21" fill="#000000" text-anchor="middle" font-size="20px" font-family="Helvetica">O</text></switch></g><g transform="translate(445.5,250.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="12" height="22" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 20px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 12px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">1</div></div></foreignObject><text x="6" y="21" fill="#000000" text-anchor="middle" font-size="20px" font-family="Helvetica">1</text></switch></g></g></svg></center>


<center><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="400px" version="1.1" content="&lt;mxfile userAgent=&quot;Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36&quot; version=&quot;8.0.9&quot; editor=&quot;www.draw.io&quot; type=&quot;google&quot;&gt;&lt;diagram id=&quot;ca0bd605-04d8-a2e4-8210-f4e2b498fed7&quot; name=&quot;Page-1&quot;&gt;7VdNj5swEP01HCthO5DkuMtu20vVSjm0PXrxANYaHBnnq7++Bmw+k2yy2qaVtjlEzLM9hvfeDMYjUb7/pOg6+yIZCA/7bO+RBw/jMAjMfwUcGoAsFw2QKs4aCHXAiv8CC/oW3XAG5WCillJovh6CsSwKiPUAo0rJ3XBaIsVw1zVNYQKsYiqm6HfOdNagi8Dv8M/A08ztjHw78kTj51TJTWH3K2QBzUhOXRo7tcwok7seRB49EikpdXOV7yMQFauOsWbdxxOj7S0rKPQlCzAkMzSP8ROex08JW36wGbZUbCwN9kb1wfECBbur6DVRLGhZ8tgj95nOhQGQuSy1ks8QSSFVvYD49a8dcWRWcxNZaKs8qWY0mwGbKNM9EGppMsYDmYNWBzNl10nkFMp66jhMgaCab4fpqXVK2qZrd/gmudkY+87UNo2ztNPRZSjlRsVgF/V5n+R5IZGmKgU9SWQuek/dQbWsF0qM/0t8TmIy0jh4rcbjRIvbSUwukFgI00hNcL/LuIbVmsbVyM608qHWtFw33TXhe2BnxU+4EEfxkQWo4GlRecsoDqr1xBaUhv21rnBsu9eNqyhk455r0BHXIP+0QQaSXMN/8P74R8vZv8N/eFWLq9/PL/W3MIyiSX8jR8g1fKnDDxO1wU8bXNr5zDmnbg3nivtvdUc8enGh8JXdEY0SBcHt2uN8Yo+vE3+YStDnTGFN0y85C02qq6orbs6Vd3Yg54yJU5VfnxurOn8YVS7236hR4tHRwwnRM9DsiIHmf6JQFxMl3An0PUiBwtmtpDBh91XR1FD30UYefwM=&lt;/diagram&gt;&lt;/mxfile&gt;" onclick="(function(svg){var src=window.event.target||window.event.srcElement;while (src!=null&amp;&amp;src.nodeName.toLowerCase()!='a'){src=src.parentNode;}if(src==null){if(svg.wnd!=null&amp;&amp;!svg.wnd.closed){svg.wnd.focus();}else{var r=function(evt){if(evt.data=='ready'&amp;&amp;evt.source==svg.wnd){svg.wnd.postMessage(decodeURIComponent(svg.getAttribute('content')),'*');window.removeEventListener('message',r);}};window.addEventListener('message',r);svg.wnd=window.open('https://www.draw.io/?client=1&amp;lightbox=1&amp;edit=_blank');}}})(this);" viewBox="0 0 556 456" style="cursor:pointer;max-width:100%;max-height:456px;"><defs/><g transform="translate(0.5,0.5)"><path d="M 7 247 L 540.63 247" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 545.88 247 L 538.88 250.5 L 540.63 247 L 538.88 243.5 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 307 447 L 307 13.37" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 307 8.12 L 310.5 15.12 L 307 13.37 L 303.5 15.12 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><ellipse cx="307" cy="247" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="146" cy="247" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 147 87 L 303.72 243.48" fill="none" stroke="#0066cc" stroke-width="3" stroke-miterlimit="10" pointer-events="none"/><g transform="translate(278.5,250.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="16" height="22" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 20px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 16px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">O</div></div></foreignObject><text x="8" y="21" fill="#000000" text-anchor="middle" font-size="20px" font-family="Helvetica">O</text></switch></g><g transform="translate(121.5,250.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="18" height="22" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 20px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 18px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">-1</div></div></foreignObject><text x="9" y="21" fill="#000000" text-anchor="middle" font-size="20px" font-family="Helvetica">-1</text></switch></g></g></svg></center>

<br/>
<br/>

# Thứ tự giữa các ánh xạ

E là một tập hợp, $$(F,\preceq)$$ là một tập hợp được sắp thứ tự. Trên $$F^X$$ có một quan hệ thứ tự $$\preceq'$$ được đĩnh nghĩa như sau:
> ## $$f \preceq' g \Leftrightarrow (\forall x \in X,  f(x) \preceq g(x))$$

Tụi mình có thể nói là: ánh xạ $$f$$ "nhỏ hơn" ánh xạ $$g$$ khi và chỉ khi tại mọi $$x$$, $$f(x)$$ "nhỏ hơn" $$g(x)$$.<br/>
<br/>

**Chú ý**

- Như ở bài viết trước tụi mình đã có định nghĩa về hai ánh xạ bằng nhau $$f$$ và $$g$$ phải có chung tập nguồn, tập đích và giả sử tập nguồn là $$E$$ thì $$\forall x \in E, f(x) = g(x))$$. Và tương tự để có quan hệ thứ tự giữa $$f$$ và $$g$$ thì $$f$$ và $$g$$ phải thuộc $$F^E$$ điều này có là $$f$$ và $$g$$ có chung tập nguồn là $$E$$ và tập đích là $$F$$.

- Đây cũng chính là ví dụ cho tụi mình thấy tụi mình không chỉ có thứ tự giữa các số mà còn có thứ tự giữa những thứ khác.

- Thứ tự giữa các ánh xạ có thể là toàn phần hoặc không toàn phần phụ thuộc vào quan hệ thứ tự trong $$F$$.<br/>
Ví dụ<br/>
  - Đối với quan hệ thứ tự thông thường thì ánh xạ $$f: \underset{x \rightarrow x}{(0,1) \rightarrow (0,1)}$$ và ánh xạ $$g: \underset{x \rightarrow 1-x}{(0,1) \rightarrow (0,1)}$$ không so sánh được. Vậy trong trường hợp này thì quan hệ thứ tự giữa các ánh xạ là quan hệ không toàn phần. <br/>
  - Cũng với hai ánh xạ $$f,g$$ như trên. Nếu tụi mình định nghĩa một quan hệ thứ tự $$\preceq'$$ trên $$F$$ như $$f(x) \preceq' g(x) \Leftrightarrow Max(f) \leq Max(g)$$. Với $$Max(f)$$ là phần tử lớn nhất theo thứ tự thông thường trên tập đích của $$f$$, tương tự với $Max(g)$, quan hệ thứ tự giữa thứ tự giữa $$Max(f)$$ và $$Max(g)$$ là quan hệ thứ tự thông thường (quan hệ thứ tự thông thường là quan hệ thứ tự giữa các số). Như vậy, $$Max(f) = 1, Max(g) = 1$$, nên hai ánh xạ này bằng nhau. Nếu tụi mình có thêm ánh xạ $$h: \underset{x \rightarrow 2x}{(0,1) \rightarrow (0,1)}$$ thì $$Max(h) = 2$$, nên suy ra $$ f < h$$. Và tụi mình có hình biểu diễn là:<br/>

  <center><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="400px" version="1.1" content="&lt;mxfile userAgent=&quot;Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36&quot; version=&quot;8.0.9&quot; editor=&quot;www.draw.io&quot;&gt;&lt;diagram id=&quot;ce097fa3-9f2c-2cf3-520c-73d41972da54&quot; name=&quot;Page-1&quot;&gt;7ZpLc9owEMc/DcfOWJZ5+JiQ0l467UwOPau2sDUxFpVFgH76SlgC60HIQ2ZagENiVtJfZn+7YiUzgNPF5gtDy/IbzXE1iKN8M4APgzhOh5H4Kw3b1jAcj1tDwUjemsDB8Ej+YGVU44oVyXFjdOSUVpwsTWNG6xpn3LAhxuja7DanlTnrEhXYMTxmqHKtP0nOy9Y60R9L2r9iUpR6ZhCpll8oeyoYXdVqvkEM57tX27xAWkv1b0qU03XHBD8P4JRRyturxWaKK+la7bZ23OxI6/6+Ga75awbE7YBnVK2wvuPdffGt9gWu8zvpUvEuq1DTkGwA70u+qIQBiMuGM/qEp7SibDcARrvXvkU7UPad05or2lD2aCfDuUPjcP9g7xURbJguMGdb0WV9wKKplB0i2sZwhTh5NuWRio5iL7ef4QclYuI4UoEcJ0pHx3ECTYmGrliG1aiuny2h4SkhjliBuSMkLjof+2DaYfQjhTekZ0FqC4GoN6TJm5DWtMYneM5mULxuPLtCiSUE+0vRYWieUZRM0/QieNoYguVnjzxHoXkmD2l6W29fDgzQH8+Jh+eo4sr7BtjR7xXVDZ+aHZc70UEA2BwaxVUh/2+0jLiBVqm1O9HC8Ya/FCIqhOakqiwTqkhRy+91QR8L+/0zZpyIyvZONSxInstp7tcl4fhxiTI551qU8cK2q1yx9EJ0NNSkIN68Ndh0HQTsaFC+7gRj4glGXS/74s4A/QLVtCeq36+eKkhH/hw/A1UdUB6szRLV78e67WBtla4NaxyZyZqekapvYxoiWcHVJ2uid4j7ZB2fD6tvc3rDGiZZh2a5C91shX1h9W1QQ2CNrx4rSE2swIO1t2z1VUwf3KdezDlSkgB/Jfv2fY0lBC2hcPua2Fcr3YAq5yTWAvrugwd4QiggUHADehyoxcE5MHj9SdIJoSNAhdvRttNtKTs0H0Xuq4w/hHw2uxjkw8nEIBXbZ/KvRT6yDpscoYA57J4ezh2i/1x9Eweqb0aJSQyccZMZjx3PF/+J53PCcMYJlTIipqWngtAYWvkDXBqxh0YSgAbsoTi5mKcizsIGQy1stlDAB9HBi5MLeiziAB0lgYDaQgGBuqVHeVsvDed7Dr4DrZfi7eFnQS28w0+v4Oe/&lt;/diagram&gt;&lt;/mxfile&gt;" onclick="(function(svg){var src=window.event.target||window.event.srcElement;while (src!=null&amp;&amp;src.nodeName.toLowerCase()!='a'){src=src.parentNode;}if(src==null){if(svg.wnd!=null&amp;&amp;!svg.wnd.closed){svg.wnd.focus();}else{var r=function(evt){if(evt.data=='ready'&amp;&amp;evt.source==svg.wnd){svg.wnd.postMessage(decodeURIComponent(svg.getAttribute('content')),'*');window.removeEventListener('message',r);}};window.addEventListener('message',r);svg.wnd=window.open('https://www.draw.io/?client=1&amp;lightbox=1&amp;edit=_blank');}}})(this);" viewBox="0 0 494 489" style="cursor:pointer;max-width:100%;max-height:489px;"><defs/><g transform="translate(0.5,0.5)"><path d="M 45 457 L 338.63 457" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 343.88 457 L 336.88 460.5 L 338.63 457 L 336.88 453.5 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 45 457 L 45 23.37" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 45 18.12 L 48.5 25.12 L 45 23.37 L 41.5 25.12 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 45 457 L 245 257" fill="none" stroke="#ff3333" stroke-miterlimit="10" pointer-events="none"/><path d="M 245 457 L 45 257" fill="none" stroke="#004c99" stroke-miterlimit="10" pointer-events="none"/><path d="M 45 457 L 245 57" fill="none" stroke="#4d9900" stroke-miterlimit="10" pointer-events="none"/><g transform="translate(329.5,454.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="10" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 11px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;"><font style="font-size: 20px">x</font></div></div></foreignObject><text x="5" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">[Not supported by viewer]</text></switch></g><g transform="translate(12.5,449.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="16" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 16px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;"><font style="font-size: 20px">O</font></div></div></foreignObject><text x="8" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">[Not supported by viewer]</text></switch></g><g transform="translate(19.5,-0.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="10" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 11px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;"><span style="font-size: 20px">y</span></div></div></foreignObject><text x="5" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">[Not supported by viewer]</text></switch></g><g transform="translate(241.5,453.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="12" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 12px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;"><font style="font-size: 20px">1</font></div></div></foreignObject><text x="6" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">[Not supported by viewer]</text></switch></g><g transform="translate(18.5,239.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="12" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 12px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;"><font style="font-size: 20px">1</font></div></div></foreignObject><text x="6" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">[Not supported by viewer]</text></switch></g><g transform="translate(13.5,39.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="12" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 12px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;"><font style="font-size: 20px">2</font></div></div></foreignObject><text x="6" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">[Not supported by viewer]</text></switch></g><path d="M 246 462 L 246 452" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 50 257 L 40 257" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 40 57 L 50 57" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 393 117 L 445 117" fill="none" stroke="#ff0000" stroke-miterlimit="10" pointer-events="none"/><g transform="translate(469.5,105.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="6" height="22" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 20px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 6px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">f</div></div></foreignObject><text x="3" y="21" fill="#000000" text-anchor="middle" font-size="20px" font-family="Helvetica">f</text></switch></g><g transform="translate(466.5,135.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="12" height="22" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 20px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 12px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">g</div></div></foreignObject><text x="6" y="21" fill="#000000" text-anchor="middle" font-size="20px" font-family="Helvetica">g</text></switch></g><path d="M 393 147 L 445 147" fill="none" stroke="#004c99" stroke-miterlimit="10" pointer-events="none"/><path d="M 393 178 L 445 178" fill="none" stroke="#4d9900" stroke-miterlimit="10" pointer-events="none"/><g transform="translate(466.5,165.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="12" height="22" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 20px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 12px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">h</div></div></foreignObject><text x="6" y="21" fill="#000000" text-anchor="middle" font-size="20px" font-family="Helvetica">h</text></switch></g></g></svg></center>

**Ví dụ**
- Đối với thứ tự thông thường, nếu ánh xạ $$f:\underset{x \rightarrow x^2}{(0,1) \rightarrow (0,1)}$$ và ánh xạ $$g:\underset{x \rightarrow x}{(0,1) \rightarrow (0,1)}$$ thì $$f \leq g$$.

<center><svg version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px" width="400px" height="300px" viewBox="0 0 800 600" enable-background="new 0 0 800 600" xml:space="preserve">  <image id="image0" width="800" height="600" x="0" y="0"
    xlink:href="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAyAAAAJYCAYAAACadoJwAAAABGdBTUEAALGPC/xhBQAAACBjSFJN
AAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAABmJLR0QA/wD/AP+gvaeTAAAA
CXBIWXMAAA9hAAAPYQGoP6dpAABT+0lEQVR42u3de5xXVb3/8dfmIgoYFhmKKZVkdOpwlEso6MTB
C9hFLAVCkcKCjJK0JD2VuQxT0VAR84qKR5RU1E6UaVc8XbSgkm6nspudxKOWiTdUlPX7Y33n5zjM
DHP7zvpeXs/H4/sY2DN7eO/ZA+zPrLU+CyRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJ
kiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJ
kiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJ
kiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJ
kiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJ6h4DgDOBO4HHgK3A+ztw/i7A
lcCjwFPAd4H9cl+UJEmSpMr0OlLR8WdS8bAVmN3Oc3sBPwSeBE4H5gO/AjYBw3NfmCRJkqTKswPw
mtKvR9OxAmR66ePf2+TYq0kjKTfkvjBJkiRJlW0MHStAbgY2tnD8ctJ0rL65L0iSJEnqab1yB6hh
+wE/a+H4OqA/sE/ugJIkSVJPswApn92Bh1o43nhsaO6AkiRJUk+zACmfHYHnWjj+bOntTrkDSpIk
ST2tT+4ANWwz0K+F4zs2eX9Ldi+9JEmSVJkeouWZLmoHC5DyeYiWp1k1FhcbW3nfOmCP3OElSZLU
qgeBsViEdIoFSPncBxwEFEBscnwc8DTw+xbO2Z1UfBwL/Db3BahHXAicnDuEeoz3u754v+uL97t+
jCBtqdDael9thwVI99iNtOv5H4AXSsdWA0eT9gG5tXTs1cA0YA2wpY3P91ta7qCl2rMJ73U98X7X
F+93ffF+S+1kAbJ9HyMVF43TqY4A9ir9+mLgCeBc0v4grwP+WnrfauBe4FrgX4B/kHZDL4Azcl+U
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
NNWi+cPEuNLb+9o49z5gFNsuUBxHeij9fe6L0za6cr8BBpOKj76kB1QXJle2zt7vvUpvbwP+1OQ1
lFSc/Jm0Z4QqS1f+fq8n/Vv+2mbHGx9aHs19cdpGV+53H1oe5ejb5P2qHffh85oqTGMf8U82OdbY
R/xHTY7tRpp20/Qfpca+0kc1OfZq0k/Gb8x9YWpRV+73AODHpNaN7p5aHTp7v/cEjmj2mkoqOH9c
+v0bcl+cttGVv99TS+ee1eRYL+D7pOLDNp2Vpyv3+/ukLmevanKsN6kQfRynYFW6ttrw+rymqnET
L+2kOo807/s5Xr7x3ArSN+9eTY71Iv0j9wQv31nzcVJHFVWmzt7vr5SOLQdmNXtNzX1RalVn73dL
/oL7gFS6rtzvb5F2Qr+c9O/5N0sf5zqvytXZ+z2FdK/vJy1CP5H0//lW4D9yX5Ra9TFSZ7pLSfdq
den3nwVeUfqYFfi8pirRj7Sh0UbSQqR7gUObfcy1pH+smv+HtQtph+RHSR1Svksa5lPl6uz9/nPp
2NYWXn/KfVFqVVf+fjfnTuiVryv3ewCp5fJGUnec+4CZuS9IberK/Z4M/Dfp/+7G+z039wWpTX/m
pf93X+Sl/5Ob3l+f1yRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJ
kiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJ
kiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJ
kiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkirI/wPlNWmtuCWslAAAACV0RVh0ZGF0ZTpjcmVh
dGUAMjAxOC0wMi0wOVQwNDoyMToxNS0wNzowMMj+PRQAAAAldEVYdGRhdGU6bW9kaWZ5ADIwMTgt
MDItMDlUMDQ6MjE6MTUtMDc6MDC5o4WoAAAAAElFTkSuQmCC" />
</svg> </center>

- Đối với thứ tự thông thường, nếu ánh xạ $$f:\underset{x \rightarrow x^2}{(1,2) \rightarrow (1,4)}$$ và ánh xạ $$g:\underset{x \rightarrow x}{(1,2) \rightarrow (1,4)}$$ thì $$g \leq f$$.
<br/>
<center><svg version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px" width="400px" height="300px" viewBox="0 0 800 600" enable-background="new 0 0 800 600" xml:space="preserve">  <image id="image0" width="800" height="600" x="0" y="0"
    xlink:href="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAyAAAAJYCAYAAACadoJwAAAABGdBTUEAALGPC/xhBQAAACBjSFJN
AAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAABmJLR0QA/wD/AP+gvaeTAAAA
CXBIWXMAAA9hAAAPYQGoP6dpAABI3UlEQVR42u3debid093/8fdKZBRiSBCKVNEoqoIaYoh5iiSG
KjX3qSot2npUqeGuzu2jrempolUtpeYkxDyTmutRSg31o8QsDYlIJFm/P9aOcxxn3meftYf367rO
deQ+e59879zbOeuz77XWFyRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJ
kiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJ
kiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJ
kiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJ
kiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJqozvAQuBv3fy8UsB5wJvALOA24D1c5+EJEmS
pOr3CWA28C7wWCce3we4t/T4k4AjgMeBmcDquU9GkiRJUnW7FLgZuJ3O3QHZm3S3ZI9mx4YBbwMX
5z4ZSZIkSdVrS+ADYG3gDjp3B+QyYHorx88hTcfql/ukJEmSpN7WJ3cBNaAvcCZwHvBEF563PvBI
K8cfBAYDa+Y+MUmSJKm3GUA69jVgFdI6jq4YAbzSyvFFx1bMfWKSJElSbzOAtG9Z4NTSx1tdfO5A
YG4rx98vfR6U++QkSZKk3rZY7gKq3A+BN0lTsLpqDjCgleMDm329NSNKH5IkSapOr9D6TBd1ggGk
bWsAhwLfJG3Bu8hAoD+wKvAOMKON579C69OsFoWL6W187UFgpdwnL0mSpDa9DGyEIaRbDCBtW4k0
Re2M0kdLzwO/Br7dxvMfBbYAAhCbHd+Y1E/k6VaeM6L09+4HPJX7H0Af8yvgW7mLUJu8PtXLa1O9
vDbVzetTnUaRWiq0td5XHTCAtO3vwO58NDwE0rSsIcDRwHOl4yOAocCzwPzSsSuAvUh9QK4sHRsG
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
zcrA+BYfE0jh8P7Sn1fLfUJ1pqv/70woPf6HzY71If0+egO3E+1JXb02jgkqqy9pHc1c0p2Ptjge
6AGm5cp7ALictEXecsBzwEGkdwKbv9P3U9IPoZHAi6VjPyLNQbyftMPF+8C+pJT9PZzr2VO+QWrs
tOgdvvE0vVN7BmkbytauzxXAfcAFpH4Gb5G6nwbSgmeVr7vX5mJgI9JOPmvz0S627+JizZ7QnWvz
79JHS6eTQojNCHtOd//fmQTcChxPGkA9BkwExpA6ortxQPm6e20cE1TWacBupDsgw4D9W3z9otJn
xwOqGQOAn5PmAM4hvUi3b/GYC0g/PFZpcXxH4C7SriPvk27zHZr7hOrM86R3LhaSrsGCZv+96Hq0
dX2WInVyfoN0jW4j/TJQz+jutXm+2WNbfvwr90nViXL+v2ntexk+elY512dx0hbJ02n6vbNv7hOq
I+VcG8cElXM7bf/eaB7uHA9IkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJ
kiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJ
kiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJ
kiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRJkiRVkf8PZ/zyHIoJqroAAAAldEVYdGRhdGU6
Y3JlYXRlADIwMTgtMDItMDlUMDQ6Mjk6NDMtMDc6MDDwGUa+AAAAJXRFWHRkYXRlOm1vZGlmeQAy
MDE4LTAyLTA5VDA0OjI5OjQzLTA3OjAwgUT+AgAAAABJRU5ErkJggg==" />
</svg></center>
<br/>
- Đối với thứ tự thông thường, nếu ánh xạ $$f:\underset{x \rightarrow x^2}{(0,2) \rightarrow (0,4)}$$ và ánh xạ $$g:\underset{x \rightarrow x}{(0,2) \rightarrow (0,4)}$$ thì $$f$$ và $$g$$ không so sánh được.

<center><svg version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px" width="400px" height="300px" viewBox="0 0 800 600" enable-background="new 0 0 800 600" xml:space="preserve">  <image id="image0" width="800" height="600" x="0" y="0"
    xlink:href="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAyAAAAJYCAYAAACadoJwAAAABGdBTUEAALGPC/xhBQAAACBjSFJN
AAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAABmJLR0QA/wD/AP+gvaeTAAAA
CXBIWXMAAA9hAAAPYQGoP6dpAABPIUlEQVR42u3de7hVVb3/8fcEDERFIy3QNI6ResrjSSmpyCxL
M0VLQUhAhMwyNTXt4jHNWVpWVmpqmYqgiCYZZmRG9YtOpVgmcbp4KOWQRphGIqKgCIzfH9+FbnDf
b2Nd3q/nWc+mtddcfOduupifPcb4DpAkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIk
SZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIk
SZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIk
SZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIk
SZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkqWd8GtgI/KGdr98BuBr4J/AU8DNg
39wnIUmSJKn6vRJ4GlgN/L4dr+8D3FV5/XnAycAfgVXA8NwnI0mSJKm6fRv4CTCf9o2AjCNGS45u
8tyOwOPArNwnI0mSJKl6vQ14Dngd8HPaNwIyG1jezPNXEdOxtsp9UpIkSVJv65O7gBrQF7gcuAb4
UweO2xdY2Mzz9wIDgT1yn5gkSZLU2wwgbTsJ2I1Yx9ERQ4FHmnl+03M75z4xSZIkqbcZQFr3MuBz
lce/OnjsAODZZp5/pvJ169wnJ0mSJPW2frkLqHIXAiuIKVgdtRbo38zzA5p8vzlDKw9JkiRVp0do
fqaL2sEA0rLXACcCZxAteDcZALwEeBXwJLCyheMfoflpVpvCxfIWvncvsEvuk5ckSVKL/g68EUNI
pxhAWrYLMUXt65XHlpYClwJntnD8IuAAoABSk+dHEvuJ/KWZY4ZW/t6JwOLcPwDVvUuAj+UuQg3B
a029xWtNvWEvYkuFltb7qg0GkJb9ATiKzcNDQUzL2hY4HVhSeX4osD3wILC+8tytwFhiH5DvVp7b
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
af4fcelU4FzgG8T1dGvlf59LTF0AP9fUPTp7rfm5po64lLiGbgcmNfPYZAZ+rqlG9Cfa/y0nFiLd
Axy8xWumAxvY/IIG2AG4hhgufgr4Ge7qqpZ19lq7gOhhvpIILEuBK/AfabVsKfGP8EbietrQ5M+b
ri0/19QdOnut+bmmjpjPC9fWlo8NTV7n55okSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIk
SZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIk
SZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIk
SZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSZIkSVIV+f940qRxjYtcPAAAACV0
RVh0ZGF0ZTpjcmVhdGUAMjAxOC0wMi0wOVQwNDozOToyMC0wNzowMMYQimQAAAAldEVYdGRhdGU6
bW9kaWZ5ADIwMTgtMDItMDlUMDQ6Mzk6MjAtMDc6MDC3TTLYAAAAAElFTkSuQmCC" />
</svg></center>
<br/>
<br/>

# Các ánh xạ đặc biệt
## Thác triển và thu hẹp của ánh xạ <br/>
Thực ra đây không phải là ánh xạ đặc biệt vì chỉ là hai cách để xác định ánh xạ. Mình đặt thác triển và thu hẹp của ánh xạ vào phần này để muốn nói là thác triển và thu hẹp của ánh xạ vẫn là ánh xạ.<br/>

### Thác triển của ánh xạ

Cho $$E,F,E'$$ là tập hợp, ánh xạ $$f: E \rightarrow F$$. $$E \in \mathfrak{P}(E)$$. Thác triển của $$f$$ trên $$E'$$ là một ánh xạ $$g: E' \rightarrow F$$ thoả mãn:
> ## $$\forall x \in E, g(x) = f(x)$$

**Chú ý**

- Từ định nghĩa trên tụi mình hoàn toàn có thể suy ra, một ánh xạ $$f: E \rightarrow F$$ có vô số trên ánh xạ trên $$E'$$ (trừ trường hợp E = E').

**Ví dụ**
<br/>
- Để tụi mình có ánh xạ $$f$$ có đồ thị như hình vẽ
<center><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="400px" version="1.1" content="&lt;mxfile userAgent=&quot;Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36&quot; version=&quot;8.0.9&quot; editor=&quot;www.draw.io&quot;&gt;&lt;diagram id=&quot;ce097fa3-9f2c-2cf3-520c-73d41972da54&quot; name=&quot;Page-1&quot;&gt;7ZjPk5sgFMf/Go87o2LMetyku+2l087soWeqRJklYpFsTP/6gkAUMebHpGl3dnNIyJfHg7zPg4fxwHLdfGawKr7SDBEv9LPGA5+8MExmvniXwk4Js/lcCTnDmZKCTnjGv5EW9bh8gzNUW4acUsJxZYspLUuUckuDjNGtbbaixJ61gjlyhOcUElf9gTNeKPXe/Cypf0E4L8zMga97fsL0JWd0U+r5vBCs2pfqXkPjS9vXBczotieBRw8sGaVctdbNEhEZWhM2Ne7pQO9+3QyV/JQBoRrwCskGmRW36+I7EwtUZg8ypOJbSmBd49QDi4KviRAC0aw5oy9oSQll7QDgt699jwmgtF3RkmvaQFqoyVDm0OjWH+yjIpIN0TXibCdMth0WQ6XoETEaQwRy/Gq7hzo78r27/QzfKRYTh75O5DDSfkweR8B2UdMNS5Ee1Y/zwFE8P+KIQ5Yj7jgSjd7P7qQW4zhS8IH0JkiHjvZ7+vpI70eQxoTr6Fts418bajru6pbLgzAQAJquU7Ry+dkYN2IBypPSnYThqOFTKVLSEslJMSEDCRKclzLPBH0k9MUrYhyLk/ZBd6xxlslpFtsCc/RcwVTOuRVlRWjtSYpkFPyDqSYdoubcZDP70skGHeteMkYjyThk3c87C/QE1eQvUf327qkGSTy+x29A1VxhRrDWFSwvx7rrYVWe3jvWPa8bYAXnlVUd0Kma+vR0Sk0N30JNjQL7FAXxIOKn1tTZMUcHaqoIO9z1zCppUE8sGAzmSfzJdUXxmfbzmW1/b9mLhlrxxXe8+A1ko3hma2npJc//ZYYO67xzJpx8kU9udusDcwfy6v8/7MNr3cyGgQ5ud9hHYzX86PbKYF20EQmu8jT1Jk/+WXThvjpaQq63r6Lgg+5pdIfl+GK6l9b1S+iGDt3H93NqRsPn2Ti53anp1isn8HUBK9lMN4zsFgymL/J+MBqrHpwubNM7rs/L0geBdiAyysU+oVK7S66FYgZsFL77EBoAF0XgT+zTAyzE1+4/Y7Vpuv/lweMf&lt;/diagram&gt;&lt;/mxfile&gt;" onclick="(function(svg){var src=window.event.target||window.event.srcElement;while (src!=null&amp;&amp;src.nodeName.toLowerCase()!='a'){src=src.parentNode;}if(src==null){if(svg.wnd!=null&amp;&amp;!svg.wnd.closed){svg.wnd.focus();}else{var r=function(evt){if(evt.data=='ready'&amp;&amp;evt.source==svg.wnd){svg.wnd.postMessage(decodeURIComponent(svg.getAttribute('content')),'*');window.removeEventListener('message',r);}};window.addEventListener('message',r);svg.wnd=window.open('https://www.draw.io/?client=1&amp;lightbox=1&amp;edit=_blank');}}})(this);" viewBox="0 0 535 381" style="cursor:pointer;max-width:100%;max-height:381px;"><defs/><g transform="translate(0.5,0.5)"><path d="M 44 334 L 467.63 334" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 472.88 334 L 465.88 337.5 L 467.63 334 L 465.88 330.5 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 44 334 L 44 17.37" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 44 12.12 L 47.5 19.12 L 44 17.37 L 40.5 19.12 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><g transform="translate(458.5,331.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="10" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 11px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;"><font style="font-size: 20px">x</font></div></div></foreignObject><text x="5" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">[Not supported by viewer]</text></switch></g><g transform="translate(11.5,326.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="16" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 16px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;"><font style="font-size: 20px">O</font></div></div></foreignObject><text x="8" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">[Not supported by viewer]</text></switch></g><g transform="translate(14.5,3.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="10" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 11px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;"><span style="font-size: 20px">y</span></div></div></foreignObject><text x="5" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">[Not supported by viewer]</text></switch></g><path d="M 214 151 L 228.45 172.68 Q 234 181 244 181 L 254 181 Q 264 181 271.5 176 L 275.25 173.5 Q 279 171 287.68 166.04 L 314 151" fill="none" stroke="#ff0000" stroke-miterlimit="10" pointer-events="none"/><path d="M 444 11 L 494 11" fill="none" stroke="#ff0000" stroke-miterlimit="10" pointer-events="none"/><g transform="translate(510.5,-0.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="6" height="22" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 20px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 6px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">f</div></div></foreignObject><text x="3" y="21" fill="#000000" text-anchor="middle" font-size="20px" font-family="Helvetica">f</text></switch></g><path d="M 214 331 L 214 151" fill="none" stroke="#000000" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="none"/><path d="M 314 331 L 314 151" fill="none" stroke="#000000" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="none"/><g transform="translate(256.5,358.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="14" height="22" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 20px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 14px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">E</div></div></foreignObject><text x="7" y="21" fill="#000000" text-anchor="middle" font-size="20px" font-family="Helvetica">E</text></switch></g><path d="M 270 294 L 266.75 294 Q 263.5 294 263.5 304 L 263.5 334.5 Q 263.5 344.5 260.25 344.5 L 258.63 344.5 Q 257 344.5 260.25 344.5 L 261.88 344.5 Q 263.5 344.5 263.5 354.5 L 263.5 385 Q 263.5 395 266.75 395 L 270 395" fill="none" stroke="#000000" stroke-miterlimit="10" transform="rotate(-90,263.5,344.5)" pointer-events="none"/></g></svg></center>
<br/>
Thì ánh xạ $$g$$ là thác triển của $$f$$ trên $$E'$$ có thể là:
<br/>
<center><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="400px" version="1.1" content="&lt;mxfile userAgent=&quot;Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36&quot; version=&quot;8.0.9&quot; editor=&quot;www.draw.io&quot;&gt;&lt;diagram id=&quot;ce097fa3-9f2c-2cf3-520c-73d41972da54&quot; name=&quot;Page-1&quot;&gt;7VpLc5swEP41np7aAQQ4HGPHaS+ddiaHnlWQQROMXCG/+usrAeIhYbAZ7Na1OSTyarUr77cvIU/AfLX/TOE6+koCFE8sI9hPwMvEsjzH4H8F4ZATnOk0J4QUBznJrAhv+DcqiMW6cIMDlDYYGSExw+sm0SdJgnzWoEFKya7JtiRxU+sahkgjvPkw1qk/cMCinPokv5agf0E4jKRm0yhmfkL/PaRkkxT6JhZYZk8+vYJSVsGfRjAguxoJLCZgTglh+Wi1n6NYmFaaLV/3emS23DdFCTtlgZUv2MJ4g+SOs32xg7QFSoJnYVL+yY9hmmJ/AmYRW8WcYPJhyih5R3MSE5otAEb2lDPSgIJ3SRJWoA0ER64MBRoa1f7N0irc2RBZIUYPnGVXwSJRiWqISBpFMWR42xQPC+8IS3Glhu8Ec8WWUTiyZRdypB/boCkiJRvqo2JV3c6KIHfaI4hBGiKmCeKD2teuSBmM7ZCCB6RXgVQVVMb0+JA+tUDqxqywfgNb99eGyImPaYbLM2fgAOyrST4Kxf+9FMM3kEvK6ZrDMLRnXS6SkAQJpTiOFRKMcZgIP+PoI06fbRFlmGfa52JihYNAqJntIszQ2xr6QueOlxVOyzIpElYwjrqaEIj25zqbjEvNGwpb15zRbnFGFeu63zWA7kDVuxCq3+4eVdNz22P8CqjKFqYF1nQNk+GwHmqw5pLuHdYSryvACs4rq4VBu2uq687nfTXVuoWaapvNLApcxeKn1lSnT9CRmsrNDg81trVgSDs2DBQ9ntG5L9s9k3/qNPmfGvx8kO94cI831bxx+e/nAWukPKChYVwvD9ht6b03DwQwjTKLmKM02jeZFBx7YFLozS7jNdq2+UD3NHTVTD0Y3aEpfwi6+tuOxR1lTfWo43rXy5ondE/+hm7LKLpYK8UFv2Kxz5dbiDJLeW0EwJVz6LmNFXCaeizQ3SjJRkry29a4jZJtPxxvjPQ+uKN3VUHGZRzPsdsj5WjZURxPOu5ojuf0O96jk2jLcYM7id5kOWIn4T7QPQ1dNf4Hozs0kQxBVz9da+imEVyLIS8e8WFGof+O2JHOroZ01eR1417vLht0BX2t5aSEcbSIoH30xmocHdCE0NDfpppA9yDT6PCWUztH6YZ/4TrrJuLLHq1DVAuod7H4cgadsu/kXap6I2UNTphej6ARAdUP1qGG6H97sJ4aiqFlCF7hYO2ccLC+lVKVX4C9GJ+A8oxUxuQ1ennUnGowSVIdJqDGzSCc9HPo4sP9hIh63+Je7uaOf6x+PpXnsuonamDxBw==&lt;/diagram&gt;&lt;/mxfile&gt;" onclick="(function(svg){var src=window.event.target||window.event.srcElement;while (src!=null&amp;&amp;src.nodeName.toLowerCase()!='a'){src=src.parentNode;}if(src==null){if(svg.wnd!=null&amp;&amp;!svg.wnd.closed){svg.wnd.focus();}else{var r=function(evt){if(evt.data=='ready'&amp;&amp;evt.source==svg.wnd){svg.wnd.postMessage(decodeURIComponent(svg.getAttribute('content')),'*');window.removeEventListener('message',r);}};window.addEventListener('message',r);svg.wnd=window.open('https://www.draw.io/?client=1&amp;lightbox=1&amp;edit=_blank');}}})(this);" viewBox="0 0 545 429" style="cursor:pointer;max-width:100%;max-height:429px;"><defs/><g transform="translate(0.5,0.5)"><path d="M 44 330 L 467.63 330" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 472.88 330 L 465.88 333.5 L 467.63 330 L 465.88 326.5 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 44 330 L 44 13.37" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 44 8.12 L 47.5 15.12 L 44 13.37 L 40.5 15.12 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><g transform="translate(458.5,327.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="10" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 11px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;"><font style="font-size: 20px">x</font></div></div></foreignObject><text x="5" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">[Not supported by viewer]</text></switch></g><g transform="translate(11.5,322.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="16" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 16px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;"><font style="font-size: 20px">O</font></div></div></foreignObject><text x="8" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">[Not supported by viewer]</text></switch></g><g transform="translate(14.5,-0.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="10" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 11px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;"><span style="font-size: 20px">y</span></div></div></foreignObject><text x="5" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">[Not supported by viewer]</text></switch></g><path d="M 214 147 L 228.45 168.68 Q 234 177 244 177 L 254 177 Q 264 177 271.5 172 L 275.25 169.5 Q 279 167 287.68 162.04 L 314 147" fill="none" stroke="#0066cc" stroke-miterlimit="10" pointer-events="none"/><g transform="translate(280.5,85.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="6" height="22" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 20px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 6px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">f</div></div></foreignObject><text x="3" y="21" fill="#000000" text-anchor="middle" font-size="20px" font-family="Helvetica">f</text></switch></g><path d="M 214 327 L 214 147" fill="none" stroke="#000000" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="none"/><path d="M 314 327 L 314 147" fill="none" stroke="#000000" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="none"/><g transform="translate(256.5,354.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="14" height="22" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 20px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 14px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">E</div></div></foreignObject><text x="7" y="21" fill="#000000" text-anchor="middle" font-size="20px" font-family="Helvetica">E</text></switch></g><path d="M 74 117 Q 154 17 174 112 Q 194 207 214 147" fill="none" stroke="#0066cc" stroke-miterlimit="10" pointer-events="none"/><path d="M 314 147 Q 344 117 369 127 Q 394 137 414 87" fill="none" stroke="#0066cc" stroke-miterlimit="10" pointer-events="none"/><path d="M 74 327 L 74 117" fill="none" stroke="#000000" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="none"/><path d="M 414 327 L 414 87" fill="none" stroke="#000000" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="none"/><path d="M 270 290 L 266.75 290 Q 263.5 290 263.5 300 L 263.5 330.5 Q 263.5 340.5 260.25 340.5 L 258.63 340.5 Q 257 340.5 260.25 340.5 L 261.88 340.5 Q 263.5 340.5 263.5 350.5 L 263.5 381 Q 263.5 391 266.75 391 L 270 391" fill="none" stroke="#000000" stroke-miterlimit="10" transform="rotate(-90,263.5,340.5)" pointer-events="none"/><path d="M 274 117 L 246.85 171.3" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 244.5 176 L 244.5 168.17 L 246.85 171.3 L 250.76 171.3 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 444 27 L 494 27" fill="none" stroke="#0066cc" stroke-miterlimit="10" pointer-events="none"/><g transform="translate(517.5,15.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="12" height="22" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 20px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 12px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">g</div></div></foreignObject><text x="6" y="21" fill="#000000" text-anchor="middle" font-size="20px" font-family="Helvetica">g</text></switch></g><path d="M 259 214 L 250 214 Q 241 214 241 224 L 241 374 Q 241 384 236.5 384 L 234.25 384 Q 232 384 236.5 384 L 238.75 384 Q 241 384 241 394 L 241 544 Q 241 554 250 554 L 259 554" fill="none" stroke="#000000" stroke-miterlimit="10" transform="rotate(-90,245.5,384)" pointer-events="none"/><g transform="translate(244.5,405.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="18" height="22" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 20px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 18px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">E'</div></div></foreignObject><text x="9" y="21" fill="#000000" text-anchor="middle" font-size="20px" font-family="Helvetica">E'</text></switch></g></g></svg></center>
<br/>
Hoặc $$g$$ thế này:
<br/>
<center><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="400px" version="1.1" content="&lt;mxfile userAgent=&quot;Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36&quot; version=&quot;8.0.9&quot; editor=&quot;www.draw.io&quot;&gt;&lt;diagram id=&quot;ce097fa3-9f2c-2cf3-520c-73d41972da54&quot; name=&quot;Page-1&quot;&gt;7Vpbk5owFP41Tp/aAQK4PK6u27502pl96HMKEZiNxIZ4669vAgmXREUZtLXKw248OTmJ5ztX4ghMF9vPFC6TryRCeORY0XYEXkaOE3gW/ysIu5LgjcclIaZpVJLsmvCW/kaSKNfFqzRCeYuREYJZumwTQ5JlKGQtGqSUbNpsc4Lbuy5hjAzCWwixSf2RRiwpqU/qawn6F5TGidrZtuTMTxi+x5SsMrnfyAHz4imnF1DJkvx5AiOyaZDAbASmlBBWjhbbKcJCtUpt5brXA7PVuSnK2CkLnHLBGuIVUicuzsV2Shcoi56FSvmnEMM8T8MRmCRsgTnB5sOcUfKOpgQTWiwAVvFUM0qBgndOMibRBoKj3AxFBhr1+e1KK9zYEFkgRnecZVPDolBJGogoGkUYsnTdFg+ldcSVuGqH7yTlGzuWNGTHlXKUHbugLSInKxoiuaqpZ02QP+4QxCCNETME8UHja9ekAsb9kIIHpFeBVBdU+fTwkD7tgdTHTGq/ha3/a0XUxMe8wOWZM3AAtvUkH8Xi/1aJ4QcoJZV0w2AY2rJjJpKRDIlNU4w1EsRpnAk74+gjTp+sEWUpj7TPcmKRRpHYZrJJUobeljAUe254WuG0IpIioQXroKkJgWh7rrEpvzSsQeq6YYzuHmPUsW7aXQvoI6gGF0L1292jagf+fh+/AqqqhNkDa76EWX9Ydw1YS0n3DmuF1xVgBeelVanQ4znV96fTrpzq3EJOde12FAW+pvFTc6rXJehATuVqh7sG21Iw5EcODLR9AuvouVz/TP6x1+Z/avHzQXni3jXe2LDG+b8fB5yB4oCBhnW9OODuC++dcSCCeVJoxB6k0L7JoOC5PYNCZ3QZrtB27Qe6p6GrR+re6PYN+X3QNd92zO4oauqtjh9cL2qeUD2FK7quvOhipRQX/JqKc77cgpc52msjAK4cQ88trKpULPdxOwoloBdiVgd/oMl3hi2sXPdhqEOkg94dgK8Lsi5jqJ5meKpvP5imnjTDcwc2PK/b8B6Vx76Y2Lvy6AyuA1Ye/gPd09DV/b83un0DSR90zW7cQDdP4FIMefLAuwmF4TtiByrBBtJ1UXgc92Y12qJr6BslKiWMo0UE7WMwVKHpgTaElvn21QamBdnWEWs5tdJUZvgXrr9uwr/cwSpKrZ2oKrPh/cvr1ZXfybtX/QbL6R0wgw5BAwJqNuKxgeh/24iPtR7JUS54hUbcO6ERv5VUVV6YvVifgPYMlMbUtXvVao4NmBSpCRPQ/aYXTmYfOvtwPy6i38/4l7vp4x/rn1uVsaz+SRuY/QE=&lt;/diagram&gt;&lt;/mxfile&gt;" onclick="(function(svg){var src=window.event.target||window.event.srcElement;while (src!=null&amp;&amp;src.nodeName.toLowerCase()!='a'){src=src.parentNode;}if(src==null){if(svg.wnd!=null&amp;&amp;!svg.wnd.closed){svg.wnd.focus();}else{var r=function(evt){if(evt.data=='ready'&amp;&amp;evt.source==svg.wnd){svg.wnd.postMessage(decodeURIComponent(svg.getAttribute('content')),'*');window.removeEventListener('message',r);}};window.addEventListener('message',r);svg.wnd=window.open('https://www.draw.io/?client=1&amp;lightbox=1&amp;edit=_blank');}}})(this);" viewBox="0 0 545 429" style="cursor:pointer;max-width:100%;max-height:429px;"><defs/><g transform="translate(0.5,0.5)"><path d="M 44 330 L 467.63 330" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 472.88 330 L 465.88 333.5 L 467.63 330 L 465.88 326.5 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 44 330 L 44 13.37" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 44 8.12 L 47.5 15.12 L 44 13.37 L 40.5 15.12 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><g transform="translate(458.5,327.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="10" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 11px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;"><font style="font-size: 20px">x</font></div></div></foreignObject><text x="5" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">[Not supported by viewer]</text></switch></g><g transform="translate(11.5,322.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="16" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 16px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;"><font style="font-size: 20px">O</font></div></div></foreignObject><text x="8" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">[Not supported by viewer]</text></switch></g><g transform="translate(14.5,-0.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="10" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 11px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;"><span style="font-size: 20px">y</span></div></div></foreignObject><text x="5" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">[Not supported by viewer]</text></switch></g><path d="M 214 147 L 228.45 168.68 Q 234 177 244 177 L 254 177 Q 264 177 271.5 172 L 275.25 169.5 Q 279 167 287.68 162.04 L 314 147" fill="none" stroke="#0066cc" stroke-miterlimit="10" pointer-events="none"/><g transform="translate(280.5,85.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="6" height="22" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 20px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 6px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">f</div></div></foreignObject><text x="3" y="21" fill="#000000" text-anchor="middle" font-size="20px" font-family="Helvetica">f</text></switch></g><path d="M 214 327 L 214 147" fill="none" stroke="#000000" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="none"/><path d="M 314 327 L 314 147" fill="none" stroke="#000000" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="none"/><g transform="translate(256.5,354.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="14" height="22" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 20px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 14px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">E</div></div></foreignObject><text x="7" y="21" fill="#000000" text-anchor="middle" font-size="20px" font-family="Helvetica">E</text></switch></g><path d="M 74 117 Q 104 277 119 182 Q 134 87 164 147 Q 194 207 214 147" fill="none" stroke="#0066cc" stroke-miterlimit="10" pointer-events="none"/><path d="M 314 147 Q 334 -3 359 112 Q 384 227 414 87" fill="none" stroke="#0066cc" stroke-miterlimit="10" pointer-events="none"/><path d="M 74 327 L 74 117" fill="none" stroke="#000000" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="none"/><path d="M 414 327 L 414 87" fill="none" stroke="#000000" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="none"/><path d="M 270 290 L 266.75 290 Q 263.5 290 263.5 300 L 263.5 330.5 Q 263.5 340.5 260.25 340.5 L 258.63 340.5 Q 257 340.5 260.25 340.5 L 261.88 340.5 Q 263.5 340.5 263.5 350.5 L 263.5 381 Q 263.5 391 266.75 391 L 270 391" fill="none" stroke="#000000" stroke-miterlimit="10" transform="rotate(-90,263.5,340.5)" pointer-events="none"/><path d="M 274 117 L 246.85 171.3" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 244.5 176 L 244.5 168.17 L 246.85 171.3 L 250.76 171.3 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 444 27 L 494 27" fill="none" stroke="#0066cc" stroke-miterlimit="10" pointer-events="none"/><g transform="translate(517.5,15.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="12" height="22" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 20px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 12px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">g</div></div></foreignObject><text x="6" y="21" fill="#000000" text-anchor="middle" font-size="20px" font-family="Helvetica">g</text></switch></g><path d="M 259 214 L 250 214 Q 241 214 241 224 L 241 374 Q 241 384 236.5 384 L 234.25 384 Q 232 384 236.5 384 L 238.75 384 Q 241 384 241 394 L 241 544 Q 241 554 250 554 L 259 554" fill="none" stroke="#000000" stroke-miterlimit="10" transform="rotate(-90,245.5,384)" pointer-events="none"/><g transform="translate(244.5,405.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="18" height="22" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 20px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 18px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">E'</div></div></foreignObject><text x="9" y="21" fill="#000000" text-anchor="middle" font-size="20px" font-family="Helvetica">E'</text></switch></g></g></svg></center>
<br/>
Hay ánh xạ $$g$$ là thế này
<br/>
<center><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="400px" version="1.1" content="&lt;mxfile userAgent=&quot;Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36&quot; version=&quot;8.0.9&quot; editor=&quot;www.draw.io&quot;&gt;&lt;diagram id=&quot;ce097fa3-9f2c-2cf3-520c-73d41972da54&quot; name=&quot;Page-1&quot;&gt;7ZpLc9owEIB/DdNTOrZlm3AMhLSXTjuTQ8+qLWxNhEVlEaC/vpJl+SHx9BhSCj4kZiWtxH67q5XNAEzm6y8MLtJvNEZk4DnxegCeB543ChzxVwo2ShAMh0qQMBwrkVsLXvEfVArLcckSxyhvdeSUEo4XbWFEswxFvCWDjNFVu9uMkvasC5ggS/AaQWJLf+KYp0r6qL+WlH9FOEn1zK5TtvyC0VvC6DIr5xt4YFZcqnkOta6yf57CmK4aIjAdgAmjlKu7+XqCiDStNpsa97KjtVo3Qxk/ZoCnBrxDskR6xcW6+EbbAmXxkzSp+BQRmOc4GoBxyudECFxxm3NG39CEEsqKAcAprqpFG1D2ndGMl7SB7KEmQ7FFo16/W1lFOBuic8TZRnRZ1Vg0lbRBRMsYIpDj97Z6WHpHUqmrZvhBsZjYc0pH9vxSj/ZjH7RV5HTJIlSOatrZUBQODyjikCWIW4rETeNr16IC43ak4I70IkhNRVVM94/0cQvSkPDS+i224e8l1Q0PecHlSXQQANZ1o7hL5P+1ViMWoDQpueUwHK35PhfJaIbkpJgQQwQJTjLpZ4I+EvLxO2Ici0z7VDbMcRzLacarFHP0uoCRnHMlthUhKzIpklZwdrqaVIjWpzqbjkvLG0pbN5zR3+KMJuum37VA76E6OhPV7zdP1R2F22P8AlR1CbMFa76AWXesmwZWpenWsVa8LoAVnLatlgbdv6eG4WRyaE/1rmFP9d12FgWhYfFj99TgkKIde6owO9w0ui1kh3zPgoExz8jZuy4/PLH/MGj3f2z1FzdqxZ1rvKHljbN/Pw94PeUBi4ZzuTzgb0vvB/NADPO0sIjbS6F9lUkh8DsmhYPZpb9C23fvdI+ja2bqznS7pvwudO2nHdMbyprmUSccXS5rfmT1JBS/YLm052sILM94UuRrrz01sEB4QFGPgeXf8R6bN40orDa3k58omnnTOV/eDO67Yrfg7bwr2lngfHTDO93j6Joh15nuJWPXPiladPMULuRttGRkM2YwekN8R5XSIF0XLPu5Nyulltygb5VPjHJBi0rZw6ivIigAbYSO/WTQBbYHuc4ebzm2CtJu+AGvZq4ivnwj6QHQMb7MUlc/rjlDfAWdTow38lzQfLvidU6YowOKegRqHxITi+h/e0gcOoahdQhe4JAYHHFIvJatSr3MeXY+A+PqaRvTr4R1eegNLUxa1MQEzLjpxMk+7U0/3U6ImO8OwvO9hRIf658CqVxW/9wKTP8C&lt;/diagram&gt;&lt;/mxfile&gt;" onclick="(function(svg){var src=window.event.target||window.event.srcElement;while (src!=null&amp;&amp;src.nodeName.toLowerCase()!='a'){src=src.parentNode;}if(src==null){if(svg.wnd!=null&amp;&amp;!svg.wnd.closed){svg.wnd.focus();}else{var r=function(evt){if(evt.data=='ready'&amp;&amp;evt.source==svg.wnd){svg.wnd.postMessage(decodeURIComponent(svg.getAttribute('content')),'*');window.removeEventListener('message',r);}};window.addEventListener('message',r);svg.wnd=window.open('https://www.draw.io/?client=1&amp;lightbox=1&amp;edit=_blank');}}})(this);" viewBox="0 0 545 429" style="cursor:pointer;max-width:100%;max-height:429px;"><defs/><g transform="translate(0.5,0.5)"><path d="M 44 330 L 467.63 330" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 472.88 330 L 465.88 333.5 L 467.63 330 L 465.88 326.5 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 44 330 L 44 13.37" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 44 8.12 L 47.5 15.12 L 44 13.37 L 40.5 15.12 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><g transform="translate(458.5,327.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="10" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 11px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;"><font style="font-size: 20px">x</font></div></div></foreignObject><text x="5" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">[Not supported by viewer]</text></switch></g><g transform="translate(11.5,322.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="16" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 16px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;"><font style="font-size: 20px">O</font></div></div></foreignObject><text x="8" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">[Not supported by viewer]</text></switch></g><g transform="translate(14.5,-0.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="10" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 11px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;"><span style="font-size: 20px">y</span></div></div></foreignObject><text x="5" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">[Not supported by viewer]</text></switch></g><path d="M 214 147 L 228.45 168.68 Q 234 177 244 177 L 254 177 Q 264 177 271.5 172 L 275.25 169.5 Q 279 167 287.68 162.04 L 314 147" fill="none" stroke="#0066cc" stroke-miterlimit="10" pointer-events="none"/><g transform="translate(280.5,85.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="6" height="22" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 20px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 6px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">f</div></div></foreignObject><text x="3" y="21" fill="#000000" text-anchor="middle" font-size="20px" font-family="Helvetica">f</text></switch></g><path d="M 214 327 L 214 147" fill="none" stroke="#000000" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="none"/><path d="M 314 327 L 314 147" fill="none" stroke="#000000" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="none"/><g transform="translate(256.5,354.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="14" height="22" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 20px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 14px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">E</div></div></foreignObject><text x="7" y="21" fill="#000000" text-anchor="middle" font-size="20px" font-family="Helvetica">E</text></switch></g><path d="M 74 229 L 164 229" fill="none" stroke="#0066cc" stroke-miterlimit="10" pointer-events="none"/><path d="M 344 197 L 414 87" fill="none" stroke="#0066cc" stroke-miterlimit="10" pointer-events="none"/><path d="M 74 327 L 74 227" fill="none" stroke="#000000" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="none"/><path d="M 414 327 L 414 87" fill="none" stroke="#000000" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="none"/><path d="M 270 290 L 266.75 290 Q 263.5 290 263.5 300 L 263.5 330.5 Q 263.5 340.5 260.25 340.5 L 258.63 340.5 Q 257 340.5 260.25 340.5 L 261.88 340.5 Q 263.5 340.5 263.5 350.5 L 263.5 381 Q 263.5 391 266.75 391 L 270 391" fill="none" stroke="#000000" stroke-miterlimit="10" transform="rotate(-90,263.5,340.5)" pointer-events="none"/><path d="M 274 117 L 246.85 171.3" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 244.5 176 L 244.5 168.17 L 246.85 171.3 L 250.76 171.3 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 444 27 L 494 27" fill="none" stroke="#0066cc" stroke-miterlimit="10" pointer-events="none"/><g transform="translate(517.5,15.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="12" height="22" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 20px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 12px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">g</div></div></foreignObject><text x="6" y="21" fill="#000000" text-anchor="middle" font-size="20px" font-family="Helvetica">g</text></switch></g><path d="M 259 214 L 250 214 Q 241 214 241 224 L 241 374 Q 241 384 236.5 384 L 234.25 384 Q 232 384 236.5 384 L 238.75 384 Q 241 384 241 394 L 241 544 Q 241 554 250 554 L 259 554" fill="none" stroke="#000000" stroke-miterlimit="10" transform="rotate(-90,245.5,384)" pointer-events="none"/><g transform="translate(244.5,405.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="18" height="22" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 20px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 18px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">E'</div></div></foreignObject><text x="9" y="21" fill="#000000" text-anchor="middle" font-size="20px" font-family="Helvetica">E'</text></switch></g></g></svg></center>

Và tại sao tụi mình lại quan tâm đến thác triển ánh xạ? Trên thực tế, sẽ có nhiều hiện tượng, mà để miêu tả nó thì việc dùng một hàm sơ cấp (như hàm sin, cos, đa thức, ...) thì sẽ không miêu tả được hoặc để đảm bảo một hàm luôn xác định trên tập nguồn của nó, tụi mình phải nghĩ đến việc kết hợp các hàm sơ cấp lại với nhau. Trong trường hợp đó, thác triển ánh xạ thường được sử dụng.

**Ví dụ**
- Tụi mình biết từ 0 đến 100 độ C thì nhiệt độ của nước phụ thuộc tuyến tính vào thời gian còn điểm sôi thì nhiệt sôi thì nhiệt độ của nước không đổi.Tụi mình có thể giả sử như sau: từ 0 đến 4 phút, hàm nhiệt độ $$T = 20 + 20*t$$, từ 4 phút đến 6 phút $$T = 100$$. Như vậy là tụi mình có hàm $$T = \begin{cases} 20 + 20t, \quad \text{nếu} \,\,\,  0 \leq t \leq 4 \\ 100, \quad \text{nếu} \,\,\, 4 < t \leq 6 \end{cases}$$.
<br/> Hàm $$T$$ là thác triển của hàm $$ \underset{t \rightarrow 20 + 20t}{[0,4] \rightarrow [0,100]}$$, và cũng là thác triển của hàm $$\underset{t \rightarrow 100}{(4,6] \rightarrow [0,100]}$$<br/>
Đồ thị hàm $$T$$ có dạng là:<br/>
<center><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="400px" version="1.1" content="&lt;mxfile userAgent=&quot;Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36&quot; version=&quot;8.0.9&quot; editor=&quot;www.draw.io&quot;&gt;&lt;diagram id=&quot;ce097fa3-9f2c-2cf3-520c-73d41972da54&quot; name=&quot;Page-1&quot;&gt;7ZdNj5swEIZ/DcdKBBOSHBO6bS9VK6VSzy5MwFqDqTGB9NfXxjYfgSS7VTdVtcshMa/HM2aegQEHhVnzkeMi/cxioI7nxo2D3juet1m68lcJJy0sVystJJzEWlr0wp78AiOadUlFYihHhoIxKkgxFiOW5xCJkYY5Z/XY7MDoOGqBE5gI+wjTqfqdxCLV6tpeltI/AUlSG3nhmpkfOHpMOKtyE8/x0KE99HSGrS9jX6Y4ZvVAQg8OCjljQo+yJgSqUmvTptd9uDDb7ZtDLp6ywNMLjphWYHfc7kucbC4gj7cqpfIsorgsSeSgXSoyKoWFHJaCs0cIGWW8XYDc9uhmbAKV7YHlwtBGykIHg3hCo9//osuKLDZgGQh+kiZ1j8VSSQdErMaBYkGOY/fYVEfSuesifGVEBvZcU8ieb/zYOvbR2EXJKh6BWTXM85mjYHXDkcA8ATFxJAeDy+6lFuM8UvSG9C5Izx119/TfR7qeQRpQYbI/Yhv8rJideFe2XLbSQAJo+kk5StS/sG7kBrQnrU8KRkAjrpVIznJQQQmlZxKmJMlVnUn6IPXdEbgg8km7NRMZiWMVZlenRMC+wJGKWcu2IrX2SQoqC+7FUlMOoXlusdn7clINJteDYvRnivGc9bDuRqCvUN28ENUvr57qYhPM3+N3oGpfYWawlgXO/xzrtwFW7em1Y+143QHrcvmstmoSer2nBkEY3uqp3n/ZU92zjD+1p/ru2BHyX6ynLoM3oBeB+usbHP49UHnafyZp8/5TFD38Bg==&lt;/diagram&gt;&lt;/mxfile&gt;" onclick="(function(svg){var src=window.event.target||window.event.srcElement;while (src!=null&amp;&amp;src.nodeName.toLowerCase()!='a'){src=src.parentNode;}if(src==null){if(svg.wnd!=null&amp;&amp;!svg.wnd.closed){svg.wnd.focus();}else{var r=function(evt){if(evt.data=='ready'&amp;&amp;evt.source==svg.wnd){svg.wnd.postMessage(decodeURIComponent(svg.getAttribute('content')),'*');window.removeEventListener('message',r);}};window.addEventListener('message',r);svg.wnd=window.open('https://www.draw.io/?client=1&amp;lightbox=1&amp;edit=_blank');}}})(this);" viewBox="0 0 485 363" style="cursor:pointer;max-width:100%;max-height:363px;"><defs/><g transform="translate(0.5,0.5)"><path d="M 44 330 L 467.63 330" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 472.88 330 L 465.88 333.5 L 467.63 330 L 465.88 326.5 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 44 330 L 44 13.37" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 44 8.12 L 47.5 15.12 L 44 13.37 L 40.5 15.12 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><g transform="translate(460.5,327.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="6" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 6px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;"><font style="font-size: 20px">t</font></div></div></foreignObject><text x="3" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">[Not supported by viewer]</text></switch></g><g transform="translate(11.5,322.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="16" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 16px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;"><font style="font-size: 20px">O</font></div></div></foreignObject><text x="8" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">[Not supported by viewer]</text></switch></g><g transform="translate(13.5,-0.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="12" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 14px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;"><span style="font-size: 20px">T</span></div></div></foreignObject><text x="6" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">[Not supported by viewer]</text></switch></g><path d="M 44 287 L 204 127" fill="none" stroke="#0066cc" stroke-miterlimit="10" pointer-events="none"/><path d="M 284 127 L 204 127" fill="none" stroke="#0066cc" stroke-miterlimit="10" pointer-events="none"/></g></svg></center>
- Hay một người đi bộ, từ 0 đến 2h, di chuyển thẳng đều từ A đến B với vận tốc 10km/h, sau đó từ 2h-3h, lại đi từ B về A với vận tốc 20 km/h, sau đó từ 3h - 5h lại đi từ A đến với vận tốc 5km/h. Với toạ độ của A,B,C so với gốc O là 0, 20, 10. Từ 0 đến 2h, tụi mình xác định được một hàm $$\underset{t \rightarrow 10t}{[0,2] \rightarrow \mathbb{R}}$$, tương tự từ 2h đến 3h, hàm $$\underset{t\rightarrow 20 - 20(t-2)}{(2,3]\rightarrow \mathbb{R}}$$ và từ 3h đến 5h có hàm $$\underset{t  \rightarrow 5(t-3)}{(3,5]\rightarrow \mathbb{R}}$$.<br/>
Vậy tụi mình có thác triển $$s=  \begin{cases} 10t, \quad \text{nếu} \,\,\,  0 \leq t \leq 2 \\ 20 - 20(t-2), \quad \text{nếu} \,\,\, 2 < t \leq 3 \\ 5(t-3), \quad \text{nếu} \,\,\, 3 < t \leq 5 \end{cases}$$.<br/>
Đồ thị hàm $$s$$ có dạng
<center><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="333px" version="1.1" content="&lt;mxfile userAgent=&quot;Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36&quot; version=&quot;8.0.9&quot; editor=&quot;www.draw.io&quot;&gt;&lt;diagram id=&quot;ce097fa3-9f2c-2cf3-520c-73d41972da54&quot; name=&quot;Page-1&quot;&gt;7ZhNj5swEIZ/DcdKBAPJHhN2216qVsqhZxcmYK3B1JhA+utrY5uvfGy3aiJVCYfEvDOeMfMMmMRBUd5+4rjMvrAEqOO5SeugZ8fzngJXfirhoIVgudRCykmipcUgbMkvMKKZl9YkgWriKBijgpRTMWZFAbGYaJhz1kzddoxOs5Y4hSNhG2N6rH4nici0urKXpfTPQNLMZl64xvIDx68pZ3Vh8jke2nWHNufYxjL+VYYT1owk9OKgiDMm9ChvI6CqtLZset7HM9Z+3RwK8ScTPD1hj2kNdsXdusTB1gKKZK1KKs9iiquKxA7aZCKnUljIYSU4e4WIUca7Ccjtjt5iC6h8d6wQhjZSHjoZJEc0hvUv+qrIZgOWg+AH6dIMWCyVbETEahwoFmQ/DY9Nd6R9uD7DN0ZkYs81jez5Jo7tY8vNhqhYzWMws8Z1ngUK0BuBBOYpiKNAcjC67EHqMJ5Gih5Ib4J0HgihqyFdnUAaUmGqP2Eb/qyZNXyoOi5r6SABtINRjlL1LWwYuQAdSetHDSOgFZdapGAFqKSE0pmEKUkL1WeSPkh9swcuiHzSro0hJ0mi0myajAjYljhWORu5rUite5KCqoJ7ttVUQGjf22z2vnRn3WAhjprRP9GM86YZ990E9AWqT1ei+vXuqfbvEf09jm5G1aY+gbUqcfH3WKsRVh3p7rC6q+kT17vdzRoE79pWTUEv76lhGEVv7aneXe2pPVETyPevtqcG4QPoWaAo/A+BLh9Arw/Un70w+at/BVSeDr97tfvw3wJ6+Q0=&lt;/diagram&gt;&lt;/mxfile&gt;" onclick="(function(svg){var src=window.event.target||window.event.srcElement;while (src!=null&amp;&amp;src.nodeName.toLowerCase()!='a'){src=src.parentNode;}if(src==null){if(svg.wnd!=null&amp;&amp;!svg.wnd.closed){svg.wnd.focus();}else{var r=function(evt){if(evt.data=='ready'&amp;&amp;evt.source==svg.wnd){svg.wnd.postMessage(decodeURIComponent(svg.getAttribute('content')),'*');window.removeEventListener('message',r);}};window.addEventListener('message',r);svg.wnd=window.open('https://www.draw.io/?client=1&amp;lightbox=1&amp;edit=_blank');}}})(this);" viewBox="0 0 333 244" style="cursor:pointer;max-width:100%;max-height:244px;"><defs/><g transform="translate(0.5,0.5)"><path d="M 32 207 L 315.63 207" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 320.88 207 L 313.88 210.5 L 315.63 207 L 313.88 203.5 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 32 207 L 32 23.37" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 32 18.12 L 35.5 25.12 L 32 23.37 L 28.5 25.12 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><g transform="translate(308.5,209.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="6" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 6px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;"><font style="font-size: 20px">t</font></div></div></foreignObject><text x="3" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">[Not supported by viewer]</text></switch></g><g transform="translate(13.5,202.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="16" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 16px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;"><font style="font-size: 20px">O</font></div></div></foreignObject><text x="8" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">[Not supported by viewer]</text></switch></g><g transform="translate(14.5,-0.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="10" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 11px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;"><span style="font-size: 20px">s</span></div></div></foreignObject><text x="5" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">[Not supported by viewer]</text></switch></g><path d="M 32 207 L 112 127" fill="none" stroke="#0066cc" stroke-miterlimit="10" pointer-events="none"/><path d="M 152 207 L 112 127" fill="none" stroke="#0066cc" stroke-miterlimit="10" pointer-events="none"/><path d="M 152 207 L 192 167" fill="none" stroke="#0066cc" stroke-miterlimit="10" pointer-events="none"/></g></svg></center>
- Ánh xạ $$ f :\underset{x \rightarrow \frac{1}{x}}{\mathbb{R}^* \rightarrow \mathbb{R}}$$ không xác định tại $$x = 0$$. Muốn cho $$f$$ xác định trên toàn bộ $$\mathbb{R}$$, tụi mình tụi mình có thể tại $$x = 0$$, ánh xạ có một giá trị nào đó. Ví dụ như $$g=  \begin{cases} \frac{1}{x}, \quad \text{nếu} \,\,\, t \neq 0 \\ 0, \quad \text{nếu} \,\,\, t = 0 \end{cases}$$.
<br/>

## Thu hẹp của ánh xạ
Cho $$E,F$$ là hai tập hợp, $$f: E \rightarrow F$$ là một ánh xạ, $$A \in \mathfrak{P}(E)$$. Thu hẹp của $$f$$ vào $$A$$, kí hiệu $$f\vert_A$$, là ánh xạ được xác định bởi:
> ## $$ f\vert_A : \underset{x \rightarrow f(x)}{A \rightarrow F}$$

Thu hẹp của ánh xạ ở đây có nghiã "ngược lại" với "thác triển". Thác triển ánh xạ được sử dụng khi bạn chỉ quan tâm đến tính chất mang tính "địa phương", nghĩa là trong một "khoảng nhỏ" của tập nguồn thì ánh xạ sẽ thay đổi như thế nào, ánh xạ có liên tục hay không,... Ở các ví dụ đối với thác triển ở của ánh xạ, tụi mình có $$g$$ là thác triển của ánh xạ $$f$$, điều này cũng tương đương với $$f$$.<br/>

**Ví dụ**
<br/>
- Để cho các bạn dễ tưởng tượng hơn vì có vẽ một hình ví dụ.
<center><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="400px" version="1.1" content="&lt;mxfile userAgent=&quot;Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36&quot; version=&quot;8.0.9&quot; editor=&quot;www.draw.io&quot;&gt;&lt;diagram id=&quot;ce097fa3-9f2c-2cf3-520c-73d41972da54&quot; name=&quot;Page-1&quot;&gt;7ZpJc5swFIB/Dcd0ALHYR5sk7aXTzuTQswoyaIKRK+Stv74SQiwCL8U2E0/sgyM/SU/y+94i4RggWO6+UrhKvpMIpYZtRjsDPBu2PXVN/i4EeylwfV8KYoojKbJqwRv+i0phOS9e4wjlrYGMkJThVVsYkixDIWvJIKVk2x62IGl71RWMUUfwFsK0K/2FI5ZI6UR9LSH/hnCcqJUts+z5DcP3mJJ1Vq5n2GBRvGT3Eipd5fg8gRHZNkTgxQABJYTJ1nIXoFSYVplNzns90Fvtm6KMnTPBlhM2MF0jteNiX2yvbIGyaCZMyj+FKcxzHBpgnrBlygUWb+aMkncUkJTQYgIwi1fVowwoxi5IxkraQIyQi6GoQ6Pev1VZhTsbIkvE6J4P2dZYFJWkQUTJKEohw5u2elh6R1ypq1b4STBf2DZLR7adUo/yY8VNqcjJmoaonNW0s6bIBScUMUhjxDqKeKPxtWtRgbEfKXggHQWprsgGN0M66UHqpay0fout92dNVMdTXnCZ8QEcwK7u5K1Y/N0pNXwDUpOUdxyGoR075iIZyZBYFKepJoIpjjPhZ5w+4vL5BlGGeaadlR1LHEVimfk2wQy9rWAo1tzyssJlRSZFwgrmQVcTCtHuf51NxaWpeYOC2HBGp8cZdadp+l0L9BGq0xtR/fHpqVbniCrGwWhU1dI9WPMVzIZj3TewSk2fDqsWrBWvEbB6Z5TVcE03xfcXNm/U2NK6xwus5wXBqQJrm1LxKxb7fL6LcutrzKYDy60zaSsC3nnllkOA+8awlRiQH9nwVMsdlnl8X5pTgvaJmzfkDobWfs857XhdX4tgnlSuePnJzr5HVxt+sjvls9c72Xnug+55dPX4r2r6WIlkCF3vQfc8uhWES2NXVwRuGLv+g+6ZdPWaOpjudLzY7buejfMc5T6Y6oHmDmWq52P/ZkyV5qtfuRcHr9zX0G74wQH9s45LfozLn3H5ZQ+A/nP1GJc93zroJ5fd4Rf3dYe/AkZHTxNjYrRPp/A8gSvR5Hf3dD+nMHxH7IBtGjBqMx1P800+LbmW7DvQKGE8ORMhe5peK6KUPaoqbHVQTLok9Mfag0h0n5581NTVX4cvM7zrtQ3vdA1/sxg44wpyLzEgs+uz+cXxHHvi+lb5Dm4TH9VFsYHJcvowuVfg1P2N5+UzRci0ZXrPvFmV4B/rn9flGbL+Fwbw8g8=&lt;/diagram&gt;&lt;/mxfile&gt;" onclick="(function(svg){var src=window.event.target||window.event.srcElement;while (src!=null&amp;&amp;src.nodeName.toLowerCase()!='a'){src=src.parentNode;}if(src==null){if(svg.wnd!=null&amp;&amp;!svg.wnd.closed){svg.wnd.focus();}else{var r=function(evt){if(evt.data=='ready'&amp;&amp;evt.source==svg.wnd){svg.wnd.postMessage(decodeURIComponent(svg.getAttribute('content')),'*');window.removeEventListener('message',r);}};window.addEventListener('message',r);svg.wnd=window.open('https://www.draw.io/?client=1&amp;lightbox=1&amp;edit=_blank');}}})(this);" viewBox="0 0 341 408" style="cursor:pointer;max-width:100%;max-height:408px;"><defs/><g transform="translate(0.5,0.5)"><path d="M 40 307 L 323.63 307" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 328.88 307 L 321.88 310.5 L 323.63 307 L 321.88 303.5 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 40 307 L 40 23.37" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 40 18.12 L 43.5 25.12 L 40 23.37 L 36.5 25.12 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><g transform="translate(314.5,309.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="10" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 11px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;"><font style="font-size: 20px">x</font></div></div></foreignObject><text x="5" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">[Not supported by viewer]</text></switch></g><g transform="translate(21.5,302.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="16" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 16px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;"><font style="font-size: 20px">O</font></div></div></foreignObject><text x="8" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">[Not supported by viewer]</text></switch></g><g transform="translate(14.5,-0.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="10" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 11px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;"><span style="font-size: 20px">y</span></div></div></foreignObject><text x="5" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">[Not supported by viewer]</text></switch></g><path d="M 70 77 Q 90 297 145 202 Q 200 107 280 147" fill="none" stroke="#0066cc" stroke-miterlimit="10" pointer-events="none"/><path d="M 70 307 L 70 77" fill="none" stroke="#000000" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="none"/><path d="M 280 310 L 280 147" fill="none" stroke="#000000" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="none"/><path d="M 160 307 L 160 177" fill="none" stroke="#000000" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="none"/><path d="M 190 307 L 190 147" fill="none" stroke="#000000" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="none"/><path d="M 160 137 L 175.5 152.5" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 179.21 156.21 L 171.78 153.73 L 175.5 152.5 L 176.73 148.78 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><g transform="translate(140.5,105.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="18" height="22" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 20px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;"><font style="font-size: 20px">f</font><font style="font-size: 20px">|</font>A</div></div></foreignObject><text x="9" y="17" fill="#000000" text-anchor="middle" font-size="12px" font-family="Helvetica">[Not supported by viewer]</text></switch></g><g transform="translate(276.5,105.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="6" height="22" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 6px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;"><span style="font-size: 20px">f</span></div></div></foreignObject><text x="3" y="17" fill="#000000" text-anchor="middle" font-size="12px" font-family="Helvetica">[Not supported by viewer]</text></switch></g><path d="M 180 308 L 178 308 Q 176 308 176 315.5 L 176 319.25 Q 176 323 174 323 L 173 323 Q 172 323 174 323 L 175 323 Q 176 323 176 330.5 L 176 334.25 Q 176 338 178 338 L 180 338" fill="none" stroke="#000000" stroke-miterlimit="10" transform="rotate(-90,176,323)" pointer-events="none"/><g transform="translate(168.5,326.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="14" height="22" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 20px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 14px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">A</div></div></foreignObject><text x="7" y="21" fill="#000000" text-anchor="middle" font-size="20px" font-family="Helvetica">A</text></switch></g><path d="M 186 267 L 182.25 267 Q 178.5 267 178.5 277 L 178.5 359.5 Q 178.5 369.5 175.25 369.5 L 173.63 369.5 Q 172 369.5 175.25 369.5 L 176.88 369.5 Q 178.5 369.5 178.5 379.5 L 178.5 462 Q 178.5 472 182.25 472 L 186 472" fill="none" stroke="#000000" stroke-miterlimit="10" transform="rotate(-90,179,369.5)" pointer-events="none"/><g transform="translate(171.5,385.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="14" height="22" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 20px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 14px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">E</div></div></foreignObject><text x="7" y="21" fill="#000000" text-anchor="middle" font-size="20px" font-family="Helvetica">E</text></switch></g></g></svg></center>
- Cho ánh xạ $$f : \underset{x \rightarrow \lvert x \rvert}{\mathbb{R} \rightarrow \mathbb{R}} $$ thì $$f \vert_{(0, +\infty)}: \underset{x \rightarrow \lvert x \rvert}{(0, +\infty) \rightarrow \mathbb{R}}$$. Chủ yếu là các bạn hãy nhớ kí hiệu để sau này khỏi bỡ ngỡ.
<br/>
<br/>

## Ánh xạ cảm sinh
$$E,F$$ là hai tập hợp, $$A \in \mathfrak{P}(E)$$, $$B \in \mathfrak{P}(F)$$, $$f:E\rightarrow F$$ là một ánh xạ sao cho:
>## $$\forall x \in A, f(x)\in B$$

Ánh xạ cảm sinh bởi $$f$$ trên $$A$$ ở nguồn và $$B$$ ở đích là ánh xạ $$\underset{x \rightarrow f(x)}{A \rightarrow B}$$

<br/>
<br/>
Tụi mình cần khái niệm về ánh xạ cảm sinh, vì trong một số trường hợp, tụi mình cần giới hạn "miền giá trị" của ánh xạ lại để thuận tiện cho tính toán, kết quả chính xác hơn và để đỡ tốn chi phí lưu trữ hơn.

**Ví dụ**
- Cho một mặt phẳng, và một đường thẳng nằm trên mặt phẳng. Sẽ có trường hợp bạn chỉ quan tâm đến các vector nằm trên đường thẳng đó thôi và không quan tâm đến các vector không nằm trên đường thẳng. Khi đó, phép cộng các vector trên đường thẳng là ánh xạ cảm sinh từ phép cộng vector trên mặt phẳng.
<br/>
- Giả sử chỉ có người Việt Nam kết hôn với nhau, vậy khi xét một người Việt Nam kết hôn với ai, thì bạn chỉ quan tâm đến tập hợp những người Việt Nam, khi đó ánh xạ "kết hôn" trên Việt Nam là ánh xạ cảm sinh từ ánh xạ "kết hôn" trên thế giới. Tụi mình sẽ có hình vẽ ở dưới, các bạn có thể thấy đối với phép cộng vector trên một đường thẳng thì vector tổng vẫn nằm trên đường thẳng. Khi làm việc với phép cộng các vector nằm trên đường thẳng, tụi mình sẽ không quan tâm đến các vector nằm bên ngoài đường thẳng.
<center><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="400px" version="1.1" content="&lt;mxfile userAgent=&quot;Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36&quot; version=&quot;8.0.9&quot; editor=&quot;www.draw.io&quot; type=&quot;google&quot;&gt;&lt;diagram id=&quot;ca0bd605-04d8-a2e4-8210-f4e2b498fed7&quot; name=&quot;Page-1&quot;&gt;7ZlNb5swGMc/DcdKfuEtx40222VSpR529sABqwZHxmmSffpBsCE4W0OrxFE7cojg74e/8fOzjTEeTsrdN0nWxQ+RUe4hkO08fO8htIBx898K+04IjJBLlnUSHIQn9ptqEWh1wzJajwKVEFyx9VhMRVXRVI00IqXYjsNWgo9rXZOcnghPKeGn6k+WqaJT4wAM+nfK8sLUDIEu+UXS51yKTaXrq0RFu5KSGBsdWhckE9sjCT94OJFCqO6o3CWUt1k1GeuuW/6jtL9lSSs15QK8ADGlcRiBVUCyRXynHV4I3+g06BtVe5MXWmVf2vQ2Z4eW4a+FKnlzBpvDWknxTBPBhTxEY3D49SUmk23sSlRKY0dtRFcTzU6wDK2BfY6aXkdFSZXcNyHbgY/BUxyhMZqknCj2MrYnupvkvV1fw6NgTcUI6B6NQ+2jO7RvgBuLWmxkSvVVx1m3jCI0NoKhZaSIzKk6MWoOjpo9SAeoEwGHbwKcclLXLD3DeLn8K2P0ARn7Fhpso5nK2I8tI+SOcTwzdsI48MdGKHbHeHEFxgCEYZJMYizWJGWqbXf0XyEPgYXcd4fcLIwuzPzzjGubjT0cJ8/d9rh2OHfDt63AZsgXg+xw8oZohuwGcnzDkYxnyK9BDiw2736dCtAZo2tC9mfITiDbCy/f5cIrmCG7Gcn+DSFfY2fkE0GO7Gfyu1+h7IWXw90vGM2QbwLZ5RYnvMb+1wz5/Lx/OcjN6fARpAsfvjHhhz8=&lt;/diagram&gt;&lt;/mxfile&gt;" onclick="(function(svg){var src=window.event.target||window.event.srcElement;while (src!=null&amp;&amp;src.nodeName.toLowerCase()!='a'){src=src.parentNode;}if(src==null){if(svg.wnd!=null&amp;&amp;!svg.wnd.closed){svg.wnd.focus();}else{var r=function(evt){if(evt.data=='ready'&amp;&amp;evt.source==svg.wnd){svg.wnd.postMessage(decodeURIComponent(svg.getAttribute('content')),'*');window.removeEventListener('message',r);}};window.addEventListener('message',r);svg.wnd=window.open('https://www.draw.io/?client=1&amp;lightbox=1&amp;edit=_blank');}}})(this);" viewBox="0 0 362 297" style="cursor:pointer;max-width:100%;max-height:297px;"><defs/><g transform="translate(0.5,0.5)"><path d="M 0 248 L 360 8" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 60 208 L 113.15 172.57" fill="none" stroke="#ff0000" stroke-width="2" stroke-miterlimit="10" pointer-events="none"/><path d="M 118.14 169.24 L 113.7 177.01 L 113.15 172.57 L 109.26 170.35 Z" fill="#ff0000" stroke="#ff0000" stroke-width="2" stroke-miterlimit="10" pointer-events="none"/><path d="M 60 208 L 173.15 132.57" fill="none" stroke="#ff0000" stroke-width="2" stroke-miterlimit="10" pointer-events="none"/><path d="M 178.14 129.24 L 173.7 137.01 L 173.15 132.57 L 169.26 130.35 Z" fill="#ff0000" stroke="#ff0000" stroke-width="2" stroke-miterlimit="10" pointer-events="none"/><path d="M 60 208 L 233.15 92.57" fill="none" stroke="#0066cc" stroke-opacity="0.7" stroke-width="2" stroke-miterlimit="10" pointer-events="none"/><path d="M 238.14 89.24 L 233.7 97.01 L 233.15 92.57 L 229.26 90.35 Z" fill-opacity="0.7" fill="#0066cc" stroke="#0066cc" stroke-opacity="0.7" stroke-width="2" stroke-miterlimit="10" pointer-events="none"/><path d="M 40 128 L 75.43 74.85" fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" pointer-events="none"/><path d="M 78.76 69.86 L 77.65 78.74 L 75.43 74.85 L 70.99 74.3 Z" fill="#000000" stroke="#000000" stroke-width="2" stroke-miterlimit="10" pointer-events="none"/><path d="M 40 128 L 71.76 128" fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" pointer-events="none"/><path d="M 77.76 128 L 69.76 132 L 71.76 128 L 69.76 124 Z" fill="#000000" stroke="#000000" stroke-width="2" stroke-miterlimit="10" pointer-events="none"/><path d="M 40 128 L 113.41 72.94" fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" pointer-events="none"/><path d="M 118.21 69.34 L 114.21 77.34 L 113.41 72.94 L 109.41 70.94 Z" fill="#000000" stroke="#000000" stroke-width="2" stroke-miterlimit="10" pointer-events="none"/><path d="M 220 248 L 168.24 248" fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" pointer-events="none"/><path d="M 162.24 248 L 170.24 244 L 168.24 248 L 170.24 252 Z" fill="#000000" stroke="#000000" stroke-width="2" stroke-miterlimit="10" pointer-events="none"/><path d="M 220 248 L 236.32 280.63" fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" pointer-events="none"/><path d="M 239 286 L 231.84 280.63 L 236.32 280.63 L 239 277.06 Z" fill="#000000" stroke="#000000" stroke-width="2" stroke-miterlimit="10" pointer-events="none"/><path d="M 220 248 L 185.82 282.18" fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" pointer-events="none"/><path d="M 181.58 286.42 L 184.41 277.93 L 185.82 282.18 L 190.07 283.59 Z" fill="#000000" stroke="#000000" stroke-width="2" stroke-miterlimit="10" pointer-events="none"/><path d="M 340 108 L 288.24 108" fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" pointer-events="none"/><path d="M 282.24 108 L 290.24 104 L 288.24 108 L 290.24 112 Z" fill="#000000" stroke="#000000" stroke-width="2" stroke-miterlimit="10" pointer-events="none"/><path d="M 340 108 L 284.24 15.06" fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" pointer-events="none"/><path d="M 281.15 9.92 L 288.7 14.72 L 284.24 15.06 L 281.84 18.84 Z" fill="#000000" stroke="#000000" stroke-width="2" stroke-miterlimit="10" pointer-events="none"/><path d="M 340 108 L 226.33 13.27" fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" pointer-events="none"/><path d="M 221.72 9.43 L 230.42 11.48 L 226.33 13.27 L 225.3 17.63 Z" fill="#000000" stroke="#000000" stroke-width="2" stroke-miterlimit="10" pointer-events="none"/></g></svg></center>
<br/>
- Khi xử lí ảnh, tụi mình cần các hàm, ví dụ như hàm biến ảnh màu thành ảnh trắng đen chẳng hạn. Trên tập hợp tất các tấm ảnh, sẽ có những tấm ảnh "tương tự" nhau, nghĩa là các giá trị mỗi pixel của mỗi ảnh là "gần giống" nhau, ví dụ như tập hợp ảnh các con mèo. Hàm xử lí ảnh trắng đen của mèo là hàm cảm sinh của hàm xử lí ảnh trắng đen trên tập hợp tất cả các ảnh.
<br/>
<br/>

## Ánh xạ có tính ổn định trong một bộ phận
Ánh xạ $$f : E \rightarrow E$$ ổn định trong một bộ phận $$A$$ của $$E$$ khi và chỉ khi:
> ## $$\forall x \in A, f(x) \in A$$

Trên thực tế, tụi mình thường làm việc trên một tập con của một tập hợp, để đảm bảo một ánh xạ trên toàn bộ tập hợp có thể làm việc "trơn tru", không có lỗi trên tập con, thì tập con phải chứa tất cả các "kết quả" có thể có của ánh xạ. Như các bạn có thể để ý thì ánh xạ $$\underset{ x \rightarrow f(x)}{A \rightarrow A}$$ là một ánh xạ cảm sinh trên A.

**Ví dụ**

- Phép cộng trên tập hợp $$\mathbb{R}$$ là ánh xạ ổn định trên tập hợp $$\mathbb{N} \subset \mathbb{R}$$.

- Phép chia trên tập hợp $$\mathbb{R}$$ là ánh xạ không ổn định trên tập hợp $$\mathbb{N} \subset \mathbb{R}$$.

<br/>
<br/>
## Các ánh xạ đặc biệt
<br/>
<br/>

Sau đây mình là danh sách một số ánh xạ mà tụi mình có thể gặp. Các bạn chú ý để sau này gặp khỏi bị cái cảm giác "WHAT?" hay "cái chi đây?".

### Ánh xạ đồng nhất
>Với tập hợp $$E$$ bất kì, ánh xạ $$Id_E : \underset{x \rightarrow x}{E \rightarrow E}$$ là ánh xạ đồng nhất.

Ánh xạ này tụi mình sẽ thường gặp khi làm việc với các ánh xạ có ánh xạ ngược.
<br/>
### Ánh xạ nhúng chính tắc
> Cho tập hợp $$E$$, $$A \in \mathfrak{P}(E)$$, ánh xạ nhúng chính tắc từ $$A$$ vào $$E$$, kí hiệu $$i_{A,E}$$ là ánh xạ xác định bởi: $$i_{A,E}: \underset{x \rightarrow x}{A \rightarrow E}$$

Ánh xạ này thường dùng khi tụi mình làm việc với thác triển và thu hẹp của ánh xạ. <br/>
Tụi mình có $$f \vert_{A} = f\circ i_{A,E}$$<br/>
Chứng minh:<br/>
- $$f \vert_{A} : \underset{x \rightarrow f(x)}{A \rightarrow F}$$<br/>
- $$f\circ i_{E,A}$$ là ánh xạ từ A đến F vì $$i_{A,E}: A \rightarrow E$$ và $$f: E \rightarrow F$$. <br/>
- $$ f\circ i_{E,A} \Leftrightarrow \forall x \in A, \begin{cases} x i_{E,A}  x \\ x f y \end{cases} \Leftrightarrow y = f(x)$$<br/>
- Vậy $$f \vert_{A} = f\circ i_{A,E}$$<br/>
<br/>
- Tương tự, nếu $$g$$ là thác triển trên $$E'$$ thì $$f$$ là thu hẹp của $$g$$ trên E nên: $$g\circ i_{E,E'} = f$$.
<br/>
<br/>

### Luỹ thừa của ánh xạ
Cho $$n \in \mathbb{N} - \{0,1\}$$, ánh xạ $$f : E\rightarrow E$$. Tụi mình sẽ kí hiệu: $$f^0 = Id_E$$, $$f^n = f\circ f^{n-1}$$.<br/>
<br/>

### Ánh xạ hằng
Cho $$E,F$$ là hai tập hợp, $$a\in F$$. Ánh xạ hằng a, kí hiệu là $$a$$, là ánh xạ xác định bởi:
> a: $$\underset{x \rightarrow a}{E \rightarrow F}$$

Ánh xạ này bạn có thể gặp trong các khái niệm về tích phần, hàm liên tục,... <br/>
<br/>

### Hàm chỉ
E là tập hợp, A là tập con của E. Hàm chỉ của A, kí hiệu $$\chi_A $$ (đọc là chi A), xác định bởi:
>## $$\chi_A : \underset{x \rightarrow \begin{cases} 1 \,\,\, \text{nếu} \,\,\, x \in A \\ 0 \,\,\, \text{nếu} \,\,\, x \notin A \end{cases}}{E \rightarrow \{0,1\}}$$

Hàm chỉ giúp tụi mình xác định được các phần tử nào thuộc A, Hàm chỉ có thể gặp khi bạn học về ma trận.
<br/>
<br/>

### Ánh xạ chiếu chính tắc thứ i
$$n \in \mathbb{N}^* , E_1, ..., E_n$$ là những tập hợp. Với mỗi $$ i \in \{1,...,n\}$$, tụi mình có ánh xạ chiếu chính tắc thứ i, kí hiệu là $$ p_i$$, là ánh xạ xác định như sau:
> ## $$p_i: \underset{(x_1,...,x_n)\rightarrow x_i}{E_1 \times ... \times E_n \rightarrow E_i}$$

Nói tên nghe dài dòng chứ thực ra rất đơn giản, ánh xạ này tụi mình thường làm việc với các vector, các vector được biểu diễn theo bộ n gồm n toạ độ của vector, ánh xạ này giúp tụi mình biết toạ độ thứ i của vector là bao nhiêu, vì vậy ánh xạ này còn gọi là ánh xạ toạ độ thứ i. Việc gọi ánh xạ chiếu là với việc lấy mỗi toạ độ thứ i giống như việc bạn chiếu vector lên một trục toạ độ vậy.

<br/>
<br/>
Kết, các bạn không cần phải thuộc hết tất cả khái niệm này, chỉ cần hiểu được các khái niệm này như thế nào là được, để khi nhắc về toán, tụi mình không còn các cảm giác "mơ hồ" nữa. Tụi mình có thể đi chậm nhưng sẽ bước những bước thật vững, cảm ơn các bạn đã đọc đến bài viết này của mình.
<br/>
<br/>
Ted
<br/>
<br/>

# Tham khảo

Đại số 1 - Jean-Marie Monier<br/>
Giáo trình Toán - Thầy Bùi Tuấn Khang<br/>
Naive Set Theory - Paul R. Halmos<br/>
