---
layout: post
title:  "Cấu trúc đại số - Vành, Thể, Trường"
subtitle: "Một vài cấu trúc đại số khác"
date:   2018-03-04
categories: [dai-so]
permalink:
cover:
description:
mathjax: true


---

# Mục tiêu

- ### Thể, Trường là gì?
- ### Vành là gì?

Chào các bạn, tụi mình đã cùng nhau tìm hiểu về nhóm, nôm na mà nói thì nhóm là một tập hợp được trang bị một luật hợp thành trong. Và trong bài viết này, tụi mình sẽ được biết về các cấu trúc đại số được trang bị hai luật hợp thành trong đó là : vành, thể, trường. Nhưng vì các cấu trúc đại số này được hiểu là tập hợp được trang bị hai luật hợp thành trong, tụi mình có thể để ý trước là: vành, thể, trường = nhóm + 1 phép toán = tập hợp + 2 phép toán.

# Thể, Trường là gì?

## Thể

Cho tập hợp $$K$$ cùng với hai luật hợp thành trong $$.$$ và $$+$$.

>Tập hợp $$K$$ gọi là thể khi và chỉ khi
$$\begin{cases} \text{K là một nhóm giao hoán đối với +} \\
K - \{0_K\} \,\,\text{là một nhóm đối với .}\\
0_K \neq 1_K \\
\text{. có tính phân phối với +} \end{cases} $$

Với $$0_K$$ là phần tử trung hoà của $$+$$ trong $$K$$. $$1_K$$ là phần trung hoà của $$.$$ trong $$K$$. Mọi người lưu ý là $$0_K$$, $$1_K$$ có thể không phải là một số.

Thật là dễ hiểu đối với định nghĩa này đúng không nào? Nó giống như tụi mình "cho" nhóm giao hoán $$K$$ thêm một luật hợp thành trong $$.$$ sao cho $$.$$ thoả mãn các tính chất của luật hợp thành trong một nhóm. Nhưng đây là lúc tụi mình cần đặt câu hỏi: Tại sao $$K$$ lại là nhóm giao hoán đối với $$+$$?, Tại sao $$.$$ lại có tính phân phối với $$+$$. Tụi mình có thể định nghĩa một thể mà không cần tính phân phối không?

Câu trả lời sẽ là tụi mình hoàn toàn có thể định nghĩa bất cứ khái niệm trong toán học nào nếu tụi mình muốn. Nhưng tụi mình chỉ cần những định nghĩa mà tụi mình sẽ gặp và làm việc với nó thôi như tập hợp số nguyên, số thực, ma trận, ...

Lấy ví dụ là tập hợp số thực, trên tập hợp số thực tụi mình có hai phép toán là $$+$$ và $$.$$, rõ ràng tập hợp số thực là một nhóm Abel đối với $$+$$. Đối với phép $$.$$, thì trong tập hợp $$\mathbb{R}$$, $$.$$ có tính kết hợp, có phần tử trung hoà là $$1$$, mọi phần tử khác $$0$$ thuộc $$\mathbb{R}$$ đều khả nghịch đối với $$.$$, phép $$. $$ có tính phân phối với phép $$+$$. Do đó tụi mình cần định nghĩa một cấu trúc có thể miêu tả tập hợp $$\mathbb{R}$$. Từ đó, tụi mình có định nghĩa về thể.

 Từ việc nghiên cứu các cấu trúc đại số, "con nhà người ta" đã rút ra những điểm chung trong các cấu trúc, và đưa ra định nghĩa về thể, và định nghĩa trên gọi là thể không giao hoán, vì trong chương trình học của mình không để cập đến thể không giao hoán nhiều nên mình không có nhiều ví dụ cho các bạn.

**Ví dụ**

&emsp; Tập hợp các ma trận vuông khả nghịch cùng với ma tra trận $$0$$ là thể không giao hoán đối với phép cộng và phép nhân ma trận.

Trong quá trình tìm hiểu ở đại học, tụi mình sẽ quan tâm nhiều hơn đến thể giao hoán hay còn gọi là trường.

## Trường
> Trường là thể giao hoán. Tức là $$.$$ có tính giao hoán.

Tuy thể không giao hoán thì tụi mình có rất ít ví dụ nhưng thể giao hoán hay trường lại là những thứ mà tụi mình rất quen thuộc. Đó là trường số thực, trường số hữu tỉ, trường số phức và trường phân thức hữu tỉ. Lưu ý: Trường vector không phải là trường theo định nghĩa của đại số (vì tụi mình không có phép toán giữa các vector trong trường này).

Tương tự với nhóm, tụi mình cũng có thể con và trường con, vì trường cũng là một thể nên tụi mình ở đây, sẽ nói về thể con.

### Thể con
>$$H$$ là thể con của thể $$K$$ khi và chỉ khi $$H$$ là tập hợp con của tập hợp $$K$$ và $$H$$ là một thể.

