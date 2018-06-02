---
layout: post
title:  "Cấu trúc đại số - Các khái niệm cơ bản"
subtitle: "Cấu trúc đại số là gì?"
date:   2018-02-18
categories: [dai-so]
permalink:
cover:
description:
mathjax: true


---

# Mục tiêu

- ### Giới thiệu về cấu trúc đại số.
- ### Một số khái niệm trong cấu trúc đại số

# Giới thiệu các cấu trúc đại số

Đây, đây như ở bài nói về cách học toán, chỗ này chính là phần bắt đầu cảm thấy rối hồi năm nhất. Do đó, mình sẽ cố giải thích với các bạn. Phần giải thích của mình sẽ có phần ngây ngô với cách hiểu của một sinh viên nên nếu có bạn nào phát hiện chỗ sai của mình thì phản hồi với mình nhé.

Tụi mình đã biết về tập hợp, quan hệ và ánh xạ. Về tập hợp, nhờ quan hệ thứ tự, tụi mình đã xác định được thứ tự trên tập hợp, bây giờ, tụi mình cần những "công cụ" có thể làm việc trên tập hợp, đó là các phép toán. Và các phép toán đều được định nghĩa dựa vào ánh xạ. Và việc kết hợp tập hợp với một hoặc hai phép toán thì tụi mình sẽ được các cấu trúc đại số. Các cấu trúc đại số mà tụi mình sẽ tìm hiểu là nhóm, vành, thể, trường, không gian vector và đại số. Nói nhiều hoang mang, thực chất các cấu trúc đại số vẫn chỉ là tập hợp. Mà tập hợp là khái niệm mà tụi mình đã quen thuộc rồi nên không có gì phải lo lắng cả.

Trước hết tụi mình hãy tìm hiểu về các khái niệm cơ bản trong lí thuyết về các cấu trúc đại số nhé.

# Một số khái niệm trong cấu trúc đại số

## Luật hợp thành trong

> Luật hợp thành trong hay phép toán hai ngôi trên một tập hợp $$E$$ là mọi ánh xạ từ $$E\times E$$ vào $$E$$.

Một luật hợp thành trên $$E$$ thường được kí hiệu là $$* : \underset{(x,y) \rightarrow x*y}{E \times E}$$, hoặc $$+,.,\circ$$

Hơi khó hiểu hì, đang nói trong $$E$$ tự dưng xuất hiện $$E\times E$$. Các bạn có hiểu là trong một tập hợp $$E$$, để tụi mình tự hiện phép toán, tụi mình "lấy ra" hai phần tử, và sau khi "thực hiện" phép toán, thì kết quả là một phần tử thuộc $$E$$.

Và tại sao gọi lúc thì gọi là phép toán, lúc thì gọi là luật. Mình gọi là phép toán là vì mình cảm thấy từ "phép toán" có vẻ quen thuộc với tụi mình hơn và cũng để nói đến tính có "đầu vào" và "đầu ra", tụi mình "lấy" mấy cái này và "cho ra" mấy cái kia. Còn về từ luật, thực ra, trong sách của mình học họ chỉ có ghi "luật hợp thành trong" thôi. Luật hợp thành trong được định nghĩa là các ánh xạ từ $$E\times E$$ vào $$E$$, nghĩa là luật hợp thành trong là các ánh xạ có đồ thị là tập hợp các cặp $$((a,b),c)$$ với $$a,b,c \in E$$, điều này cho tụi mình biết ứng với mỗi cặp $$(a,b)$$ chỉ có duy nhất một $$c$$, nhưng nếu hiểu như thế này thì tụi mình "chưa" thực sự làm việc được với tập hợp. Mỗi cặp $$(a,b)$$ sẽ tương ứng với duy nhất một $$c$$ theo một quy luật nào đó. Các quy luật này có thể ngẫu nhiên hoặc xác định, tụi mình cần các quy luật mà tụi mình quan tâm thôi. Và do mình mới có từ luật hợp thành trong.

**Chú ý**
- Luật hợp thành trong là một ÁNH XẠ.

- Các kí hiệu $$* ,+ , \circ, .$$ không nhất thiết là mang nghĩa phép cộng và phép nhân thông thường trong tập hợp số nhé.


**Ví dụ**
- Phép cộng $$+$$ là một luật hợp thành trong $$\mathbb{N}$$. Tụi mình có đồ thị của phép cộng là $$\Gamma = \{((0,0),0),\, ((0,1),1),...\}$$.   

