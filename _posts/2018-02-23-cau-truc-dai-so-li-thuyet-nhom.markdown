---
layout: post
title:  "Cấu trúc đại số - Lí thuyết nhóm"
subtitle: "Nhóm là gì?"
date:   2018-02-23
categories: [dai-so]
permalink:
cover:
description:
mathjax: true


---

# Mục tiêu

- ### Nhóm là gì?
- ### Nhóm con


# Nhóm là gì?
> Một tập hợp $$G$$ cùng với một luật hợp thành trong $$* $$ là một nhóm khi và chỉ khi: $$\begin{cases} * \,\, \text{có tính kết hợp} \\ G \,\, \text{có phần tử trung hoà đối với * } \\ \text{Mọi phần tử của G đều khả nghịch đối với * } \end{cases}$$

Tụi mình thường kí hiệu nhóm là cặp $$(G,* )$$.

Các bạn có hiểu về định nghĩa này không? Với mình, ban đầu chẳng có cái gì để "dính" vào não cả :v. Từ đâu mà ra cái định nghĩa này? Định nghĩa về tập hợp chưa đủ dùng hay sao còn phải dùng nhóm? Nói chung là lúc đầu chẳng hiểu gì hết.

Điều đầu tiên tụi mình cần phải trả lời là định nghĩa về tập hợp chưa đủ dùng hay răn mà tụi mình cần phải dùng đến nhóm? Điểm khác biệt rõ ràng nhất là nhóm có luật hợp thành trong hay phép toán hai ngôi còn tập hợp thì không. Vậy tại sao tụi mình lại cần có luật hợp thành trong? Như những gì tụi mình đã biết về tập hợp là khi nói đến tập hợp là tụi mình chỉ gom các vật thể lại với nhau và không làm gì cả. Nhưng không làm gì cả thì không có gì vui rồi?

Thực tế, các phần tử trong tập hợp với nhau để tạo ra các phần tử khác, như  phân tử hidro "kết hợp" với phân tử oxi cho ra phân tử nước, bạn có một viên kẹo xin thêm một viên nữa thì bạn có hai viên kẹo =)), lắp động cơ vào khung xe tụi mình được một cái xe, vợ với chồng ở chung với nhau là được một gia đình, chắc các bạn đang tự hỏi là luật hợp thành trong là "kết hợp" hai phần tử trong cùng một tập hợp cho ra một phần tử ở trong tập hợp đó, nhưng "vợ", "chồng" và "gia đình" đâu có cùng thuộc một tập hợp?, điều này tuỳ thuộc vào tập hợp nào mà bạn xét, nếu tập hợp tụi mình xét là tập hợp các tập hợp con của tập hợp con người thì tập hợp có 1 phần tử là "vợ" hay "chồng" thuộc tập hợp đó, và gia đình là tập hợp hai phần tử là con người cũng thuộc tập hợp đó.

Và tụi mình vẫn thường thấy nhất là các phép cộng và phép nhân trong số học, số học là nền tảng của toán học, do đó, nếu không có phép cộng hay phép nhân sẽ không có số học và toán học ngày nay.

Vì vậy, tụi mình cần có luật hợp thành trong, và việc kết hợp một tập hợp cùng với một luật hợp thành trong cho tụi mình một nhóm. Điều này khẳng định với tụi mình lại rằng nhóm là một TẬP HỢP.

Nhưng nếu chỉ định nghĩa nhóm là một tập hợp cùng với một luật hợp thành trong thì có vẻ chưa đủ lắm. Vì luật hợp thành trong lấy hai phần tử thuộc tập hợp cho tụi mình biết kết quả là một phần tử trong tập hợp, nhưng nếu tụi mình cần một luật hợp thành trong mà kết hợp phần tử này với phần tử nào để được kết quả là phần tử đã biết thì sao?. Do đó luật hợp thành trong của tụi mình cần phải thoả mãn một vài điều kiện nữa.

