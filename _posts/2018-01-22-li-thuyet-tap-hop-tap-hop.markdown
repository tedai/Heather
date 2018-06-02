---
layout: post
title:  "Lí thuyết tập hợp - Tập hợp"
subtitle: "Những điều cần biết về tập hợp"
date:   2018-01-22
categories: [dai-so]
permalink:
cover:
description:
mathjax: true
---

# Mục tiêu

- ### Tại sao phải học về tập hợp
- ### Hiểu về tập hợp
- ### Quan hệ bao hàm của hai tập hợp
- ### Cặp có thứ tự và tích Descartes

<br/>
# Tại sao phải học về tập hợp?


Bây giờ tụi mình sẽ bắt đầu với khái niệm về tập hợp, tại sao lại là tập hợp? Lúc đầu mình cũng đặt câu hỏi như vậy, răn không học luôn tích phân, đạo làm luôn cho rồi? Giờ mình mới biết lí thuyết về tập hợp chính là nguồn gốc của mấy cái "lằng nhằng" sau này. Nó là nguồn gốc của mọi vấn đề nhưng chúng ta lại không hề có định nghĩa về nó :3, bọn mình chỉ biết là khi mình gom những cái gì đó lại một chỗ thì mình được một tập hợp.

Ví dụ: Tập hợp mấy con gà ở trong chuồng, danh sách người yêu cũ, bản thân mình cũng chỉ tập hợp của các tế bào, hay không khí đang thở là tập hợp của hơi nước, bụi, oxy, nitơ, hay làm việc về công nghệ thông tin thì dữ liệu chính là tập hợp của những thông tin, vân vân và mây mây.

Ngay cả trong ví dụ trong đời thường thì bọn mình cũng đã thấy được trường hợp tập hợp hữu hạn và tập hợp vô hạn phần tử như tập hợp mấy con gà ở trong chuồng là tập hợp hữu hạn, còn tập hợp không khí là tập hợp vô hạn vì bọn mình không thể biết được số nguyên tử, phân tử có trong không khí được, (và danh sách người yêu cũ có lẽ còn tuỳ thuộc từng người để là tập hợp hữu hạn hay vô hạn =))). Đưa ra các ví dụ trên có thể ít liên quan đến toán học nhưng là để các bạn có thể tưởng tượng được những thứ xung quanh và chính bản thân chúng ta đều là những tập hợp, nên tập hợp rất cần khi làm việc trong đời sống thực tế.

Và vì sao tập hợp là nguồn gốc của mấy cái "lằng nhằng"?. Từ khái niệm tập hợp, bọn mình có thể xây dựng được nhiều khái niệm khác. Ở cấp học phổ thông bọn mình có học về tập hợp các số tự nhiên, số nguyên, số hữu tỉ,... Nhưng nếu viết là "tập hợp", như tụi mình đã nhắc đến ở trên, thì tụi mình sẽ gom mấy cái số nớ lại với nhau thôi chứ chưa cộng trừ nhân chia gì trong đó được.

Do đó, khi lên đại học, để chính xác hơn, bọn mình có khái niệm về các cấu trúc đại số: nhóm, vành, thể, không gian,... nhưng chúng ta nên nhớ một điều là bản chất các cấu trúc đại số đó vẫn chỉ là TẬP HỢP, mà khi đến tập hợp thì đó khái niệm khá quen thuộc và đơn giản đúng không nên các khái niệm khác sẽ đơn giản thôi.

Theo như mình thấy, nhiều bạn và kể cả bản thân mình có một định kiến là tập hợp chỉ là tập hợp của các số, có lẽ vì lúc cấp ba học nhiều nên giờ tạo thành thói quen. Tập hợp có thể chứa bất thứ gì, vì đã nói trong thực tế nên mình sẽ lấy các ví dụ về toán học, đó có thể là tập hợp các hàm, các ma trận, vector, đường thẳng là tập hợp các điểm, đồ thị của một hàm là tập hợp các giá trị của hàm đó, tập hợp các biến, các nghiệm, ... và ta cũng có cả khái niệm tập hợp của tập hợp như mặt phẳng là tập hợp các đường thẳng và đường thẳng lại là tập hợp các điểm. Các khái niệm khác như quan hệ, ánh xạ, hàm đều được tạo nên từ tập hợp. Các khái niệm toán học đều quy về bản chất là tập hợp nên mình nghĩ chúng ta nên có một nền tảng vững chắc về lí thuyết tập hợp trước khi học tiếp những khái niệm khác.