- Ánh xạ  $$* : \underset{(x,y) \rightarrow xy+2}{\mathbb{R}\times \mathbb{R} \rightarrow \mathbb{R}}$$ là một luật hợp thành trong $$\mathbb{R}$$.

- Ánh xạ $$\vert . \vert : \underset{(x,y) \rightarrow \vert x - y\vert}{\mathbb{R}\times \mathbb{R} \rightarrow \mathbb{R}}$$ là một luật hợp thành trong $$\mathbb{R}$$.

- Ánh xạ $$\underset{(x,y) \rightarrow \frac{(x+y)}{2}}{\mathbb{N}\times \mathbb{N}\rightarrow \mathbb{N}}$$ không phải một luật thành trong trên $$\mathbb{N}$$ vì $$\frac{(x+y)}{2}$$ chưa chắc thuộc $$\mathbb{N}$$.

- Trong tập hợp các đồ vật, lấy ra hai cái điện thoại bỏ vô bao nilon tụi mình cũng được một đồ vật. Vậy hành động như vậy tương ứng với một ánh xạ, và ánh xạ đó là một luật hợp thành trong tập hợp các đồ vật.

- Trong tập hợp các tờ giấy A4, việc dán chồng hai tờ giấy lại với nhau là một luật hợp thành trong.


### Tính chất có thể có của luật hợp thành trong
#### Tính ổn định - Tính đóng
> Một luật hợp thành trong $$* $$ trên $$E$$ có tính ổn định trên một tập con $$A$$ của E khi và chỉ khi $$\forall (x,y) \in A^2, x*y \in A$$

#### Tính kết hợp
> Một luật hợp thành trong $$* $$ trên  $$E$$ có tính kết hợp khi và chỉ khi $$\forall (x,y,z) \in E^3, (x*y)* z = x * (y * z)$$.

Điều này có nghĩa là khi một phép toán có tính kết hợp, thì khi kết hợp nhiều phép toán đó lại với nhau thì thứ tự thực hiện phép toán là tuỳ ý. Giống nhau việc tỉa cành của một cái cây thì thứ tự cắt nhánh nào trước không ảnh hưởng đến thành quả cuối cùng.

**Chú ý**
- Không phải phép toán nào cũng có tính kết hợp.

- Tụi mình chỉ đang tính chất kết hợp của MỘT phép toán.

**Ví dụ**
- Cho $$E$$ là một tập hợp. Thì phép giao $$\cap$$ trong $$\mathfrak{P}(E)$$ là một luật hợp thành trong có tính kết hợp.

- Ánh xạ $$\underset{(x,y)\rightarrow x}{\mathbb{R}^2 \rightarrow \mathbb{R}}$$ là một luật hợp thành trong $$\mathbb{R}$$ và nó có tính kết hợp.

#### Tính giao hoán
> Một luật hợp thành trong $$* $$ trên $$E$$ có tính giao hoán khi và chỉ khi $$\forall (x,y) \in E^2, x*y = y*x$$

Đây là một tính chất quan trọng và rất dễ bị "quên". Khi luật hợp thành trong $$* $$ có tính giao hoán thì $$x*y$$ và $$y*x$$ sẽ bằng nhau và tụi mình sẽ coi là một phần tử. Như trong tập hợp số, phép nhân có tính chất giao hoán do đó tụi mình mới có thể ghi $$xy + yx = 2xy$$ nhưng trong tập hợp các ma trận, phép nhân hai ma trận lại không tính giao hoán nên $$XY + YX$$ chưa chắc bằng $$2XY$$.

**Chú ý**
- Không phải phép toán nào cũng có tính giao hoán.

- Nhắc lại điều ở trên nhé :v.

**Ví dụ**
- Phép trừ (ánh xạ $$\underset{(x,y)\rightarrow x - y}{\mathbb{R}^2 \rightarrow \mathbb{R}}$$) trong tập hợp $$\mathbb{R}$$ không có tính giao hoán.

- Ánh xạ $$\underset{(x,y)\rightarrow x}{\mathbb{R}^2 \rightarrow \mathbb{R}}$$ là một luật hợp thành trong $$\mathbb{R}$$ có tính kết hợp nhưng không có tính giao hoán.

- Ánh xạ $$\underset{(x,y) \rightarrow x^y}{\mathbb{R}^2_+ \rightarrow \mathbb{R}^2_+}$$ là một luật hợp thành trong $$\mathbb{R}_+$$ và không có tính giao hoán.