Qua nghiên cứu, "con nhà người ta" cho tụi mình biết rằng luật hợp thành trong cần phải thoả mãn bốn tính chất là: **tính đóng**, **tính kết hợp**, **tính có phần tử trung hoà**, **tính có phần tử khả nghịch**

Các tính chất này nghĩa là sao? Tụi mình có thể nói dài hơn một tí là:

Cho tập hợp $$E$$ cùng với luật hợp thành $$* $$ trong nó

**Tính đóng**<br/>
Nếu $$a,b$$ thuộc $$E$$ thì $$a*b$$ thuộc $$E$$.

**Tính kết hợp**<br/>
Tính chất này thì tụi mình đã biết $$\forall (x,y,z) \in E^3, (x*y)* z = x*(y*z)$$.  

**Tính có phần tử trung hoà**<br/>
Tồn tại $$e$$ thuộc $$E$$ sao cho $$e$$ là phần tử trung hoà đối với $$* $$.

**Tính có phần tử khả nghịch**<br/>
MỌI phần tử thuộc $$E$$ đều khả nghịch đối với $$* $$. Phần tử y thuộc $$E$$ sao cho $$x \in E: x*y = e$$ thì y gọi là phần tử nghịch đảo của $$x$$ đối với $$* $$.<br/>
Tụi mình sẽ kí hiệu phần tử nghịch đảocủa $$x$$ là $$x^{-1}$$. Các bạn phân biệt phần tử nghịch đảo và phần tử có quan hệ ngược nhé.

Nhưng tại sao tụi mình lại cần các tính chất này? Tụi mình có thể xem một video trên kênh Socratica - Youtube để hiểu được lí do. Socratica cung cấp một series khá hay về Đại số trừu tượng (Abstract Algebra), các bạn có thể tham khảo.

<center><iframe width="560" height="315" src="https://www.youtube.com/embed/yHq_yzYZV6U" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe></center>

Nếu như các bạn đã hiểu vì sao một nhóm lại cần những tính chất đó, ở đây mình xin tổng quát lại ví dụ ở video trên. Như ở trên tụi mình cần một cách để xác định phần tử $$a$$ kết hợp phần tử $$x$$ nào ra phần tử $$b$$, và cách dễ nhất chính là giải phương trình $$a*x=b$$. Giả sử $$a$$, $$a^{-1}$$ và $$b$$ đã biết, từ các bước tìm nghiệm $$x$$, tụi mình sẽ biết được tụi mình cần những tính chất gì trong một nhóm.

$$a*x=b$$, $$\begin{cases} a \in E \\ x \in E \end{cases} \Rightarrow b \in E$$  (Tính đóng)

$$a^{-1}* (a*x)= a^{-1}* b$$, Phần tử khả nghịch

$$(a^{-1} * a)* x = a^{-1}* b$$, Tính kết hợp

$$e * x = a^{-1}* b$$, Có phần tử trung hoà

$$x = a^{-1}* b$$ Và đây là nghiệm

Vậy các tính chất tối thiểu để tụi mình có thể giải phương trình $$a*x=b$$ là tính đóng, tính có phần tử khả nghịch, tính kết hợp và tính có phần tử trung hoà.

Vậy định nghĩa của tụi mình ở trên có thoả mãn các tính chất này, tính đóng được thoả mãn theo định nghĩa của luật hợp thành trong và các tính chất còn lại đều được trình bày rõ ràng.

Định nghĩa ở trên là định nghĩa một cách chặt chẽ để tụi mình có thể dùng để chứng minh các định lí nhưng để cho ngắn gọn tụi mình có thể nhớ là

> Nhóm là tập hợp cùng với MỘT phép toán thoả mãn: đóng, kết hợp, khả nghịch, trung hoà.

**Chú ý**
- Luật hợp thành trong $$* $$ không nhất thiết phải là phép nhân trên tập hợp số.

- Luật hợp thành trong của một nhóm không nhất thiết phải có tính giao hoán, nếu có tính giao hoán thì nhóm đó được gọi là nhóm giao hoán hoặc nhóm Abel.