<br/>
# Khái niệm tập hợp

>Tập hợp là một khái niệm nguyên thuỷ và không có định nghĩa về nó

Bắt tay vào tìm hiểu nào. Tụi mình không có định nghĩa về tập hợp mà chỉ có thể mô tả nó và xây dựng khái niệm tập hợp dựa trên một hệ các tiên đề, các bạn có thể tham khảo ở cuối bài. Một trong những khái niệm ban đầu của tập hợp mà tụi mình cần công nhận là _sự thuộc về_. Ta sẽ hiểu một tập hợp được tạo thành từ những thành phần riêng lẻ khác. Các thành phần riêng lẻ đó sẽ được gọi là _phần tử_ của tập hợp. Các phần tử của tập hợp sẽ được kí hiệu bằng các chữ cái in thường: a, b, x, y, ... và kí hiệu tập hợp bằng những chữ cái in hoa: A, B, C ...

Khi đó quan hệ thuộc về, "x là phần tử của A hay x thuộc A" sẽ được biểu diễn là: $$x \in A $$. Ngược lại, nếu "x không thuộc A" sẽ kí hiệu là $$x \notin A $$.

Tập hợp không có phần tử nào sẽ là tập hợp rỗng. Kí hiệu: $$ \varnothing $$.

<br/>
#  Quan hệ bao hàm

_Cho hai tập hợp $E,\, F $. $E$ bao hàm trong $F$ khi và chỉ khi tất cả những phần tử thuộc $E$ đều thuộc $F$. <br />
Khi đó kí hiệu $ E \subset F $_

>$ E \subset F \Leftrightarrow \forall x \in E, x \in F $

Ta còn thể nói $E$ là <i>bộ phận</i> của $F$ hoặc $E$ là <i>tập hợp con</i> của $F$. Kí hiệu tập hợp các tập hợp con của $E$ là
$ \mathfrak{P}(E) $.

Ví dụ: $$ E = \{ 1,2,3 \} \Rightarrow \mathfrak{P}(E) = \{\varnothing, \{1\}, \{2\},\{3\}, \{1,2\}, \{2,3\},\{3,1\},\{1,2,3\}\} $$.

Từ đây ta có tiên đề về sự mở rộng (The axiom of extension), nôm na là định nghĩa hai tập bằng nhau.

<br/>
# Tiên đề về sự mở rộng (The axiom of extension)

_Hai tập hợp bằng nhau nếu và chỉ nếu chúng có cùng các phần tử_
>$E = F \Leftrightarrow (\forall x, x \in E \Leftrightarrow x \in F) $

Ta viết lại mệnh đề nhờ vào quan hệ bao hàm là $E = F \Leftrightarrow ( E\subset F \wedge F \subset E)$.

Tiên đề này giúp chúng ta định nghĩa quan hệ bằng nhau giữa hai tập hợp. Tại sao lại gọi là "extension"? Theo tham khảo sách và theo cách mình nghĩ thì ta có thể phát biểu lại tiên đề trên là: "Một tập hợp sẽ chỉ được định nghĩa nhờ vào các phần tử của nó mà không phải dựa vào khái niệm tạo thành nó". "Sự mở rộng" ở đây có thể hiểu là các phần tử của tập hợp. Tại sao phải phức tạp thế này? Lấy một ví dụ cho đỡ "nóng đầu" đã.

Ví dụ: Nam và Thành có cùng bạn gái tên là Lan. Nếu coi Nam và Thành là những tập hợp thì ta coi Lan "thuộc về" Nam thì tập hợp Nam sẽ là {Lan}, tương tự, Lan "thuộc về" Thành thì tập hợp của Thành cũng sẽ là {Lan}. "Tập hợp" Nam và Thành sẽ "bằng nhau" vì có cùng phần tử là "Lan". Nếu mình coi sự "bằng nhau" ở đây là sự "bằng nhau" về tính cách, tuổi tác, xương thịt, vân vân và mây mây của Nam và Thành thì rõ ràng là Nam và Thành không bằng nhau.


Ví dụ khác: Nếu các bạn đã học về lập trình hướng đối tượng, cụ thể là Java chắc sẽ quen thuộc với ví dụ này. Khi xét sự "bằng nhau" giữa các đối tượng, nếu coi đối tượng là tập hợp các thông tin của nó, thì rõ ràng hai đối tượng có cùng thông tin sẽ bằng nhau. Nhưng nếu muốn xét 2 đối tượng đó có phải là cùng một thực thể (instance) không thì việc cùng thông tin là chưa đủ.