Đây là một định nghĩa giúp tụi mình có thể dễ dàng nhớ khi nói đến thể con. Để chứng minh một tập hợp là một thể thì tụi mình cần một định nghĩa chi tiết hơn, nhưng mình thấy điều đó là không cần thiết vì khi đưa quá thứ thì tụi mình sẽ không tập trung vào thứ gì cả. Trong thời gian học đại học, tụi mình chỉ cần biết thể và trường là gì thôi, khi nghiên cứu cao hơn về toán, thì tụi mình mới có điều kiện sử dụng các định nghĩa này nhiều hơn.


# Vành là gì?
> Tập hợp $$A$$ là một vành khi và chỉ khi: $$\begin{cases} (A, +) \,\,\text{là một nhóm giao hoán} \\
A \,\, \text{có phần tử trung hoà đối với} \,\, .  \\
. \,\, \text{có tính phân phối với} \,\, + \end{cases}$$

Nếu $$.$$ có tính giao hoán thì tụi mình có một **vành giao hoán**.

Vẫn câu hỏi cũ, tại sao tụi mình lại cần vành? Trước hết, tụi mình cần nhớ vành là một nhóm nên tất cả các tính chất của nhóm đều đúng cho vành. Vành là một nhóm đối với phép $$+$$, nhưng vành còn có một phép toán thứ hai là phép $$.$$, $$.$$ thoả mãn các tính chất của luật hợp thành trong một nhóm chỉ trừ một tính chất là mọi phần tử đều khả nghịch đối với $$.$$, nghĩ lại thì tụi mình đã gặp cấu trúc nào như thế này chưa? Đúng rồi, đó là tập hợp các số nguyên.

Do trên tập hợp số nguyên tụi mình chỉ cộng, trừ, nhân được nhưng chia thì chưa chắc được do đó, định nghĩa về vành có mô tả tập hợp số nguyên một cách tốt nhất.

Các bạn có thể để ý khi so sánh định nghĩa về vành với định nghĩa của thể thì thể khác vành ở điểm duy nhất đó chính là mọi phần tử của thể đều khả nghịch đối với $$.$$

Ngoài ví dụ về tập hợp số nguyên thì tụi mình có một số tập hợp là vành: tập hợp ma trận vuông với phép cộng và nhân ma trận, tập hợp đa thức với phép cộng và phép nhân đa thức,...

Tương tự với các cấu trúc khác, tụi mình muốn (nếu có thể) sẽ phân tích vành thành các vành con "nhỏ hơn" để dễ dàng hơn trong nghiên cứu và tính toán. Do đó, tụi mình cần đến khái niệm vành con.

Điều tụi mình cần lưu ý là các phần tử vành chưa chắc là khả nghịch, nhưng nếu một cấu trúc thoả mãn các điều kiện của một vành và tất cả các phần tử của cấu trúc đó khả nghịch thì cấu trúc đó vẫn là một vành. Do đó, thể là một vành nhưng vành không phải là một thể.

## Vành con
> Tập hợp $$B$$ là một vành con của vành $$A$$ khi và chỉ khi $$B$$ là tập hợp con của tập hợp $$A$$ và $$B$$ là một vành

Tương tự, định nghĩa về thể con, tụi mình không cần đi sâu vào định nghĩa chi tiết của vành con, mà chỉ cần biết thế nào là vành con là được rồi.

**Ví dụ**
- $$\mathbb{Z}$$ là vành con của vành $$\mathbb{Q}$$

- Tập hợp đa thức hệ số nguyên là vành con của vành đa thức hệ số thực

- Tập hợp $$\mathbb{Z}/2\mathbb{Z}$$ là vành con của vành $$\mathbb{Z}/6\mathbb{Z}$$ với phép "cộng rồi mod 2" và phép "nhân rồi mod 2".

Tiếp đến một khái niệm "khá khó chịu" đó là Ideal của vành giao hoán.

## Ideal của một vành giao hoán
Cho $$(A,+, .)$$ là một vành giao hoán, $$I$$ là một tập con khác rỗng của $$A$$.
> $$I$$ là một ideal của $$A$$ khi và chỉ khi: $$\begin{cases} + \,\, \text{có tính đóng trong I}\\ \forall a \in A, \forall x \in I,\quad ax \in I \end{cases}$$

Để tìm hiểu về ideal, tụi mình xét một phần tử $$x \in I$$, thì suy ra $$ax \in I$$, điều này có nghĩa là $$I$$ chứa mọi phần tử "chia hết cho" $$x$$. Chú ý là không phải tất cả phần tử thuộc $$I$$ đều chia hết cho $$x$$.

Tại sao tụi mình lại quan tâm đến ideal? Tụi mình hoàn toàn có thể thấy từ định nghĩa của ideal liên quan đến "tính chia hết", tính chia hết ảnh hưởng đến việc tụi mình có thể phân tích một phần tử thành tích các phần tử khác. Nhưng việc phân tích này thì có ích gì? Việc phân tích một số thành tích các thừa số nguyên tố thì tụi mình đã quen thuộc, ở đây, tụi mình sẽ quan tâm việc phân tích một đa thức thành tích của các đa thức khác. Và nhờ việc phân tích này giúp tụi mình có thể tìm nghiệm của đa thức dễ dàng hơn.