- Cho đoạn mạch gồm đèn và công tắc được mắc nối tiếp như hình vẽ,
<center><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="287px" version="1.1" content="&lt;mxfile userAgent=&quot;Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_3) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/64.0.3282.167 Safari/537.36&quot; version=&quot;8.2.1&quot; editor=&quot;www.draw.io&quot;&gt;&lt;diagram id=&quot;78595903-b96a-8fcd-6ec4-7a1187d73f36&quot; name=&quot;Page-1&quot;&gt;zVbBbtswDP0aXwPbipPm2KbtdtiAAD1sOyo2YwuVTUNWEmdfPymSbCtO0XbztuYQiI8USb1HAg7Iumw/CVoXXzEDHsRh1gbkPojjVRKqfw2cDJCsbgyQC5YZKOqBJ/YTLGjv5XuWQeMFSkQuWe2DKVYVpNLDqBB49MN2yP2qNc1hBDyllI/RbyyThUFv3LM0/hlYXrjKUWg9W5o+5wL3la0XxGR3/hl3SV0uG98UNMPjACIPAVkLRGlOZbsGrql1tJl7jy94u74FVPItF2Jz4UD5HlzH577kyXFxACGZouYL3QLfYMMkw0q5tigllgG5cwG3nOXaIbFWaCFLroxIHRsp8LkjMtZIQWudvmxzPT+zHcdjWlAhZyiUe8c4XyPX5/sKKxV5Z/tUpaB98a1Rx6AaTMASpDipEHshJpZ0O5SLubWPvcRLCxUDdR1G7VDlXeaeWHWw3F7nef46z1Blt3p0+zcPKFRPFKfvygid8UMbs8SZGxBMdQXCxjRSsenyoarrsEfGXVLTAmSjXbhgVC0fFTnIwciMSR6QmFwh0WECOJXs4Fe8xqytsEGmeuk0jFYXGi4TP0WDe5GCvTUc/ItE8dxPtIwvVDZPHiU6C909+03aJ3+ovSeldQ+lDN8h5YfRbR7+nm5R8soATKfb4l262R3zdjYbLNuUC/m/VJxq+f6hiO6LYiIVP7pCJJxIIrL4WxIps/++MeH9NyR5+AU=&lt;/diagram&gt;&lt;/mxfile&gt;" onclick="(function(svg){var src=window.event.target||window.event.srcElement;while (src!=null&amp;&amp;src.nodeName.toLowerCase()!='a'){src=src.parentNode;}if(src==null){if(svg.wnd!=null&amp;&amp;!svg.wnd.closed){svg.wnd.focus();}else{var r=function(evt){if(evt.data=='ready'&amp;&amp;evt.source==svg.wnd){svg.wnd.postMessage(decodeURIComponent(svg.getAttribute('content')),'* ');window.removeEventListener('message',r);}};window.addEventListener('message',r);svg.wnd=window.open('https://www.draw.io/?client=1&amp;lightbox=1&amp;edit=_blank');}}})(this);" viewBox="0 0 287 72" style="cursor:pointer;max-width:100%;max-height:72px;"><defs/><g transform="translate(0.5,0.5)"><ellipse cx="183" cy="36" rx="35" ry="35" fill="none" stroke="#000000" stroke-width="2" pointer-events="none"/><path d="M 158 61 L 208 11" fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" pointer-events="none"/><path d="M 158 11 L 208 61" fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" pointer-events="none"/><path d="M 111 36 L 148 36" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><ellipse cx="108" cy="36" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 108 1 L 68 36" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 11 36 L 65 36" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><ellipse cx="8" cy="36" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="68" cy="36" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 218 36 L 275 36" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><ellipse cx="278" cy="36" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/></g></svg></center>
Đối với đèn, trạng thái đèn không sáng kí hiệu là 0, trạng thái đèn sáng kí hiệu là 1. Như vậy để biểu diễn trạng thái của đèn, tụi mình có tập hợp $$E = \{0,1\}$$. Tụi mình định nghĩa một ánh xạ $$+$$ từ $$E^2$$ đến $$E$$ có đồ thị $$\Gamma = \{((0,0),0),\, ((0,1),1), \, ((1,0),0),\,((1,1),1)\}$$. Hoặc viết dưới dạng kí hiệu của ánh xạ tụi mình có thể viết $$0 + 0 = 0, 0+1= 1, 1+0 = 0, 1+1 =1$$. Tụi mình sẽ đặt cho nó một cái tên là ánh xạ "2 lần bật tắt đèn". Nói như vậy thì chắc các bạn đã suy ra được "quy luật" của ánh xạ trên, coi đèn sáng tương ứng với việc tụi mình bật đèn, và khi đèn không sáng tương ứng với việc tụi mình tắt đèn. Như vậy khi tụi mình "tắt rồi tắt" thì đèn vẫn tắt hay "bật rồi bật" thì đèn vẫn bật, đó là lí do tại sao $$0+0=0$$ và $$1+1=1$$. Rõ ràng ánh xạ trên là một luật hợp thành trong $$E$$ và nó không có tính giao hoán vì $$0+1 \neq 1+0$$.