- Đôi lúc bạn sẽ nghe nói là nhóm có 1 hoặc 2 phép toán. Ví dụ trong tập hợp hợp số nguyên, tụi mình có phép cộng và phép trừ, nhưng thực ra phép trừ chỉ là phép cộng với số đối (phần tử nghịch đảo) nên cũng tính là phép cộng. Trong định nghĩa về nhóm tụi mình đã định nghĩa mọi phần tử đều khả nghịch nên không cần thiết phải thêm một phép toán như vậy. Do đó, hãy nhớ là nhóm sẽ là một tập hợp và MỘT phép toán.

- Mọi phần tử thuộc nhóm là phần tử chính quy hay khử được.<br/>
_Chứng minh_<br/>
Cho nhóm $$(G,* )$$<br/>
$$\forall (x,y,z) \in G^3$$, $$x*y = x*z \Rightarrow x^{-1}* (x*y) = x^{-1} * (x*z) \Rightarrow (x^{-1}* x ) * y = (x^{-1}* x)* z \Rightarrow e*y = e*z \Rightarrow y = z$$<br/>
Tương tự, $$y*x = z*x \Rightarrow y = z$$<br/>
Vậy tụi mình có điều phải chứng minh.

**Ví dụ**

Về phần ví dụ này, để đưa các ví dụ liên quan đến số học thì không khó, nhưng tụi mình cần thoát ra khỏi số học một chút vì nhóm là một công cụ mạnh và có ứng dụng không chỉ trong số học mà còn trong những lĩnh vực chuyên sâu khác. Nếu số học được ra đời trước công nguyên thì khái niệm về nhóm và đại số trừu tượng mới được phát triển từ thế kỉ 19 thì các bạn có thể biết được nhóm là công cụ "hiện đại" như thế nào. Nhóm có ứng dụng trong những lĩnh vực được coi là "đau đầu" như hoá học và khoa học vật liệu, thiên văn học, Vật lí, Đại số Topo, Hình học, ... Và khi học liên quan đến công nghệ thông tin, tụi mình sẽ gặp nhóm trong mật mã học (Cryptography), lí thuyết đồ thị (Graph Theory),... Nhóm thường biểu diễn một cấu trúc có tính tuần hoàn hoặc đối xứng.

- Tập hợp số nguyên là một nhóm đối với phép cộng. Tập hợp số tự nhiên không là một nhóm đối với phép cộng.

- Cho một hình vuông cùng với các đỉnh được đánh thứ tự, phép xoay hình vuông quanh tâm của nó tạo nên các vị trí mới, tập hợp các vị trí của hình vuông cùng với phép xoay cho tụi mình một nhóm

- Phép lật một tờ giấy và phép tạo giữ nguyên tờ giấy tạo thành một nhóm.

- Tập hợp các song ánh $$E \rightarrow E$$ cùng với phép hợp ánh xạ tạo thành một nhóm.

- Một mặt phẳng là một nhóm đối với phép cộng hai vector.

- Xét một quả táo trên bàn, tập hợp các thao tác $$\{\text{bỏ quả táo trên bàn, giữ quả táo yên trên bàn, lấy quả táo ra khỏi bàn} \}) tạo thành một nhóm đối với phép "thực hiện thao tác này sau đó thực hiện thao tác kia".

- Xét trên biên giới đất liền Việt Nam, chọn một điểm xuất phát, cho là Đà Nẵng đi, bạn sẽ đi bộ, coi trong quá trình đi bạn không có quay đầu, thì tập hợp các thao tác "đi tới một số bước", "đi lùi một số bước" và "đứng yên" cho tụi mình một nhóm đối với phép "thực việc này trước sau đó tới việc kia". Chú ý tập hợp này là một tập hợp vô hạn.

Video từ Socratica sẽ cung cấp cho các bạn thêm một vài ví dụ nữa