Do đó, tiên đề trên muốn nói là khi xét sự bằng nhau của tập hợp ta chỉ quan tâm đến các phần tử của tập hợp đó chứ không quan tâm tập hợp đó là gì.


<br/>
# Tiên đề về sự định rõ (The axiom of specification)

_Với mọi tập hợp $E$ và với mọi điều kiện $P(x) $ thì sẽ có tương ứng một tập hợp $F$, mà những phần tử của tập hợp $F$ chính là những phần tử $x$ thoả mãn điều kiện $P(x)$ của tập hợp $E$. $$ F= \{  x \in E : P(x) \} $$_

<br/>
Tiên đề này giúp ta có một cách khác mô tả tập hợp thay vì phải liệt kê từng phần tử của tập hợp.

Ví dụ: $$A=\{1, 2, 3, 4, 5, 6\},\quad B=\{x : x \in A \wedge x = 2k+1, k \in \mathbb{N}\}=\{1,3,5\}$$

Một trong những ứng dụng của tiên đề trên là: Chứng minh không tồn tại một tập hợp nào bao gồm tất cả. Các bạn có thể tham khảo thêm trong sách "Naive Set Theory".


<br/>
# Hợp, Giao, Hiệu của các tập hợp

  Ở mục này, ta cho các tập hợp $A,B \in \mathfrak{P}(E)$ . Tập hợp $E$ được coi là tập hợp lớn nhất, tập hợp chứa tất cả các tập hợp. Rõ ràng quy ước này mâu thuẫn với tiên đề trên nhưng sẽ chấp nhận để dễ dàng làm việc với các tập hợp ở mục này, cũng như ở các bài viết sau. Từ tiên đề về sự định rõ, ta có thể định nghĩa được hợp, giao, hiệu của hai tập hợp, lưu ý rằng hợp, giao, hiệu của hai tập hợp vẫn là một tập hợp. <br />

  <strong>Hợp của A và B</strong> &emsp; $$A \cup B = \{x \in E : x \in A \vee x \in B \} $$ <br />
  <strong>Giao của A và B</strong> &emsp; $$A \cap B = \{x \in E : x \in A \wedge x \in B \} $$ <br />
  <strong>Hiệu của A và B</strong> &emsp; $$A - B = \{x \in E : x \in A \wedge x \notin B \} $$ <br />

  Từ hợp, giao, hiệu của 2 tập hợp ta hoàn toàn có thể mở rộng cho hợp, giao, hiệu của nhiều tập hợp.

  **Chú ý:** Hai tập hợp $F,G$ <strong>rời nhau</strong> khi và chỉ khi $F\cap G = \varnothing$

  <br/>
# Cặp có thứ tự và Tích Descartes của hai tập hợp

  Trước khi nói về cặp có thứ tự, ta hãy nói về "cặp không thứ tự". Cặp không thứ tự là gì? =)) Đã nói là cặp rồi đương nhiên là có 2 rồi, vậy một _cặp không thứ tự_ đơn giản là một tập hợp gồm có 2 phần tử và một cặp không thứ tự sẽ là $$\{x,y\}$$.
   Và cần nhớ lại là nãy giờ tụi mình khi nói về tập hợp vẫn chưa có khái niệm "thứ tự", vậy để định nghĩa được một _cặp có thứ tự_. Bọn mình sẽ tìm cách để "đánh đấu" được thứ tự của một tập hợp có hai phần tử. Và cách "đánh dấu" đơn giản là 'ghi nhớ' lại phần tử thứ nhất của cặp đó. Do đó, ta có định nghĩa về _cặp có thứ tự_ như sau: <br/>

## Cặp có thứ tự
> Cặp có thứ tự có định nghĩa từ tập hợp $$(x,y)=\{\{x\},\{x,y\}\}$$

À mà lưu ý nhé vì tập hợp không có tính thứ tự nên định nghĩa: $(x,y)=\{\{x,y\},\{x\}\}$ vẫn như nhau nhé.

Và để nổi bật tính 'thứ tự' của cặp có thứ tự, tụi mình sẽ đi chứng minh tính chất sau:

<center> $$ \forall x,y,x',y': (x,y)=(x',y') \Leftrightarrow \begin{cases} x=x' \\ y=y'\end{cases}  $$ </center>