Xét tập hợp các đa thức A, $$I$$ là ideal của A, giả sử $$x + 1$$ thuộc $$I$$, điều này suy ra $$(x+1)(x+2), (x+1)(x+3)(x+4) ...$$ thuộc $$I$$. Điều này cho tụi mình biết nếu một đa thức thuộc $$I$$ rất có khả năng nó có một thừa số nguyên tố là $$x+1$$.

Tuy nhiên, bây giờ, tụi mình chưa có đủ các công cụ để xét đến tập hợp các đa thức, nên sẽ nói tiếp về Ideal ở phần sau nhé.

<br/>
<br/>
Để kết thúc bài viết mình xin tổng hợp một chút xíu về vành, thể, trường nhé. Mình viết theo kiểu liệt kê như thế này, chắc các bạn đọc sẽ thấy chán và khó nhớ. Nhưng đây là các khái niệm cơ bản và được xây dựng dựa trên các tiên đề nên việc hiểu được vì sao thế này, vì sao thế kia sẽ rất khó khăn. Tuy nhiên, với mình, hiểu được thì mới làm được. Và mình muốn nói là các tập hợp số đã xuất hiện từ đây rất lâu rồi, và gần đây việc xuất hiện các khái niệm mới như tập hợp ma trận, tập hợp vector, tập hợp ánh xạ, ... Nên người ta mới nảy ra ý tưởng đưa khái niệm tổng quát cho các tập hợp trên, từ đó mà tụi mình có khái niệm cấu trúc đại số. Và do đó như việc xuất hiện tính phân phối trong định nghĩa về vành là do tụi mình cần nó để cho việc tính toán của mình dễ dàng hơn, hay lúc thì giao hoán lúc thì không đó là vì trong thực tế có những nhóm giao hoán và có những nhóm không giao hoán. Vì vậy, tụi mình nên nghĩ theo hướng này các tập hợp cùng với các phép toán là có trước rồi sau quá người mới tổng quát hoá lên thành các khái niệm về cấu trúc đại số, chứ không phải là tụi mình có cấu trúc đại số rồi từ đó mới xây dựng các tập hợp số tự nhiên, số nguyên, bla bla ...

Ok, vì những khái niệm về vành, thể, trường rất khó nhớ nhưng tụi mình cần nó để hiểu những khái niệm khác, nên phải có cách mà nhớ.

Tụi mình có thể các định nghĩa này dựa trên ví dụ của nó. Với vành, thì đó là tập hợp số nguyên, trong tập hợp số nguyên thì tụi mình có gì nào? Tập hợp số nguyên là một nhóm với phép cộng, không phải phần tử khác $$0$$ nào cũng khả nghịch với phép nhân. $$0 \neq 1$$. Phép nhân có tính phân phối với phép cộng và vậy là tụi mình có thể suy ra được định nghĩa về vành. Với thể và trường, thì tụi mình có thể nhớ tập hợp số thực, và cũng suy ra tương tự

Hoặc tụi mình cũng thể nhớ một cách ngắn gọi là vành thì tụi mình có thể "cộng, trừ, nhân" được. Với thể thì tụi mình có "cộng, trừ, nhân, chia" được. Các bạn chú ý nhé, theo định nghĩa về vành và thể thì tụi mình chỉ có hai phép toán thôi. Phép trừ ở đây tương đương phép cộng với phần tử đối hay nói các khác mọi phần tử đều khả nghịch với phép cộng. Tương tự với phép chia.

Hoặc là tụi mình cũng thể nhớ theo công thức là trường = 2 nhóm giao hoán, thể = trường - 1 giao hoán, vành = thể - 1 khả nghịch. Các bạn chú ý nhé, trường chỉ là một tập hợp, việc nói hai nhóm giao hoán ở đây có nghĩa nó là nhóm giao hoán đối với hai phép toán.

Tạm ổn rồi, hẹn các bạn ở bài viết sau nhé.

> Il vaut mieux faire que dire - Alfred de Musset

Ted

<br/>
<br/>
# Tham khảo

Đại số 1 - Jean-Marie Monier<br/>
Giáo trình Toán - Thầy Bùi Tuấn Khang<br/>
[Ring - Wikipedia](https://en.wikipedia.org/wiki/Ring_(mathematics))<br/>
[Field - Wikipedia](https://en.wikipedia.org/wiki/Field_(mathematics))<br/>
[Ideal - Wikipedia](https://en.wikipedia.org/wiki/Ideal_(ring_theory))<br/>
Abstract Algebra - Socratica Chanel<br/>
Abstract Algebra, an inquiry-based approach - J.K.Hodge, S.Schlicker, T.Sundstrom<br/>
Abstract Algebra - Dummit, Foote