<center><iframe width="560" height="315" src="https://www.youtube.com/embed/g7L_r6zw4-c" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe></center>

Và một kênh youtube nữa mình muốn chia sẻ với các bạn đó là Professor Macauley, kênh có các playlist tương đương với các khoá đại số và giải tích tụi mình các bạn có thể tìm xem. Sau đây là một video nói về một số ứng dụng của lí thuyết nhóm trên kênh này.

<center><iframe width="560" height="315" src="https://www.youtube.com/embed/oL15D_1Y0wk" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe></center>


# Nhóm con
Cho $$(G,* )$$ là một nhóm, $$H \in \mathfrak{P}(G)$$
> $$H$$ là nhóm con của $$G$$ khi và chỉ khi $$\begin{cases} \forall (x,y) \in H^2, x*y \in H \\ e \in H \\ \forall x \in H, x^{-1} \in H \end{cases}$$

Đây là những định nghĩa mà mình lấy từ giáo trình mà mình học, đây là những định nghĩa khá chặt chẽ, giúp tụi mình khi chứng minh các định lí. Nhưng để cho tụi mình có nhìn rõ vấn đề thì nói thật cũng phải mất một khoảng thời gian thì mình mới hiểu.

Nhóm con được hiểu theo nghĩa bao hàm nên tụi mình có thể định nghĩa một dễ hiểu hơn là

> Nhóm con = Tập hợp con và Nhóm

Có nghĩa là $$H$$ là một nhóm con của $$G$$ khi chỉ khi $$H$$ là tập hợp con của $$G$$ và $$H$$ là một nhóm.

Vậy định nghĩa ni có thoả mãn định nghĩa ban đầu không? Hãy xem nhé $$H \in \mathfrak{P}(G) $$ nên $$H$$ là tập hợp con của $$G$$. $$H$$ là một nhóm suy ra $$H$$ có tính đóng, kết hợp, trung hoà, khả nghịch. Tính đóng, trung hoà, khả nghịch đã được thể hiện ở trên. Vì với mọi $$x,y,z$$ thuộc $$G$$ tụi mình đều có tính kết hợp với $$* $$. Do đó, trong định nghĩa về nhóm con tụi mình không có đề cập tính kết hợp.

Tại sao tụi mình lại quan tâm đến nhóm con? Do tính đóng của nhóm, những gì "làm việc" trong nhóm sẽ "ở trong" nhóm. Do đó, khi làm việc với một nhóm lớn nếu có thể "chuyển" từ nhóm lớn sang nhóm "nhỏ hơn" giúp công việc của tụi mình sẽ đơn giản hơn, điều này cũng hoàn toàn tương tự đối với các cấu trúc mà tụi mình sẽ tụi sẽ tìm hiểu sau.

**Chú ý**
- Nhóm con vẫn là tập hợp, Nhóm con là một nhóm.

- Các tính chất đúng với nhóm thì đúng với nhóm con.

- Vì nhóm con là một tập hợp nên tụi mình có thể thực hiện phép giao hai nhóm con. Và giao của hai nhóm con là một nhóm con.<br/>
_Chứng minh_<br/>
Cho $$G$$ là một nhóm có luật hợp thành trong là $$* $$. Giả sử tụi mình $$H,K$$ là hai nhóm con của $$G$$.<br/>
Rõ ràng $$H \cap K$$ là tập hợp con của $$G $$.<br/>
Vì phần tử trung hoà $$e$$ đối với $$* $$ là duy nhất nên $$e\in H$$ và $$e \in K$$. Suy ra $$e \in H \cap K$$. (Tính có phần tử trung hoà)<br/>
Vì mọi phần tử trong một nhóm là khả nghịch nên $$x \in H \Rightarrow x^{-1} \in H$$, tương tự $$x \in K \Rightarrow x^{-1} \in K$$. Suy ra $$x \in H \cap K \Rightarrow x^{-1} \in H\cap K$$. (Tính có phần tử khả nghịch)<br/>
Do tính đóng của nhóm nên tụi mình có nếu $$\begin{cases} x \in H \\ y \in H \end{cases} \Rightarrow x*y \in H$$, tương tự, $$\begin{cases} x \in K \\ y \in K \end{cases} \Rightarrow x*y \in K$$. Nên $$\begin{cases} x \in H \cap K\\ y \in H\cap K \end{cases} \Rightarrow x*y \in H\cap K$$. (Tính đóng)<br/>
Vậy $$H\cap K$$ là một nhóm con của $$G$$.