#### Tính phân phối
Cho $$E$$ là một tập hợp. $$* $$ và $$\top$$ là hai luật hợp thành trong $$E$$.
> $$\top$$ có tính phân phối đối với $$* $$ khi và chỉ khi $$\forall (x,y,z) \in E^3, \begin{cases} x \top (y*z) = (x\top y ) * (x \top z) \\ (y*z) \top x = (y \top x)* (z \top x) \end{cases}$$

Tính phân phối là tính chất có thể có giữa hai luật hợp thành trong $$E$$. Thực ra, khái niệm trên là gộp giữa hai niệm "phân phối trái" và "phân phối phải" tuỳ vào vị trí của $$x$$ so với $$\top$$, nhưng để tụi mình chỉ cần nhớ định nghĩa tính phân phối rồi suy ra định nghĩa về tính phân phối trái, phải cũng được.

**Chú ý**
- Không phải giữa hai luật hợp thành nào cũng có tính phân phối.

- $$\top$$ phân phối với $$* $$ nhưng chưa chắc $$\top$$ có tính giao hoán.

- Sẽ có trường hợp giữa hai luật hợp thành trong có tính phân phối trái mà không có tính phân phối phải và ngược lại. Nếu hai luật hợp thành trong đều có tính phân phối trái và phân phối phải thì hai luật hợp thành có tính phân phối.

**Ví dụ**
- Phép toán $$* : \underset{(x,y) \rightarrow max(x,y)}{\mathbb{R}^2 \rightarrow \mathbb{R}}$$ phân phối với phép $+ : \underset{(x,y) \rightarrow min(x,y)}{\mathbb{R}^2 \rightarrow \mathbb{R}}$$.

- Trên tập hợp số tự nhiên, phép nhân có tính phân phối đối với phép cộng, nhưng phép cộng không có tính phân phối với phép nhân.

- Phép chia trên tập hợp số thực có tính phân phối phải đối với phép cộng nhưng không có tính phân phối trái.

Tụi mình đã có luật hợp thành "trong". Vậy tụi mình có cái chi gọi là luật hợp thành "ngoài" không? Tụi mình hoàn toàn có thể tự định nghĩa luật hợp thành ngoài dựa vào định nghĩa của luật hợp thành trong :v.

## Luật hợp thành ngoài
>Cho hai tập hợp $$E,F$$. Luật hợp thành ngoài hay phép toán ngoài trên $$E$$ là tất cả các ánh xạ $$F \times E \rightarrow E$$ hoặc $$E \times F \rightarrow E$$.

Khác với luật hợp thành trong, đối với luật hợp thành ngoài, tụi mình sẽ "lấy" một phần tử ở tập hợp ngoài, kết hợp với một phần tử ở tập hợp $$E$$ sau khi thực hiện phép toán cho ra kết quả là một phần tử trong $$E$$

**Ví dụ**
- Phép nhân một số với một vector là một luật hợp thành ngoài.

- Phép nhân một số thực với một số nguyên là một luật hợp thành ngoài trên $$R$$.

## Một số loại phần tử trong cấu trúc đại số

### Phần tử trung hoà
Cho tập hợp $$E$$ cùng với luật hợp thành $$* $$ trong $$E$$
> $$e$$ là phần tử trung hoà đối với $$* $$ khi và chỉ khi: $$\forall x \in E, \begin{cases} x*e = x \\ e*x = x \end{cases}$$

Tương tự trong định nghĩa về tính phân phối, định nghĩa về phần tử trung hoà ở đây cũng đã gộp hai khái niệm về phần tử trung hoà trái và phần tử trung hoà, tuỳ vào vị trí của x so với $$* $$. Tụi mình chỉ cần nhớ định nghĩa này thôi rồi suy ra hai định nghĩa còn lại.