Điều này có thể phát biểu là hai cặp bằng nhau khi và chỉ khi các phần tử tương ứng bằng nhau.


**Chứng minh**

$\Rightarrow$

$$(x,y) = (x',y') \Rightarrow \{\{x\},\{x,y\}\} = \{\{x'\},\{x',y'\}\} $$   (*)

Theo định nghĩa là hai tập hợp bằng nhau: Hai tập bằng nhau khi mọi phần tử của tập này thuộc tập hợp kia và ngược lại.

$$ (*) \Rightarrow \left[ \begin{align*}
\{x\} =  \{x'\} \, \, \mathrm {và} \, \, \{x,y\} = \{x',y'\} \\
\{x\} =  \{x',y'\} \, \,\mathrm{và}\, \, \{x,y\} = \{x'\}
\end{align*}\right.$$


&emsp;Nếu $$ \{x\} = \{x'\} \Rightarrow x = x',\, \{x',y'\} = \{x,y\} \Rightarrow \{x',y'\} = \{x',y\} \Rightarrow y'=y$$.


&emsp;Nếu $$ \{x\} =\{x',y'\} $$, tới đây chắc một số bạn sẽ thấy tập hợp có một phần tử răn mà bằng tập hợp có hai phần tử, nhưng cứ theo định nghĩa về hai tập hợp bằng nhau, ta suy ra:

$$ x' \in \{x\} \, \,\mathrm{và}\, \, y' \in \{x\} \Rightarrow x = x' \, \,\mathrm{và}\, \,x = y' $$


Tương tự

$$ \{x,y\} = \{x'\} \Rightarrow x' = x \wedge x' = y $$

<br/>
$$ \begin{cases} x = y' \\ x' = x \end{cases} \Rightarrow y' = x', \,\begin{cases} y' = x' \\ x' = y \end{cases} \Rightarrow y'=y $$


Như vậy, điều kiện cần của mệnh đề trên đã được chứng minh.

Điều kiện đủ là hiển nhiên khi $x = x' \, \,\mathrm{và}\, \, y = y'$. Như vậy tính chất đặc trưng của cặp có thứ tự đã được chứng minh.


Dựa vào những nguyên tắc trên tụi mình hoàn thành có thể định nghĩa được <i>bộ-n có thứ tự</i> dựa trên định nghĩa về cặp có thứ tự.


Ví dụ: Trong trường hợp <i> bộ ba có thứ tự</i>, $$(x,y,z) =(x,(y,z))= \{\{x\},\{\{x\},(y,z)\}\} =  \{\{x\},\{\{x\},\{\{y\},\{y,z\}\}\}\} $$

Và <i>bộ-n</i> cũng có tính chất tương tự như trên của cặp.


Từ việc định nghĩa được <i>cặp có thứ tự</i>, tụi mình đi đến định nghĩa về <i>Tích Descartes của hai tập hợp</i>. <br/><br/>


## Tích Descartes của hai tập hợp

> $E,\,F$ là hai tập hợp. Tích Descartes của E và F là:  &emsp;$$E \times F = \{(x,y) : x \in E \wedge y \in F \} $$

**Lưu ý:** Trong trường hợp $F = E$, ta có thể viết: $E \times E = E^2$.

Và chúng ta cũng để ý rằng tích Descartes của hai tập hợp vẫn là một tập hợp của các cặp có thứ tự. Từ định nghĩa, tụi mình có thể thấy tích Descartes giúp tụi mình lấy ra từng cặp tương ứng giữa hai tập hợp.

Tích Descartes cho n tập hợp: $$E_1 \times E_2 \times ... \times E_n = \{(x_1,x_2,...,x_n) : x_1 \in E_1, ..., x_n \in E_n\}$$

Vậy tại sao lại tụi mình lại cần định nghĩa về cặp và tích Descartes? Do hai khái niệm đó sẽ giúp tụi mình hiểu được khái niệm về quan hệ, sau đó là hàm và ánh xạ. Đây là những khái niệm quan trọng và cũng là những khái niệm hay bị thầy cô "hỏi lại" nhiều nhất =)).

<br/>
Ted
<br/>
# Tham khảo

Đại số 1 - Jean-Marie Monier <br/>
Giáo trình toán - thầy Bùi Tuấn Khang<br/>
Naive Set Theory - Paul R. Halmos<br/>
Elements of Set Theory - Herbert B. Enderton<br/>
Hệ các tiên đề về tập hợp: Zermelo–Fraenkel set theory - Wikipedia