**Ví dụ**
- Xét một điểm $$A$$ cố định trên một mặt phẳng, tập hợp các vector có gốc là $$A$$ nằm trên mặt phẳng cho tụi mình nhóm. Và tập hợp các vector gốc $$A$$ nằm trên một đường thẳng $$A$$ là một nhóm con.

- Tập hợp $$\{-1, 0, 1\}$$ không phải là nhóm con của nhóm các số nguyên $$\mathbb{Z}$$ đối với phép cộng thông thường vì không có tính đóng.

- Tụi mình có phép toán $$mod$$ là phép chia lấy dư trong tập số nguyên, ví dụ $$ 5 \, \text{mod} \, 2 = 1, 8 \, \text{mod} \,2 = 0$$. Tập hợp $$\mathbb{Z}$$ là một nhóm đối với phép "cộng rồi mod 2", và tập hợp $$\{0,1\}$$ là một nhóm con của $$\mathbb{Z}$$.

- Tập hợp $$\{0\}$$ là một con của nhóm các số nguyên đối với phép cộng thông thường.

- Vector không ở gốc toạ độ và các mặt phẳng đi qua gốc $$O$$ là các nhóm con của không gian vector có gốc toạ độ là  $$O$$. Chú ý sau này tụi mình sẽ biết không gian vector là một nhóm đối với phép cộng vector.

<br/>
Mình xin kết thúc bài viết tại đây, hi vọng các bạn có thể hiểu được nhóm là gì vì nhóm là một khái niệm cơ bản và là trung tâm của các lí thuyết toán học hiện đại, việc hiểu được nhóm giúp các bạn có thể hiểu được các khái niệm trừu tượng hơn sau này. Các bạn có phản hồi thì bình luận ở dưới nhé.

>Aim for the sky, but move slowly, enjoying every step along the way. It is all those little steps that make the journey complete - Chanda Kochhar


Ted
<br/>
<br/>

# Tham khảo

Đại số 1 - Jean-Marie Monier<br/>
Giáo trình Toán - Thầy Bùi Tuấn Khang<br/>
[Group Theory Introduction - brilliant.com](https://brilliant.org/wiki/group-theory-introduction/)<br/>
[Introduction to Groups - mathisfun.com](https://www.mathsisfun.com/sets/groups-introduction.html)<br/>
[Examples of group - Wikipedia](https://en.wikipedia.org/wiki/Examples_of_groups)<br/>
[Những kiến thức cơ bản về lí thuyết nhóm - vi.wikipedia.com](https://vi.wikipedia.org/wiki/Nh%E1%BB%AFng_ki%E1%BA%BFn_th%E1%BB%A9c_c%C6%A1_b%E1%BA%A3n_c%E1%BB%A7a_l%C3%AD_thuy%E1%BA%BFt_nh%C3%B3m)<br/>
[Why is group theory important? - University of Connecticut](http://www.math.uconn.edu/~kconrad/math216/whygroups.html)<br/>
[Abstract Algebra - Socratica](https://www.youtube.com/playlist?list=PLi01XoE8jYoi3SgnnGorR_XOW3IcK-TP6)<br/>
[Modern (Abstract) Algebra - scalenescott](https://www.youtube.com/channel/UCXOHGjg_XSGzPLkcqXs4lXg)<br/>
[Visual Group Theory - Professor Macauley](https://www.youtube.com/channel/UCH1cV4RtgI_N97M8jepiUzw/playlists)
