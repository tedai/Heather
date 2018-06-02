---
layout: post
title:  "Lí thuyết tập hợp - Ánh xạ"
subtitle: "Công cụ của chúng ta"
date:   2018-02-7
categories: [dai-so]
permalink:
cover:
description:
mathjax: true


---

# Mục tiêu

- ### Hàm, ánh xạ là gì?
- ### Ảnh và nghịch ảnh của một bộ phận (tập hợp con)
- ### Ba loại ánh xạ phổ biến

<br/>
Trước khi tìm hiểu về ánh xạ, tụi mình cùng nhắc lại khái niệm quan hệ một chút nhé. Một quan hệ hai ngôi sẽ được định nghĩa từ 3 thành phần, đó là: tập nguồn, tập đích và đồ thị của nó. Mọi quan hệ đều có quan hệ ngược và tụi mình cũng đã nói về hợp của hai quan hệ. Và những gì tụi mình sẽ tìm hiểu về ánh xạ thì ánh xạ cũng sẽ có tập nguồn, tập đích và đồ thị của nó, tụi cũng sẽ tìm hiểu về ánh xạ ngược và hợp hai của hai ánh xạ, thực chất ánh xạ cũng chỉ là quan hệ thôi. Khi tụi mình đã nắm chắc về quan hệ rồi thì không có gì phải lo lắng nữa nhỉ.

Tụi mình đã có tập hợp và nhờ quan hệ, tụi mình đã có thể định nghĩa được quan hệ thứ tự trên tập hợp, và trên tập hợp các phần tử còn có thể có nhiều loại quan hệ khác theo một quy luật "nào đó", không chỉ trong cùng một tập hợp, phần tử ở một tập hợp còn có thể có quan hệ với các phần tử ở các tập hợp khác. Khi nói đến quan hệ, tụi mình thường nói theo cặp, kiểu như, a có quan hệ X với b. Bây giờ, khi nói về ánh xạ, tụi mình sẽ quan tâm ở hơn tới việc chuyển từ phần tử sang phần tử khác ở tập nguồn sẽ gây ra việc chuyển đổi gì đối với phần tử ở tập đích, a có quan hệ X với b, vậy c có quan hệ X với cái gì? Khái niệm ánh xạ sẽ nhấn mạnh hơn về "sự thay đổi" giữa các phần tử. Đó sẽ là cách tụi mình làm việc với tập hợp - sự chuyển đổi phần tử ở tập hợp này sẽ "gây ra" sự chuyển đổi phần tử ở tập hợp khác hay chính nó. Hơi rối nhỉ, khi vào định nghĩa và ví dụ mình sẽ nói rõ hơn. Các khái niệm sau này tụi mình sẽ tìm hiểu hầu hết đều được định nghĩa từ ánh xạ. Vậy ánh xạ là gì?
<br/>
<br/>

# Hàm, ánh xạ là gì?