**Chú ý**
- Phần tử trung hoà nếu tồn tại thì là duy nhất.<br/>
Chứng minh: Giả sử $$e,e'$$ là hai phần tử trung hoà đối với $$* $$ trong $$E$$. $$\begin{cases} e * e' = e \\ e*e' = e' \end{cases} \Rightarrow e = e'$$.

- Có thể có nhiều phần tử trung hoà trái hoặc phải.

- Một tập hợp có thể không có phần tử trung hoà.

**Ví dụ**
- $$0$$ là phần tử trung hoà đối với phép cộng trong $$\mathbb{N}$$.

- $$Id_E$$ là phần tử trung hoà đối với phép hợp hai ánh xạ $$\underset{(f,g) \rightarrow g\circ f}{E^E\times E^E \rightarrow E^E}$$ trong $$F^E$$

- Đối với ví dụ về "bật tắt đèn" ở trên, trong tập hợp $$E = \{0,1\}$$, tụi mình có $$0 + 0 = 0, \, 0 + 1 = 1$$ nên $$0$$ là phần tử trung hoà trái đối với luật hợp thành $$+$$ trên $$E$$ nhưng $$0$$ không phải là phần tử trung hoà phải vì $$1+0 = 0 \neq 1$$. Nhưng tụi mình lại có $$1$$ là phần tử trung hoà phải vì $$ 0 + 1 = 1, \, 1 + 1 = 1$$.


### Phần tử chính quy
Cho tập hợp $$E$$ cùng với luật hợp thành $$* $$ trong $$E$$
> $$a$$ là phần tử chính quy đối với $$* $$ khi và chỉ khi: $$\forall (x,y) \in E^2, \begin{cases} a*x = a*y \Rightarrow x = y \\ x*a = y*a \Rightarrow x = y \end{cases}$$

Hay nói cách khác đây là các phần tử mà tụi mình có thể "khử" được. Tương tự phần tử trung hoà, tụi mình cũng có định nghĩa về phần tử chính quy trái và phần tử chính quy phải, tùy vào vị trí của $$a$$ đối với $$* $$. Định nghĩa của phần tử trung hoà là gộp từ hai định nghĩa phần tử trung hoà trái và phần tử trung hoà phải.

**Ví dụ**
- Tất cả các phần tử khác $$0$$ trong $$\mathbb{Z}$$ đều là chính quy đối phép nhân.

- Cho luật hợp thành trong $$* : \underset{(x,y) \rightarrow \lvert x \rvert}{\mathbb{Z}^2 \rightarrow \mathbb{Z}}$$, mọi phần tử trong $$\mathbb{Z}$$ đều không phải là phần tử trung hoà đối với $$* $$.

- Xét ví dụ "bật tắt đèn" ở trên, tụi mình có : $$0+0=0, 0+1=1, 1+0 = 0, 1+1=1$$ không có phần tử trung hoà nào đối với $$+$$.


### Phần tử khả nghịch
Cho tập hợp $$E$$ cùng với luật hợp thành $$* $$ trong $$E$$, phần tử trung hoà là $$e$$.

> $$x$$ là phần tử khả nghịch đối với $$* $$ khi và chỉ khi tồn tại một phần tử $$y$$ thuộc $$E$$ sao cho $$x * y = y * x = e$$

**Ví dụ**
- Song ánh là một phần tử khả nghịch đối với phép hợp hai ánh xạ trong tập hợp các ánh xạ.

- Tất cả các phần tử thuộc $$\mathbb{Z}$$ đều là phần tử khả nghịch đối với $$+$$.

- $$0$$ là phần tử khả nghịch đối với phép $$+$$ trong tập hợp $$\mathbb{N}$$.

Chắc các bạn mệt rồi, tụi mình tạm dừng ở đây nhé. Bài viết này mình chỉ mang tính liệt kê, nên mong bài viết sau sẽ thú vị hơn. Hẹn gặp các bạn ở bài viết sau.

> Never give up on a dream just because of the time it will take to accomplish it. The time will pass away anyway. - E.Nightingale

Ted


# Tham khảo

Đại số 1 - Jean-Marie Monier<br/>
Giáo trình Toán - Thầy Bùi Tuấn Khang<br/>
[Binary Operation - Wikipedia](https://en.wikipedia.org/wiki/Binary_operation)<br/>
[Binary Operations - Christina Carter](https://youtu.be/OJPC9AVYJEg)<br/>
[Extenal - Wikipedia](https://en.wikipedia.org/wiki/External_(mathematics)#Other_examples)<br/>