## Hàm
> Hàm từ $$E$$ đến $$F$$ là một quan hệ $$f$$ từ $$E$$ đến $$F$$ thoả mãn:
> $$\forall (x,y,y') \in E\times F \times F,\, \begin{cases} x\, f \, y \\ x \, f\, y' \end{cases} \Rightarrow y = y' $$

Tụi mình có thể thay đổi qua lại giữa hai kí hiệu $$x \, f \, y$$ và $$ y = f(x)$$.

Tập hợp xác định là tập hợp các phần tử $$x \in E$$ sao cho $$x$$ có quan hệ $$f$$ với phần tử $$y \in F$$. Kí hiệu là $$Def(f)$$. Khi đó $$x$$ được gọi là tạo ảnh của $$y$$ và $$y$$ được gọi là ảnh của $$f$$.

## Ánh xạ
> Ánh xạ $$f$$ từ $$E$$ đến $$F$$ là một hàm từ $$E$$ đến $$F$$ có $$Def(f)=E$$

Tập hợp các ánh xạ từ $$E$$ vào $$F$$ sẽ được kí hiệu là $$F^E$$.<br/>
Hai ánh xạ $$f,g$$ bằng nhau khi có cùng tập nguồn và tập đích và $$\forall x \in E, f(x) = g(x)$$.


Tự dưng đang nói nhiều nói lắm về ánh xạ, rồi "đùng" một phát xuất hiện "hàm" nào ở đây? Các bạn có thể thấy hàm và ánh xạ chỉ khác nhau ở tập xác định. Trong thực tế, hai khái niệm thường hay được dùng qua lại lẫn nhau mà không có quá nhiều khác biệt, và các tính chất đúng với ánh xạ cũng đúng với hàm, nên không cần thiết phải "lăn tăn" quá giữa hàm và ánh xạ làm gì. Và tụi mình thường quen thuộc với khái niệm hàm vì tụi mình thường gặp trường hợp không phải tất cả phần tử thuộc tập nguồn đều có quan hệ với phần tử thuộc tập đích.


**Chú ý**
- Như vậy, từ định nghĩa trên, tụi mình có thể thấy điểm khác biệt lớn nhất là có thêm cái đống ni $$\forall (x,y,y') \in E\times F \times F,\, \begin{cases} x\, f \, y \\ x \, f\, y' \end{cases} \Rightarrow y = y' $$. Điều này có nghĩa là $$x$$ (phần tử của tập nguồn) chỉ có quan hệ nhiều nhất với một $$y$$ (phần tử của tập đích). Đây là đặc điểm giúp tụi mình có thể phân biệt được ánh xạ và quan hệ thông thường.
<br/>
<br/>
Tại sao phải thêm tính chất đó? Trong thực tế, tụi mình thường gặp các quan hệ kiểu như Việt Nam có thủ đô là Hà Nội và hiện giờ Việt Nam không có thủ đô nào khác, hay bạn chỉ có một bố ruột và không có bố ruột nào khác, Điểm của bạn sau khi hoàn thành bài thi là 10 (bạn có khả năng đạt được nhiều điểm khác nhau, nhưng sau khi hoàn thành bài kiểm tra thì kết quả bạn nhận được chỉ là một, có thể 8, 9, 7 ...). Và toán học quan tâm đến những vấn đề như vậy, toán học muốn biết "chính xác" $$x$$ có quan hệ với $$y$$ nào. Không thể là hiện nay, Việt Nam có thủ đô là Hà Nội hoặc thành phố Hồ Chí Minh, hay bạn có bố ruột này và bố ruột khác hay điểm của bạn sau khi đã hoàn thành bài thi là 1 hoặc 10. Đó là lí do tại sao tụi mình cần những tụi mình cần tính chất như trên.

- Ánh xạ còn có thể biểu diễn quan hệ kiểu nguyên nhân - kết quả, và đương nhiên kết quả đó chỉ có một. Khi bạn trải qua một kì thi, thì nguyên nhân ở đây có thể là số thời gian bạn dành cho việc học, ứng với mỗi lượng thời gian thì bạn chỉ có duy nhất một kết quả. Hay khi bạn chọn mua một mặt hàng nào đó, thì ứng với một lượng tiền bạn trả sẽ có một sản phẩm có chất lượng "tương đương" với số tiền bạn bỏ ra.

- Khi nói hay viết hàm hay ánh xạ $$f$$ tụi mình sẽ hiểu là tất cả các phần tử (giá trị) ở tập nguồn có quan hệ $$f$$ với các phần tử ở tập nguồn. Còn khi viết $$f(x)$$ tụi mình sẽ hiểu là một phần tử (hay giá trị) ở tập đích có quan hệ $$f$$ với một phần tử $$x$$ ở tập nguồn.

- Ứng với mỗi phần tử của tập nguồn thì sẽ chỉ có nhiều nhất một phần tử ở tập đích có quan hệ với nó, nhưng ngược lại, ứng với mỗi phần tử ở tập đích sẽ có thể có nhiều hơn một quan hệ ngược với các phần tử ở tập nguồn.

Tụi mình đã có đã có tập hợp, đã có quan hệ thứ tự trên các tập hợp, bây giờ tụi mình cần có "công cụ" để làm việc trên các tập hợp đó, và đó là ánh xạ. Khi nói về ánh xạ, tụi mình quan tâm tới việc chuyển đổi các phần tử ở tập nguồn có gây ra việc chuyển đổi phần tử ở tập đích. Để mình vẽ hình ra thì các bạn sẽ hiểu được thôi hì.

![GlqiM.gif](https://pli.io/GlqiM.gif)

Như các bạn thấy, khi tụi mình chuyển từ phần tử này sang phần tử kia của tập nguồn thì cũng sẽ xảy ra sự chuyển từ phần tử này sang phần tử kia ở tập đích, hay nói cách khác với phần tử ở tập đích "phụ thuộc" vào phần tử ở tập nguồn. Khi làm việc với ánh xạ tụi mình sẽ quan tâm đến việc này nhiều hơn thay vì khi làm việc với quan hệ tụi mình chỉ quan tâm theo từng cặp riêng lẻ.

Và hình ảnh này chắc sẽ quen thuộc với mọi người, các điểm nằm trên $$Ox$$ tượng trưng cho tập nguồn, các điểm nằm trên $$Oy$$ tượng trưng cho tập đích, và các điểm không nằm trên $$Ox$$ và $$Oy$$ ở đây tượng trưng cho đồ thị của ánh xạ.

![GloJH.gif](https://pli.io/GloJH.gif)

Nói tóm lại là khi có tập hợp và quan hệ tụi mình chưa làm việc được gì với tập hợp cả, và ánh xạ sẽ là công cụ giúp tụi mình có thể làm được rất nhiều việc, và "cách làm việc" của ánh xạ được hiểu như trên, việc chuyển từ phần tử này sang phần tử khác ở tập nguồn, nhờ có ánh xạ mà sẽ gây nên sự chuyển từ phần tử này sang phần tử khác ở tập nguồn. Hay cho một biến tượng trưng $$x$$ khi giá trị của $$x$$ thay đổi từ phần tử này sang phần tử khác ở tập nguồn thì sẽ làm một biến tượng trưng $$y$$ (lấy các giá trị là các phần tử ở tập đích) thay đổi. Hay tụi mình có thể nói là $$y$$ phụ thuộc vào $$x$$. Và chú ý là ứng với mỗi $$x$$ chỉ có một $$y$$. Các bạn chắc sẽ thắc mắc tại sao mình phải "rườm rà" như vậy? Điều này là do mình muốn các bạn có một cái nhìn trực quan hơn khi làm việc với tập hợp rời rạc và tập hợp liên tục. Khi làm việc với hàm rời rạc thì mình thấy việc dùng từ "chuyển" thấy có vẻ "hợp lí" hơn, còn khi tụi mình làm với hàm liên tục tụi mình sẽ dùng từ "thay đổi".

**Ví dụ**

- Nếu coi ứng với mỗi giá tiền thì sẽ có một căn nhà với diện tích nhất định, thì quan hệ giữa giá tiền và diện tích nhà sẽ là một ánh xạ và khi tụi mình "thay đổi" giá tiền thì diện tích của căn nhà cũng sẽ "thay đổi". (Nói diện tích nhà "thay đổi", nhưng có thể không thay đổi nhé, đối với ánh xạ thì trường hợp có 2 giá tiền khác nhau nhưng vẫn cùng một diện tích nhà vẫn có thể xảy ra.)

- Nếu coi chiều cao của cột thuỷ ngân trong nhiệt kế ứng với một nhiệt độ nhất định thì quan hệ giữa độ cao của cột thuỷ ngân và nhiệt độ là một ánh xạ.

- Quan hệ "có bố ruột là" là một ánh xạ, tương tự "có vợ là" cũng là một ánh xạ (phản đối đa thê nhé :v). Khi tụi mình "chuyển" từ phần tử này sang phần tử khác thì phần tử ở tập đích cũng sẽ "chuyển" theo, tức là khi chuyển qua xét một người khác thì vợ của người này khác vợ người kia nhé.

- Quan hệ giữa thời gian và vị trí của bạn là một ánh xạ, vị trí của bạn có thể có hoặc không thay đổi theo thời gian nhưng ứng mỗi thời điểm nhất định thì vị trí của bạn chỉ là có một.

- Quan hệ giữa sự nỗ lực của bạn với kết quả bài kiểm tra là một ánh xạ (chú ý nhé bạn có khả năng đạt được điểm từ 1 đến 10 nhưng kết quả của một bạn chỉ có một).

- Quan hệ giữa cặp (kích thước 1, kích thước 2) và diện tích hình chữ nhật là một ánh xạ.

- Quan hệ giữa cặp (số lượng từ đã biết, độ lưu loát) và khả năng nói ngoại ngữ là một ánh xạ.

- Quan hệ giữa tên đăng nhập facebook và mật khẩu là một ánh xạ.

Các bạn chú ý là phần tử của tập hợp có thể là bất cứ thứ gì, là chó, là mèo, là bàn, là ghế, là ma trận, là vector, cũng có thể là ánh xạ ... tập đích và tập nguồn cuả một ánh xạ cũng không phải là ngoại lệ. Nhưng tụi mình không thường thấy các ánh xạ kiểu "có vợ là" ở trên là vì trong toán học, để dễ dàng và thuận tiện cho việc tính toán, người ta phải "mô hình hoá" các đối tượng thực tế hoặc các đối tượng trừu tượng như ánh xạ thành các con số, nhưng cách làm này sẽ "làm mờ" đi bản chất là tụi mình vẫn đang làm việc vô cùng "thực tế" :v. Ví dụ với ánh xạ "có vợ là" ở trên, nếu mình kí hiệu trên tập nguồn là tập hợp các ông chồng có các phần tử là A,B,C... còn kí hiệu trên tập đích là tập hợp các người vợ có các phần tử là 1, 2, 3..., và quan hệ "có vợ là" được là $$f$$ thì mình viết là Tuấn "có vợ là" Trang hay $$f(A) = 32$$, cách nào các bạn sẽ dễ hiểu hơn. Do đó hãy "think out of the box" và đừng ghét những con số.

<br/>
<br/>
Tụi mình đã biết mọi quan hệ đều có quan hệ ngược, và ánh xạ cũng là một quan hệ vậy ánh xạ chắc chắn có một quan hệ ngược ứng với nó. Nhưng để tụi mình có cái gọi là "ánh xạ ngược" thì quan hệ ngược phải thoả mãn điều kiện của ánh xạ. Trên thực tế, không phải quan hệ ngược nào của một ánh xạ cũng là ánh xạ. Ví dụ: Tụi mình có quan hệ "có bố ruột là" là một ánh xạ nhưng quan hệ ngược của nó là "là bố của" lại không phải là một ánh xạ, bởi vì tụi mình chỉ có một bố ruột nhưng một ông bố thì có thể có nhiều con. Hay ứng với kích thước (2,3) thì tụi mình có diện tích hình chữ nhật là 6 nhưng ứng với diện tích hình chữ nhật là 6 thì tụi mình có thể có các kích thước như (2,3) hoặc (1,6). Vậy để một ánh xạ có ánh xạ ngược thì tụi mình cần phải có một điều kiện nào đó, điều đó tụi mình sẽ cùng nhau tìm hiểu ở những phần tiếp theo. Và tại sao tụi mình phải quan tâm đến ánh xạ ngược? Từ ánh xạ tụi mình có thể biết "sự phụ thuộc" của các phần tử ở tập đích vào các phần tử ở tập nguồn, vậy các phần tử ở tập nguồn có "phụ thuộc" vào các phần tử không? Ánh xạ ngược sẽ cho tụi mình biết điều đó. À mà khoan, tại sao tụi mình không tự định nghĩa ánh xạ ngược từ định nghĩa quan hệ ngược nhỉ?
<br/>

## Ánh xạ ngược
> Cho một ánh xạ $$f$$ từ $$E$$ đến $$F$$. $$f^{-1}$$ là ánh xạ ngược của $$f$$ khi:
> $$\begin{cases} f^{-1} \, \text{là một quan hệ ngược của} \, f \\ f^{-1} \, \text{là một ánh xạ} \, \end{cases}$$

## Ánh xạ hợp
Hoàn toàn tương tự tụi mình có thể định nghĩa ánh xạ hợp của 2 ánh xạ là một quan hệ hợp của hai ánh xạ đó mà thoả mãn điều kiện của ánh xạ. Nhưng
> đối với hợp của hai ánh xạ thì nó luôn là một ánh xạ.

Tụi mình hoàn toàn có thể chứng minh.

Tụi mình có thể kí hiệu hợp của hai ánh xạ $$f$$ và $$g$$ là $$ x \,\, g \circ f\,\, z $$ hoặc $$z =  g \circ f (x) = g(f(x))$$.
<br/>
Chứng minh:<br/>
Cho hai ánh xạ $$f : E \rightarrow F$$ và $$g: F \rightarrow G$$. Tụi mình có quan hệ hợp của hai ánh xạ trên được định nghĩa là:<br/>

$$\forall (x,z) \in E \times G, x \,\, g \circ f\,\, z \Leftrightarrow \exists y \in F, \begin{cases} x \,\, f\,\, y \\ y \,\, g\,\, z\end{cases} $$<br/>

Vậy giả sử tồn tại $$z$$ và $$z'$$ sao cho: $$\begin{cases} x \,\, g \circ f\,\, z \\ x \,\, g \circ f\,\, z' \end{cases}$$. Điều này sẽ tương đương với:<br/>

$$ \exists (y,y') \in F^2, \begin{cases} x \,\, f\,\, y \\ y \,\, g\,\, z \\  x \,\, f\,\, y' \\y' \,\, g\,\, z'  \end{cases} \Leftrightarrow \begin{cases} x \,\, f\,\, y \\ x \,\, f\,\, y' \\ y \,\, g\,\, z \\y' \,\, g\,\, z'  \end{cases} \Leftrightarrow  \begin{cases} y = y' \\ y \,\, g\,\, z \\y \,\, g\,\, z' \end{cases} \Leftrightarrow z = z' $$

Và vì $$f$$ và $$g$$ là ánh xạ nên với mọi $$x \in E$$ và mọi $$y \in F$$ tụi mình đều có $$y = f(x) $$ và $$z = g(y)$$, suy ra $$\forall x \in E, z = g(f(x)) = g\circ f(x)$$.<br/>

Vậy $$ g\circ f$$ là một ánh xạ.<br/>

Các bạn lưu ý là vì trong thực tế, tụi mình có thể dùng lẫn lộn được khái niệm hàm và ánh xạ nên định nghĩa về hàm hợp cũng tương tự về định nghĩa của ánh xạ hợp nhé.

**Ví dụ**<br/>
Các ví dụ bây giờ của tụi mình về hợp hai ánh xạ cũng giống như ví dụ về hợp hai quan hệ chỉ khác là các quan hệ của tụi mình bây giờ là ánh xạ.

- Tụi mình có hai ánh xạ: "có bố ruột là" và "là chồng của". Ánh xạ "có mẹ ruột là" là ánh xạ hợp của hai ánh xạ trên.

- Quan hệ giữa "lượng xăng trong bình" và công suất của xe là một ánh xạ, Quan hệ giữa là công suất của xe và vận tốc của xe là ánh xạ, vậy quan hệ giữa lượng xăng trong bình và vận tốc của xe là ánh xạ hợp của hai ánh xạ trên.

- Cho tập hợp $$E = \{1,2,3\}$$, tụi mình có một ánh xạ $$f: E \rightarrow E$$ có đồ thị $$\Gamma = \{(1,1),(2,3),(3,1)\}$$ và ánh xạ $$g: E \rightarrow E$$ có đồ thị $$\Gamma' = \{(1,2), (2,1), (3,3)\}$$. Thì ánh xạ $$ g \circ f $$  sẽ có đồ thị $$\Omega = \{(1,2), (2,3), (3,2)\}$$, và ánh xạ $$f \circ g$$ sẽ có đồ thị $$\Omega '= \{(1,3), (2,1), (3,1)\}$$.

- Ánh xạ $$f(x) = \sqrt{x^2 - 1}$$ là ánh xạ hợp $$g\circ h$$ với $$g(y) = \sqrt{y}$$ và $$h(x) = x^2 - 1$$.

<br/>

**Chú ý**
- Ánh xạ hợp là một ÁNH XẠ (không phải là cái gì mới).

- Phép hợp các ánh xạ có tính chất kết hợp nhưng không có tính giao hoán. Các bạn có thể thấy ở ví dụ trên đồ thị của $$g\circ f$$ và $$ f \circ g$$ là khác nhau. Đây là tính chất cơ bản của phép hợp các ánh xạ, khi chứng minh một định lí nào đó liên quan đến phép hợp các ánh xạ tụi mình thường dùng tính chất này.
<br/>
Tính chất kết hợp được hiểu là, khi hợp nhiều hơn hai ánh xạ, tụi mình có thể hợp hai ánh xạ kề nhau bất kì trước, sau đó lấy ánh xạ hợp vừa mới có đó hợp tiếp với các ánh xạ còn lại.
<br/>
Tính kết hợp:<br/>
Với mọi ánh xạ $$f : E \rightarrow F, g: F \rightarrow G, h: G \rightarrow H$$: $$(h \circ g)\circ f = h \circ (g \circ f)$$<br/>
<br/>
Chứng minh:<br/>
Rõ ràng $$(h \circ g)\circ f$$ và $$ h \circ (g \circ f)$$ có cùng tập nguồn và tập đích.
Lấy $$(x,t)$$ bất kì thuộc $$E \times H$$:<br/>
$$ x \, (h \circ g)\circ f \, t  \Leftrightarrow \exists y \in F, \begin{cases} x \, f\, y \\ y\, h \circ g\, t \end{cases} \Leftrightarrow  \exists y \in F, \exists z \in G,  \begin{cases} x \, f\, y \\ y \, g \, z \\ z \, h \, t \end{cases} \Leftrightarrow \exists z \in G,  \begin{cases} x \, g\circ f \, z \\ z \, h\, t \end{cases} \Leftrightarrow x \,h \circ (g \circ f) \, t$$. <br/>
Vậy suy ra điều phải chứng minh.

<br/>
<br/>
## Ảnh và nghịch ảnh của một bộ phận (tập hợp con)
<br/>

Đây là các khái niệm sinh ra khi tụi mình cần các khái niệm chỉ tập hợp các ảnh và tạo ảnh qua ánh xạ trong một bộ phận. <br/>
Cho $$E,F$$ là hai tập hợp và ánh xạ $$f : E \rightarrow F. \, A \in \mathfrak{P}(E), B \in \mathfrak{P}(F)$$.<br/>
Tụi mình có các định nghĩa về ảnh và nghịch ảnh của một bộ phận là:

> Ảnh của $$A$$ qua $$f$$: $$f(A) = \{y\in F; \exists a \in A, y = f(x)\}$$

> Nghịch ảnh của $$B$$ qua $$f$$ là: $$ f^{-1}(B) = \{ x \in E, f(x) \in B\}$$

**Chú ý**<br/>
- Mọi người để ý rằng, $$f(A)$$ và $$f^{-1}(B)$$ là các tập hợp.

**Ví dụ**
- Cho ánh xạ $$f : \underset{x \rightarrow x^2}{\mathbb{R} \rightarrow \mathbb{R}}$$. Tụi mình có $$f([-1,1]) = [0,1]$$ và $$f^{-1}([1,4]) = [-2,-1] \cup [1,2]$$.

<br/>
<br/>
## Ba loại ánh xạ phổ biến
Tụi mình đã nói nhiều về ánh xạ, bây giờ là lúc tụi mình phân loại nó, tụi mình có 3 loại ánh xạ phổ biến đó là: đơn ánh, toàn ánh và song ánh. Và phổ biến như thế nào thì khi bàn chi tiết, tụi mình sẽ tìm hiểu kĩ hơn.<br/>

<br/>
### Đơn ánh
> Một đơn ánh $$f$$ là một ánh xạ $$f : E \rightarrow F$$ thoả mãn điều kiện:<br/> $$\forall (x,x') \in E^2, f(x) = f(x') \Leftrightarrow x = x'$$

Nói thật, khi học về mấy cái ni mình hay bị nhầm lắm, do đó, mình muốn các bạn có thể phân biệt và nắm rõ nó để có thể vận dụng một cách hiệu quả. <br/>

**Chú ý**
- Điều mình muốn các bạn chú ý đầu tiên, đơn ánh là một ánh xạ và có thêm cái đống ni $$\forall (x,x') \in E^2, f(x) = f(x') \Leftrightarrow x = x'$$. Cái đống ni có nghĩa là không có phần tử nào ở tập nguồn có cùng ảnh, đối với mỗi phần tử của tập nguồn thì ảnh của nó là duy nhất. Do có tính chất này mà từ khi biết một phần tử ở tập đích thì tụi mình hoàn toàn có thể xác định được, nếu tồn tại, tạo ảnh của nó qua $$f$$.
<br/>

- Đơn ánh là một ánh xạ, và ánh xạ là quan hệ mà cứ mỗi phần tử ở nguồn đều chỉ có quan hệ với nhiều nhất với một phần tử ở tập đích, kết hợp với định nghĩa đơn ánh thì có thể hiểu đơn ánh là một kiểu quan hệ một - một.

**Ví dụ**<br/>
Vì sao nói đơn ánh là phổ biến? Từ phần chú ý, các chắc bạn của phát hiện ra đơn ánh là gì trong đời sống hằng ngày của tụi mình rồi. Chỉ là do lâu nay tụi mình không để ý thôi.
<br/>
- Quan hệ giữa bản thân mình và số chứng minh nhân dân là một đơn ánh.
<br/>

- Quan hệ giữa xe máy và biển số xe là một đơn ánh. Và tương tự, hầu hết những quan hệ giữ thông tin cá nhân và bạn đều đơn ánh.
<br/>

- Quan hệ giữa trang web và tên miền của nó là một đơn ánh.
<br/>

- Đơn ánh có vai trò giúp các bạn hiểu được các khái niệm trong cấu trúc dữ liệu (như hash table) và cơ sở dữ liệu.
<br/>

- Ánh xạ $$f : \underset{x \rightarrow x^2} {\mathbb{R} \rightarrow \mathbb{R}} $$ không là đơn ánh. Ánh xạ $$f: \underset{ x \rightarrow x^2}{[0,1] \rightarrow \mathbb{R}}$$ là một đơn ánh.

- Để phân biệt ánh xạ thông thường và đơn ánh, các bạn có thể nhìn hình ảnh này.

<center> <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="400px" version="1.1" content="&lt;mxfile userAgent=&quot;Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36&quot; version=&quot;8.0.7&quot; editor=&quot;www.draw.io&quot; type=&quot;google&quot;&gt;&lt;diagram id=&quot;ca0bd605-04d8-a2e4-8210-f4e2b498fed7&quot; name=&quot;Page-1&quot;&gt;7Vpdk5sgFP01PrYjokYfk+y2felMZ/ah7SNRVpklkiFkk/TXFxU0om5tJonp2jxk5PIhnHuAc0ELLteHzxxt0q8sxtRy7PhgwQfLcUIQyP/ccCwNnjYknMSlCdSGJ/ILK6OtrDsS422joGCMCrJpGiOWZTgSDRvinO2bxZ4Zbb51gxLcMjxFiLat30ks0tIaeHZt/4JJkuo3A1vlrFD0knC2y9T7MpbhMmeNdDOq6DZFMdufmOCjBZecMVE+rQ9LTHNUNWJlvU89uVWXOc7EkAq+v1rZUbRaxVFk23b4QbXwiuhOwaA6Ko4aF9mCdIFMLPYpEfhpg6I8Zy9JIG2pWFOZAvJxKzh7wUtGGS9qQrv4yZxnQqm2F+hIE8uE4gDMiyBKkkwmIjkSLMstVMcwF/jQO1pQYShZidkaC36URXQF7bujZppK72v/gkDZ0hPfQs1JpDiVVG3X4MoHhe9ArOEFsUbbTTkHnskBx4PBb9hv4AG5CjQ94HZ4oMMBV8Hf/Y9/tRCNgb83QfxtA//ZiPj7E8QfNncAOCb/ZxPEf9bE3/G88fAPJoh/YCig2Yj4hxfE/+60pgfuSmvqRqdEds+Q+44/ItnBJSOrf8QBvrHbVrvvKA5wJugAYIZbY86ACca73j3tt2CCAa9nCE4IxnTABCMu39BBTpcOupkDJhhymUsQHPPIAQzR/Fk8z4/vcxwo2m5JNFTqlzn6sB50ACwx48cfMlUlfuaJj16ePBDxQ9XLn+ucsos4bt0XGD6Qw2A7HuGewavZLxBPsHhzjW4788RZXoeztI1jigR5bfazy4PqDd8YkSPoPSB3A4ME5fhULefkXsFoqJrluiFoNFSC0GqoIFQ17PM45gwJdUbi2HAmvc2Snil/G5Y4s7C5pPtnssTzjdPQwLsdS4bEY9dkSe9q08Ofy61D3t2vQ46xDkFoEGM4wwz1YS5o12TYFANOM+IPRxQbzpB4572KDXfIJPdHneSBsY3MztxGfNcgnXvDbWTIJeZ75VgwhGNwVI65hsI4dyPxHYNj4IYcG3Js8F45Bu+eY9CIdUB4rhwO/9DQNTnWcTKyhNYcZGnRwUdgLeYymbsizXMWbpaohG8t7KLAwgofcqvBTSknxFts1Ldy7Yu6lkTJxQmJEJ2rjDWJY9onn4pP8HKx9NAlfy6gdszb7I6PmaoPDE6J5/y92pHJ+qvA0uH1R5fw8Tc=&lt;/diagram&gt;&lt;/mxfile&gt;" onclick="(function(svg){var src=window.event.target||window.event.srcElement;while (src!=null&amp;&amp;src.nodeName.toLowerCase()!='a'){src=src.parentNode;}if(src==null){if(svg.wnd!=null&amp;&amp;!svg.wnd.closed){svg.wnd.focus();}else{var r=function(evt){if(evt.data=='ready'&amp;&amp;evt.source==svg.wnd){svg.wnd.postMessage(decodeURIComponent(svg.getAttribute('content')),'*');window.removeEventListener('message',r);}};window.addEventListener('message',r);svg.wnd=window.open('https://www.draw.io/?client=1&amp;lightbox=1&amp;edit=_blank');}}})(this);" viewBox="0 0 541 378" style="cursor:pointer;max-width:100%;max-height:378px;"><defs/><g transform="translate(0.5,0.5)"><ellipse cx="90" cy="222" rx="90" ry="155" fill="none" stroke="#000000" pointer-events="none"/><ellipse cx="80" cy="112" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="80" cy="192" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="60" cy="242" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="85" cy="292" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="125" cy="227" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="135" cy="147" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="450" cy="222" rx="90" ry="155" fill="none" stroke="#000000" pointer-events="none"/><ellipse cx="405" cy="237" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="485" cy="202" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="470" cy="117" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="435" cy="147" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="425" cy="287" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="465" cy="172" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="435" cy="342" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 90 292 L 413.63 287.1" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 418.88 287.02 L 411.94 290.62 L 413.63 287.1 L 411.83 283.62 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 129 227 L 473.65 202.45" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 478.88 202.08 L 472.15 206.07 L 473.65 202.45 L 471.65 199.09 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 65 242 L 414.67 282.27" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 419.89 282.87 L 412.53 285.55 L 414.67 282.27 L 413.34 278.59 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><ellipse cx="485" cy="262" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 85 192 L 453.64 172.34" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 458.88 172.06 L 452.08 175.93 L 453.64 172.34 L 451.71 168.94 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 140 147 L 423.63 147" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 428.88 147 L 421.88 150.5 L 423.63 147 L 421.88 143.5 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 85 112 L 423.66 146.36" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 428.89 146.89 L 421.57 149.66 L 423.66 146.36 L 422.28 142.7 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><g transform="translate(138.5,-0.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="282" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 282px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">ánh xạ thông thường</div></div></foreignObject><text x="141" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">ánh xạ thông thường</text></switch></g></g></svg> </center>
<center><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="400px" version="1.1" content="&lt;mxfile userAgent=&quot;Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36&quot; version=&quot;8.0.7&quot; editor=&quot;www.draw.io&quot; type=&quot;google&quot;&gt;&lt;diagram id=&quot;ca0bd605-04d8-a2e4-8210-f4e2b498fed7&quot; name=&quot;Page-1&quot;&gt;7Vpdk5sgFP01PrYjokYft+62felMZ/ah20eibGSWSIaQTdJfX4xgIpqUZpKwXZuHjFw+hHMPcC7owWy++cLRovzGCky9wC82Hrz3giAFifyvDdvGEGnDjJOiMYG94ZH8wsroK+uKFHjZKSgYo4IsusacVRXORceGOGfrbrFnRrtvXaAZ7hkec0T71h+kEGVjTSJ/b/+KyazUbwa+ypmi/GXG2apS76tYhZucOdLNqKLLEhVsfWCCDx7MOGOieZpvMkxrVDViTb3PR3LbLnNcCZsKcTyd+nk+nRZ57vt++kG18IroSsGgOiq2GhfZgnSBTHxal0TgxwXK65y1JIG0lWJOZQrIx6Xg7AVnjDK+qwn93U/mPBNKtX2HjjSxSigOwLoIomRWyUQuR4JluU+qY5gLvDk6WtBiKFmJ2RwLvpVFdAXtu61mmkqv9/4FibKVB76FmpNIcWrWtr0HVz4ofC2xhhfEGi0XzRx4JhtcWIPfsd/AA3IV6HogHPDAgAOugn/4H/92IXKBfzRC/H0D/4lD/OMR4g+7OwB0yf/JCPGfdPEPosgd/skI8U8MBTRxiH96QfzfnNaMwJvSmrrRMZE9MuR+EDskO7hkZPWPOCA2dtt293XigGCEDgBmuOVyBoww3o3e0n4LRhjwRobghMClA0YYccWGDgqGdNDNHDDCkMtcgqDLIwdgo/mr4q4+vq9xoGi5JLmt1G9y9GE9GABYYsa3TzLVJn7WiY9RndwQ8aTq1c/7nKaLuOjdFxg+kMNgK57jI4NXs18gPsPi5Brdd+aBs6IBZ2kbxxQJ8trt55AH1Ru+MyJHcPSAPEwMEjTjU7WCg3sFo6F2luuGoNFQA0KvoR2h2mGfx7HAJtRxxDF7Jp1myZEpfxuWBJO0u6THZ7Ikio3T0CS6HUts4rFrsuToanMZ/pxciSILjjV4OOOYsRJBaFDDnmOG/jCXtGtybIwhpxnzpw7lRmAT8bxXuRHabCSx00meGBvJ5MyNJA4N0oU33EhsrjHfK8cSG45BpxwLDY1x7kYSBwbHwA05ZnNw8F45Bm045lSsQCPaAem5gjj9Q0PX5NjA2UgWeinwsti7A5XM8jJYP5U97km5IE6xTd+79a/iehKkFh8kR/ROZcxJUdBj8mj3kV0thu6H5M0F1Ix5Xz3wuVL7CcEhsYK/VzMyuf/ur3Ho/rNK+PAb&lt;/diagram&gt;&lt;/mxfile&gt;" onclick="(function(svg){var src=window.event.target||window.event.srcElement;while (src!=null&amp;&amp;src.nodeName.toLowerCase()!='a'){src=src.parentNode;}if(src==null){if(svg.wnd!=null&amp;&amp;!svg.wnd.closed){svg.wnd.focus();}else{var r=function(evt){if(evt.data=='ready'&amp;&amp;evt.source==svg.wnd){svg.wnd.postMessage(decodeURIComponent(svg.getAttribute('content')),'*');window.removeEventListener('message',r);}};window.addEventListener('message',r);svg.wnd=window.open('https://www.draw.io/?client=1&amp;lightbox=1&amp;edit=_blank');}}})(this);" viewBox="0 0 541 378" style="cursor:pointer;max-width:100%;max-height:378px;"><defs/><g transform="translate(0.5,0.5)"><ellipse cx="90" cy="222" rx="90" ry="155" fill="none" stroke="#000000" pointer-events="none"/><ellipse cx="80" cy="112" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="80" cy="192" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="60" cy="242" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="85" cy="292" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="125" cy="227" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="135" cy="147" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="450" cy="222" rx="90" ry="155" fill="none" stroke="#000000" pointer-events="none"/><ellipse cx="405" cy="237" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="485" cy="202" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="470" cy="117" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="435" cy="147" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="425" cy="287" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="465" cy="172" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="435" cy="342" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 90 292 L 413.63 287.1" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 418.88 287.02 L 411.94 290.62 L 413.63 287.1 L 411.83 283.62 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 129 227 L 473.65 202.45" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 478.88 202.08 L 472.15 206.07 L 473.65 202.45 L 471.65 199.09 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 65 242 L 473.64 261.69" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 478.88 261.95 L 471.72 265.11 L 473.64 261.69 L 472.06 258.11 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><ellipse cx="485" cy="262" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 85 192 L 453.64 172.34" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 458.88 172.06 L 452.08 175.93 L 453.64 172.34 L 451.71 168.94 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 140 147 L 423.63 147" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 428.88 147 L 421.88 150.5 L 423.63 147 L 421.88 143.5 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 85 112 L 458.63 116.92" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 463.88 116.99 L 456.84 120.39 L 458.63 116.92 L 456.93 113.39 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><g transform="translate(223.5,-0.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="112" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 114px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">đơn ánh</div></div></foreignObject><text x="56" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">đơn ánh</text></switch></g></g></svg></center>

Từ hình ảnh trên, tụi mình có thể thấy ở ánh xạ thông thường thì ảnh của các phần tử ở tập nguồn vẫn có thể "trùng nhau" còn đối với đơn ánh thì không, cũng từ hình ảnh trên tụi mình có thể thấy rõ được quan hệ "một - một" trong đơn ánh.

<br/>
<br/>
## Toàn ánh
> Một toàn ánh $$f$$ là một ánh xạ $$f : E \rightarrow F$$ thoả mãn điều kiện: $$\forall y \in F, \exists x \in E, y = f(x)$$

Tụi mình có thể hiểu toàn ánh là ánh xạ mà mọi phần tử ở tập đích đều có ít nhất một tạo ảnh.

**Chú ý**
- Toàn ánh là một loại ánh xạ và toàn ánh không mang nghĩa "ngược lại" so với đơn ánh (Điều này hồi trước mình hay nhầm thôi).


**Ví dụ**
- Phép chiếu một đường cong lên một mặt phẳng là một toàn ánh vì ứng với mỗi điểm trên hình chiếu tụi mình đều có được ít nhất một điểm trên đường cong.<br/>

- Trong một ngày, tại một cửa tiệm có bán nhiều mặt hàng (gà, trứng, sữa, ...), trong ngày đó, cửa tiệm bán hết tất cả các sản phẩm của mình thì quan hệ "mua" giữa người mua và mặt hàng là một toàn ánh.

- Các khái niệm toàn ánh và đơn ánh các bạn sẽ gặp khi học về thiết kế dữ liệu (đương nhiên khi dạy người ta không có nói gì về đơn ánh và toàn ánh hết, nhưng nhờ đơn ánh và toàn ánh giúp bạn dễ hiểu vấn đề hơn).

- Ánh xạ $$ f: \underset{x \rightarrow  \lvert x\rvert}{\mathbb{R} \rightarrow \mathbb{R}}$$ không là toàn ánh nhưng ánh xạ $$f: \underset{x \rightarrow \lvert x\rvert}{\mathbb{R} \rightarrow [0,+\infty)}$$ là toàn ánh.

- Tương tự đối với toàn ánh, mình sẽ có hình minh hoạ giúp các bạn phân biệt được đơn ánh và toàn ánh.

<center><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="400px" version="1.1" content="&lt;mxfile userAgent=&quot;Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36&quot; version=&quot;8.0.7&quot; editor=&quot;www.draw.io&quot; type=&quot;google&quot;&gt;&lt;diagram id=&quot;ca0bd605-04d8-a2e4-8210-f4e2b498fed7&quot; name=&quot;Page-1&quot;&gt;7VpPb5swHP00HDdhjAkc27TbLpMm9bDu6IALVh0cOU6T7NPPBBuCIZ0XJaUq66HCz3/A7/f4+WHHg/Pl7qvAq+I7zwjzAj/befDOC4IExOp/BexrABkgFzSrIdACD/Q30aCv0Q3NyLrTUHLOJF11wZSXJUllB8NC8G232RNn3buucE56wEOKWR/9STNZ1GiM/Bb/RmhemDsDX9cscPqcC74p9f1KXpK6ZonNMLrpusAZ3x5B8N6Dc8G5rK+WuzlhFauGsbrflxO1zSMLUkqXDlG0WPhpulhkaer7fvJJj/CC2UbToB9U7g0vagQVAlW43RZUkocVTquarRKBwgq5ZKoE1OVaCv5M5pxxcegJ/cOfqnmijBn8wI6CeCm1BmDVBDOal6qQqpkQ1e5WPxgRkuxOzhY0HCpVEr4kUuxVE9PBxG5vlKbL2za+INZYcRRbaDSJtabyZuyWXHWh+XXkGl6Qa7xe1e/AE92RzJn8Dv4GEVBZoBuBcCACAwG4Cv/hf/6bRDQG/2iC/PsW/7MR+Y8myD/srgBwTP3PJsj/rMt/gNB4/McT5D+2HNBsRP6TC/L/7rwmAu/Ka4JgemKPgG02RxQ7mKDbR+8p24AJ2n1kLbcQjBmACfrNyFoFgqFV4M0C4LLgltlNtXdW8cDwek1T13W2rjE7ZWCAYMWZ2D+qUlP4VRU+o6q4o/JR96uu25r6EUnW26yzYqCmwTciJScmr8UnsciJfDVF9IN5FCw0ECyDCcKwpC/d5xyKoL7DD07VDE7uToWxJYJ6frpXcLSpZw3UiMwMBK2BahJ6Ax0E1Uz7PI2Z76mxNOaqlrGCHMySbkKIzgxyL7PYKeOaQXbZJb5mIjmZLF5LMRdKJMghkdR8jKYxK5FAiM7TGIosjdkZ6Zoam+IHi7U7FSQjuoXAxS9/VLcQuriFaNSXPLYWktm5C0loiS60ssU1X3KXI4CPqrHYRWNwVI2F1mnFuQtJFNhm5Q015vLZ+VE1Bl00NqpZgdbHCkjOzGMo+ctA19RY/yhHcm8OvRu/VPDhCpRFT3fKKsjXlGb2q/tb2D37URkPmmJ2oyuWNMvYKWt0+HFKZYTuhqzNBZyMfc4zcMzfHL0diyr4dyejiu3vZepgtj9Hgvd/AA==&lt;/diagram&gt;&lt;/mxfile&gt;" onclick="(function(svg){var src=window.event.target||window.event.srcElement;while (src!=null&amp;&amp;src.nodeName.toLowerCase()!='a'){src=src.parentNode;}if(src==null){if(svg.wnd!=null&amp;&amp;!svg.wnd.closed){svg.wnd.focus();}else{var r=function(evt){if(evt.data=='ready'&amp;&amp;evt.source==svg.wnd){svg.wnd.postMessage(decodeURIComponent(svg.getAttribute('content')),'*');window.removeEventListener('message',r);}};window.addEventListener('message',r);svg.wnd=window.open('https://www.draw.io/?client=1&amp;lightbox=1&amp;edit=_blank');}}})(this);" viewBox="0 0 541 378" style="cursor:pointer;max-width:100%;max-height:378px;"><defs/><g transform="translate(0.5,0.5)"><ellipse cx="90" cy="222" rx="90" ry="155" fill="none" stroke="#000000" pointer-events="none"/><ellipse cx="80" cy="112" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="80" cy="192" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="60" cy="242" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="85" cy="292" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="125" cy="227" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="135" cy="147" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="450" cy="222" rx="90" ry="155" fill="none" stroke="#000000" pointer-events="none"/><ellipse cx="470" cy="117" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="435" cy="147" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="425" cy="287" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="465" cy="172" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 90 292 L 413.63 287.1" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 418.88 287.02 L 411.94 290.62 L 413.63 287.1 L 411.83 283.62 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 129 227 L 453.7 177.95" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 458.89 177.17 L 452.5 181.67 L 453.7 177.95 L 451.45 174.75 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 65 242 L 473.64 261.69" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 478.88 261.95 L 471.72 265.11 L 473.64 261.69 L 472.06 258.11 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><ellipse cx="485" cy="262" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 85 192 L 453.64 172.34" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 458.88 172.06 L 452.08 175.93 L 453.64 172.34 L 451.71 168.94 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 140 147 L 423.63 147" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 428.88 147 L 421.88 150.5 L 423.63 147 L 421.88 143.5 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 85 112 L 458.63 116.92" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 463.88 116.99 L 456.84 120.39 L 458.63 116.92 L 456.93 113.39 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><g transform="translate(221.5,-0.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="116" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 118px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">toàn ánh</div></div></foreignObject><text x="58" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">toàn ánh</text></switch></g></g></svg></center>

<center><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="400px" version="1.1" content="&lt;mxfile userAgent=&quot;Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36&quot; version=&quot;8.0.7&quot; editor=&quot;www.draw.io&quot; type=&quot;google&quot;&gt;&lt;diagram id=&quot;ca0bd605-04d8-a2e4-8210-f4e2b498fed7&quot; name=&quot;Page-1&quot;&gt;7Vpdk5sgFP01PrYjokYft+62felMZ/ah20eibGSWSIaQTdJfX4xgIpqUZpKwXZuHjFw+hHMPcC7owWy++cLRovzGCky9wC82Hrz3giAFifyvDdvGEGnDjJOiMYG94ZH8wsroK+uKFHjZKSgYo4IsusacVRXORceGOGfrbrFnRrtvXaAZ7hkec0T71h+kEGVjTSJ/b/+KyazUbwa+ypmi/GXG2apS76tYhZucOdLNqKLLEhVsfWCCDx7MOGOieZpvMkxrVDViTb3PR3LbLnNcCZsKcTyd+nk+nRZ57vt++kG18IroSsGgOiq2GhfZgnSBTHxal0TgxwXK65y1JIG0lWJOZQrIx6Xg7AVnjDK+qwn93U/mPBNKtX2HjjSxSigOwLoIomRWyUQuR4JluU+qY5gLvDk6WtBiKFmJ2RwLvpVFdAXtu61mmkqv9/4FibKVB76FmpNIcWrWtr0HVz4ofC2xhhfEGi0XzRx4JhtcWIPfsd/AA3IV6HogHPDAgAOugn/4H/92IXKBfzRC/H0D/4lD/OMR4g+7OwB0yf/JCPGfdPEPosgd/skI8U8MBTRxiH96QfzfnNaMwJvSmrrRMZE9MuR+EDskO7hkZPWPOCA2dtt293XigGCEDgBmuOVyBoww3o3e0n4LRhjwRobghMClA0YYccWGDgqGdNDNHDDCkMtcgqDLIwdgo/mr4q4+vq9xoGi5JLmt1G9y9GE9GABYYsa3TzLVJn7WiY9RndwQ8aTq1c/7nKaLuOjdFxg+kMNgK57jI4NXs18gPsPi5Brdd+aBs6IBZ2kbxxQJ8trt55AH1Ru+MyJHcPSAPEwMEjTjU7WCg3sFo6F2luuGoNFQA0KvoR2h2mGfx7HAJtRxxDF7Jp1myZEpfxuWBJO0u6THZ7Ikio3T0CS6HUts4rFrsuToanMZ/pxciSILjjV4OOOYsRJBaFDDnmOG/jCXtGtybIwhpxnzpw7lRmAT8bxXuRHabCSx00meGBvJ5MyNJA4N0oU33EhsrjHfK8cSG45BpxwLDY1x7kYSBwbHwA05ZnNw8F45Bm045lSsQCPaAem5gjj9Q0PX5NjA2UgWeinwsti7A5XM8jJYP5U97km5IE6xTd+79a/iehKkFh8kR/ROZcxJUdBj8mj3kV0thu6H5M0F1Ix5Xz3wuVL7CcEhsYK/VzMyuf/ur3Ho/rNK+PAb&lt;/diagram&gt;&lt;/mxfile&gt;" onclick="(function(svg){var src=window.event.target||window.event.srcElement;while (src!=null&amp;&amp;src.nodeName.toLowerCase()!='a'){src=src.parentNode;}if(src==null){if(svg.wnd!=null&amp;&amp;!svg.wnd.closed){svg.wnd.focus();}else{var r=function(evt){if(evt.data=='ready'&amp;&amp;evt.source==svg.wnd){svg.wnd.postMessage(decodeURIComponent(svg.getAttribute('content')),'*');window.removeEventListener('message',r);}};window.addEventListener('message',r);svg.wnd=window.open('https://www.draw.io/?client=1&amp;lightbox=1&amp;edit=_blank');}}})(this);" viewBox="0 0 541 378" style="cursor:pointer;max-width:100%;max-height:378px;"><defs/><g transform="translate(0.5,0.5)"><ellipse cx="90" cy="222" rx="90" ry="155" fill="none" stroke="#000000" pointer-events="none"/><ellipse cx="80" cy="112" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="80" cy="192" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="60" cy="242" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="85" cy="292" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="125" cy="227" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="135" cy="147" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="450" cy="222" rx="90" ry="155" fill="none" stroke="#000000" pointer-events="none"/><ellipse cx="405" cy="237" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="485" cy="202" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="470" cy="117" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="435" cy="147" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="425" cy="287" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="465" cy="172" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="435" cy="342" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 90 292 L 413.63 287.1" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 418.88 287.02 L 411.94 290.62 L 413.63 287.1 L 411.83 283.62 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 129 227 L 473.65 202.45" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 478.88 202.08 L 472.15 206.07 L 473.65 202.45 L 471.65 199.09 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 65 242 L 473.64 261.69" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 478.88 261.95 L 471.72 265.11 L 473.64 261.69 L 472.06 258.11 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><ellipse cx="485" cy="262" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 85 192 L 453.64 172.34" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 458.88 172.06 L 452.08 175.93 L 453.64 172.34 L 451.71 168.94 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 140 147 L 423.63 147" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 428.88 147 L 421.88 150.5 L 423.63 147 L 421.88 143.5 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 85 112 L 458.63 116.92" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 463.88 116.99 L 456.84 120.39 L 458.63 116.92 L 456.93 113.39 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><g transform="translate(223.5,-0.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="112" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 114px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">đơn ánh</div></div></foreignObject><text x="56" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">đơn ánh</text></switch></g></g></svg></center>


<br/>
## Song ánh
> Song ánh $$f$$ là ánh xạ $$f:E \rightarrow F$$ thoả mãn điều kiện của đơn ánh và toàn ánh <br/>
> $$\forall y \in F, \exists ! x \in E: y = f(x)$$

**Chú ý**
- Tính chất nổi bật nhất của song ánh: song ánh chính là ánh xạ có ánh xạ ngược. Và tụi mình hoàn toàn có thể chứng minh.<br/>
Chứng minh<br/>
Tụi mình sẽ đi chứng minh quan hệ ngược của song ánh $$f$$ là một ánh xạ. <br/>
Cho một song ánh $$f: E \rightarrow F$$<br/>
$$f^{-1}$$ là quan hệ ngược của $$f$$ suy ra: $$\forall (x,y) \in E\times F, x \, f \, y \Leftrightarrow y \, f^{-1} \, x$$ <br/>
$$f$$ là song ánh $$\Leftrightarrow$$ $$\forall y \in F, \exists ! \, x \in E: y = f(x) \Leftrightarrow \forall y \in F, \exists ! \, x \in E: y \, f^{-1} x$$.<br/>
Theo định nghĩa về ánh xạ thì mỗi phần tử ở tập nguồn chỉ có quan hệ nhiều nhất một phần tử ở tập đích. Ở đây, đối với $$f^{-1}$$, $$x$$ là phần tử ở tập đích và $$y$$ là phần tử ở tập nguồn. Vậy $$f^{-1}$$ thoả mãn điều kiện về ánh xạ.

- Tính chất quan trọng thứ hai của ánh xạ, và tụi mình thường dùng tính chất để tìm ánh xạ ngược của song ánh, đó là $$f \circ f^{-1} = Id_{E}$$. Với $$Id_{E}$$ là ánh xạ $$\underset{x \rightarrow x}{E \rightarrow E}$$. <br/>
Chứng minh:<br/>
$$f: E \rightarrow F$$ là một song ánh <br/>
$$f^{-1}$$ là ánh xạ ngược của $$f$$ suy ra, $$\forall (x,y) \in E\times F, y \, f^{-1} \, x \Leftrightarrow x \, f \, y$$<br/>
$$x \,f \circ f^{-1}\, x' \Leftrightarrow \exists y \in F, \begin{cases}  x \, f \, y \\ y \,f^{-1}\, x' \end{cases} \Leftrightarrow \exists y \in F, \begin{cases}  x \, f \, y \\ x' \,f\, y \end{cases} \Leftrightarrow x = x'$$.

- Song ánh mang tất cả các tính chất của đơn ánh và toàn ánh.

**Ví dụ**

Song ánh là một ánh xạ quan trọng vì tính chất có ánh xạ ngược của nó.

- Hàm $$f(x) = x$$ trên $$\mathbb{R}$$ là một song ánh.

- Quan hệ giữa bạn và ảnh của bạn qua gương là song ánh.

- Quan hệ giữa bạn và dấu vân tay của bạn là song ánh.

Và hình mô tả song ánh sẽ là như thế này.

<center><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="400px" version="1.1" content="&lt;mxfile userAgent=&quot;Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36&quot; version=&quot;8.0.7&quot; editor=&quot;www.draw.io&quot; type=&quot;google&quot;&gt;&lt;diagram id=&quot;ca0bd605-04d8-a2e4-8210-f4e2b498fed7&quot; name=&quot;Page-1&quot;&gt;7Vpdb5swFP01PG7CGAg8tmm3vUya1Id1jw64YNXBkXGaZL9+JtgkGJJaUShRWR4ifP2Bfe7h3oONA+fL7XeOVvlPlmLqeG66deCD43kxiOR/ZdjVhkAbMk7S2gQOhifyFyujq6xrkuKy1VAwRgVZtY0JKwqciJYNcc427WYvjLbvukIZ7hieEkS71t8kFXltjQL3YP+BSZbrOwNX1SxQ8ppxti7U/QpW4LpmifQwqmmZo5Rtjkzw0YFzzpior5bbOaYVqhqxut+3E7XNlDkuhE2HMFws3CRZLNIkcV03/qJGeEN0rWBQExU7jYscQbpAFu43ORH4aYWSqmYjSSBtuVhSWQLyshScveI5o4zve0J3/5M1L4RSbd+jI02sEIoDsGqCKMkKWUjkSrBsd68mhrnA25OrBQ2GkpWYLbHgO9lEd9C+22mmqfLm4F8QKVt+5FuoOYkUp7Jm7AO48kLha4k1vCLWqFzVz8AL2eLUGvyW/QM8IKNA2wN+jwd6HDAI/v5//JtANAb+wQTxdw38ZyPiH04Qf9jOAHBM/s8miP+sjb8XBOPhH00Q/8hQQLMR8Y+viP/Nac0A3JTWBN70yB4CU2yOSHYwQbUf3FK0AROU+4GRbiEY0wET1JuhkQW8vizwYQ6wSbhFelftnVU4UFSWJLHNs3WN3ikDPQBLzPjuWZaawp+q8DWoilsinlW/6vpQU08Rp53NOsMHchlszRN8YvGKfALxDIuzIaLrzCNnBT3O0jaOKRLkrT3PPg+qO/xiRK7g5O6UHxkkqNenenlHm3rGQA3J9EDQGKgGoTPQnlDNsi/jmH6fukWO2TPpLEu8aEyWeLO4HVHCC1nSCU1mzBmSJTbbzEOy5GS0uQ5/zkaiwIZj3qgcMyIRhMFlHAtCg2NmSBuSY1N84zG2t7x4RLnh2Qjuzyo3fBu5EY76kEdGIpldmkh8g3S+ES2GfMhtzhA+K8ciG47BUTnmG8cdlyaS0DPFygdyzOa99bNyDNpwbFSxAo23HRBfGMeC+J2BhuRY9yyoZEUmLc4cOnegyDuUkypBnCOZ3uvubn93lEelOUiC6J2qWJI0padU0f7DlkoDPfSpmiuIGPOMqOcTgebY7phP3iAiZoKHRKFrJvTBVKQsHj52qh+kw7dk8PEf&lt;/diagram&gt;&lt;/mxfile&gt;" onclick="(function(svg){var src=window.event.target||window.event.srcElement;while (src!=null&amp;&amp;src.nodeName.toLowerCase()!='a'){src=src.parentNode;}if(src==null){if(svg.wnd!=null&amp;&amp;!svg.wnd.closed){svg.wnd.focus();}else{var r=function(evt){if(evt.data=='ready'&amp;&amp;evt.source==svg.wnd){svg.wnd.postMessage(decodeURIComponent(svg.getAttribute('content')),'*');window.removeEventListener('message',r);}};window.addEventListener('message',r);svg.wnd=window.open('https://www.draw.io/?client=1&amp;lightbox=1&amp;edit=_blank');}}})(this);" viewBox="0 0 541 378" style="cursor:pointer;max-width:100%;max-height:378px;"><defs/><g transform="translate(0.5,0.5)"><ellipse cx="90" cy="222" rx="90" ry="155" fill="none" stroke="#000000" pointer-events="none"/><ellipse cx="80" cy="112" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="80" cy="192" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="60" cy="242" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="85" cy="292" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="125" cy="227" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="135" cy="147" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="450" cy="222" rx="90" ry="155" fill="none" stroke="#000000" pointer-events="none"/><ellipse cx="470" cy="117" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="435" cy="147" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="425" cy="287" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="465" cy="172" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 90 292 L 413.63 287.1" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 418.88 287.02 L 411.94 290.62 L 413.63 287.1 L 411.83 283.62 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 129 227 L 443.64 212.3" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 448.88 212.05 L 442.05 215.88 L 443.64 212.3 L 441.73 208.88 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 65 242 L 473.64 261.69" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 478.88 261.95 L 471.72 265.11 L 473.64 261.69 L 472.06 258.11 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><ellipse cx="485" cy="262" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 85 192 L 453.64 172.34" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 458.88 172.06 L 452.08 175.93 L 453.64 172.34 L 451.71 168.94 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 140 147 L 423.63 147" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 428.88 147 L 421.88 150.5 L 423.63 147 L 421.88 143.5 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 85 112 L 458.63 116.92" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 463.88 116.99 L 456.84 120.39 L 458.63 116.92 L 456.93 113.39 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><g transform="translate(217.5,-0.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="124" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 124px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">song ánh</div></div></foreignObject><text x="62" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">song ánh</text></switch></g><ellipse cx="455" cy="212" rx="5" ry="5" fill="#000000" stroke="#000000" pointer-events="none"/></g></svg></center>


Vì bài viết đã dài rồi nên mình xin dời những nội dung tiếp theo vào bài viết sau, ánh xạ là một khái niệm quan trọng trong đại số, nên các bạn không nên quá vội vàng khi chưa nắm kĩ khái niệm này. Lời kết, khi các bạn đã đọc tới bài viết này rồi thì chắc bạn cũng đã mong muốn hiểu rõ hơn về đại số, mong các bạn sẽ thu nhặt được nhiều điều từ bài viết của mình. Cảm ơn các bạn đã đọc.

Ted

<br/>
<br/>
# Tham khảo

Đại số 1 - Jean-Marie Monier<br/>
Giáo trình Toán - Thầy Bùi Tuấn Khang<br/>
Naive Set Theory - Paul R. Halmos<br/>
Elements of Set Theory - Herbert B. Enderton<br/>
[Bijection - Wikipedia](https://en.wikipedia.org/wiki/Bijection#Examples)<br/>
[Functions or Mapping - math-only-math.com](http://www.math-only-math.com/functions-or-mapping.html)<br/>
[Functions in real world - educationworld.com](http://www.educationworld.com/a_curr/mathchat/mathchat010.shtml)<br/>
[Examples On One To One Function Or Injection - We teach Academy Math - Youtube Chanel](Examples On One To One Function Or Injection )<br/>
[Injective, Surjective and Bijective - mathisfun.com](https://www.mathsisfun.com/sets/injective-surjective-bijective.html)<br/>
[What is the practical benefit of a function being injective? surjective? - math.stackexchange.com](https://math.stackexchange.com/questions/178796/what-is-the-practical-benefit-of-a-function-being-injective-surjective)<br/>
[Surjective (onto) and injective (one-to-one) functions - Khan Academy](https://www.khanacademy.org/math/linear-algebra/matrix-transformations/inverse-transformations/v/surjective-onto-and-injective-one-to-one-functions)
