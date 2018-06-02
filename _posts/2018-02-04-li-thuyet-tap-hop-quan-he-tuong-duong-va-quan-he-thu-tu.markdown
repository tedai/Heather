---
layout: post
title:  "Lí thuyết tập hợp - Quan hệ tương đương và quan hệ thứ tự"
subtitle: "Hai loại quan hệ phổ biến"
date:   2018-02-4
categories: [dai-so]
permalink:
cover:
description:
mathjax: true


---

# Mục tiêu

- ### Hai loại quan hệ phổ biến
- ### Quan hệ tương đương
- ### Quan hệ thứ tự

<br/>

# Hai loại quan hệ phổ biến

Như trong bài viết về quan hệ, tụi mình đã biết các tính chất có thể có của một quan hệ là: phản xạ, đối xứng, phản đối xứng và bắc cầu. Vậy, bây giờ tụi mình sẽ cùng nhau tìm hiểu về hai loại quan hệ phổ biến: quan hệ tương đương và quan hệ thứ tự. Tại sao hai quan hệ này lại phổ biến? Từ đầu đến giờ, tụi mình đã liên tục nhắc lại một thứ đó là: Tập hợp. Mọi thứ tụi mình làm việc xung quanh đều là tập hợp đúng không nào? Tập hợp có thể là tập hợp số, hàm số, tập hợp quần áo, tập hợp nhân viên trong một công ty, ... Và để nguyên các tập hợp như vậy thì tụi mình vẫn chưa "làm việc" được gì đúng không nào? Để làm việc được thì tụi mình phải định nghĩa các "phép toán" : cộng, trừ, nhân, chia, ... chi đó, điều này tụi mình sẽ cùng nhau nhắc đến sau ở phần các cấu trúc đại số. Thay vào đó, trước tiên, trong toán học, cũng như các công việc hằng ngày, tụi mình cần phải biết cách "phân loại", "sắp xếp", để công việc của tụi mình có thể thực hiện được và thực hiện có hiệu quả.

Để có thể thực hiện được "phép cộng" trên tập hợp số tự nhiên, tụi mình phải sắp xếp các số tự nhiên lên trên một "tia số" hay "trục số", rồi việc thực hiện "phép cộng" chỉ là việc "dịch chuyển" vị trí trên "trục số" đó thôi. Ví dụ: để thực hiện "phép cộng" 0 với 1 trên tập hợp các số tự nhiên thì tụi mình chỉ cần dịch chuyển từ vị trí 0 lên 1 đơn vị trên trục số. Do đó, tụi mình có thể thấy, nếu không "sắp xếp" các số tự nhiên trên "trục số" thì lỡ 2 ở vị trí của 1 thì "phép cộng" 0 + 1 sẽ trở thành 0 + 1 = 2.

Hay công việc hằng ngày, tụi mình cũng phải "sắp xếp" các công việc theo một "thứ tự" ưu tiên, hay phân loại quần áo, loại nào mặc ấm, loại nào mặc đi chơi ...

Khi thực hiện "phân loại" hay "sắp xếp" tụi mình đều cần có các loại quan hệ như quan hệ tương đương và quan hệ thứ tự. Đương nhiên, trong cuộc sống hằng ngày, tụi mình không cần phải hiểu đến mức "cặn kẽ" các khái niệm toán học thì mới có thể "sắp xếp" hay "phân loại" được công việc của tụi mình. Nhưng việc hiểu các khái niệm này sẽ hiểu thấu đáo được các nguyên lí làm việc trong các vấn đề kĩ thuật sau này và cũng giúp tụi mình suy nghĩ một cách có logic hơn.

Vậy, hãy xem thử quan hệ tương đương và quan hệ thứ tự là gì nhé.

<br/>

# Quan hệ tương đương

> Quan hệ tương đương $$\mathcal{R}$$ là một quan hệ hai ngôi "đồng nhất" trên tập hợp F và có các tính chất: phản xạ, đối xứng, bắc cầu.

**Ví dụ**

- Quan hệ bằng nhau là quan hệ tương đương trong tập hợp các số tự nhiên. Vì:
  - Có tính phản xạ: $$\forall x \in \mathbb{N} : x = x$$
  - Có tính đối xứng: $$\forall (x,y) \in \mathbb{N}^2 : x = y \Rightarrow y = x$$
  - Có tính bắc cầu: $$\forall (x,y,z) \in \mathbb{N}^3 : x = y \, \text{và}\, y = z \Rightarrow x = z$$

<br/>
- Quan hệ song song trong tập hợp các đường thẳng thuộc cùng một mặt phẳng $$D$$ là quan hệ tương đương. Vì:
  - Có tính phản xạ: $$\forall a \in D : a \parallel a $$
  - Có tính đối xứng: $$\forall (a,b) \in D^2 : a \parallel b \Rightarrow b \parallel a $$
  - Có tính bắc cầu: $$\forall (a,b,c) \in D^3 : a \parallel b \, \text{và}\, b \parallel c \Rightarrow a \parallel c $$

<br/>
- Quan hệ "ở trong cùng một gia đình" trong tập hợp loài người H là quan hệ tương đương. Vì:
  - Có tính phản xạ: $$\forall a \in H : a \,\text{ở trong cùng một gia đình với}\, a $$. Ví dụ: Lan ở trong cùng một gia đình với Lan.
  - Có tính đối xứng: $$\forall a \in H^2 : a \,\text{ở trong cùng một gia đình với}\, b \Rightarrow b \,\text{ở trong cùng một gia đình với}\, a $$
  - Có tính bắc cầu: $$\forall (a,b,c) \in H^3 : a \,\text{ở trong cùng một gia đình với}\, b \quad \text{và}\quad b \,\text{ở trong cùng một gia đình với}\, c \Rightarrow a \,\text{ở trong cùng một gia đình với}\, c $$
<br/>

**Chú ý**

- Trong bài viết này, tụi mình sẽ chỉ nói về định nghĩa quan hệ tương đương, quan hệ thứ tự, các quan hệ này có tính chất như thế nào, chứ không phải là thực hiện việc "so sánh" hay "phân loại" các phần tử. Khi thực hiện việc "so sánh", tụi mình cần phải có một "tiêu chuẩn" nào đó.
<br/>
<br/>
Trong cuộc sống hằng ngày, khi "so sánh" mức độ quan trọng của một công việc, tụi mình có thể dựa vào tiêu chuẩn là khoảng cách thời gian từ bây giờ đến thời hạn. Nếu khoảng thời gian từ bây giờ đến thời hạn của công việc này ngắn hơn khoảng thời gian từ bây giờ đến thời hạn của công việc kia thì công việc này sẽ "quan trọng hơn" công việc kia.
<br/><br/>
Hay khi hai số tự nhiên với nhau chính là tụi mình đang dựa vào khoảng cách từ vị trí của mỗi số đến điểm số 0. Hay trong việc phân loại các bài viết trong vào chủ đề, tụi mình sẽ dựa vào "tiêu chuẩn" là "độ liên quan" của mỗi bài viết đến các chủ đề. Quan hệ "ở trong cùng một chủ đề" là quan hệ tương đương dựa trên "tiêu chuẩn" là độ liên quan" của mỗi bài viết đến các chủ đề.
<br/><br/>
Trong toán học, tụi mình cũng có các tiêu chuẩn như vậy, được gọi dưới cái tên là "chuẩn". Khái niệm "chuẩn" tụi mình sẽ cùng nhau nói ở những phần tiếp theo. Khi đi sâu vào kĩ thuật, các bạn sẽ có thể định nghĩa các "chuẩn" của riêng mình để cho công việc được hiệu quả hơn.
<br/>
<br/>
<br/>

Tiếp theo, bây giờ tụi mình có tập hợp và các phần tử của nó, cùng với quan hệ hai ngôi đồng nhất được định nghĩa trên tập hợp đó. Khi làm việc với phần tử $$x$$ của tập hợp, sẽ có lúc tụi mình cần xem những phần tử nào có quan hệ với x. Để biết một số nào đó có  chia hết cho 3 hay không trong tập hợp các số tự nhiên, tụi mình sẽ quan tâm đến tập hợp các số có quan hệ "là bội" đối với 3. Hay trong tập loài người, nếu tổ chức nào đó muốn làm việc với bạn, ví dụ như trường học, chẳng hạn, thì có thể họ sẽ quan tâm đến tập hợp những ai có quan hệ "trong cùng gia đình" với bạn. Hay bạn có bao giờ quan tâm đến tập hợp những ai có quan hệ "là người yêu thương, lo lắng" cho bạn? Vì nhu cầu trên, tụi mình sẽ có khái niệm về lớp tương đương.

<br/>
## Lớp tương đương
> $$\mathcal{R}$$ là một quan hệ hai ngôi "đồng nhất" trong tập hợp $$F$$. Với mọi $$x$$ thuộc $$F$$, lớp tương đương của $$x$$ là tập hợp, kí hiệu: $$cl_\mathcal{R}(x)$$ được xác định bởi:
> ## $$cl_\mathcal{R}(x) = \{ y \in E; x \mathcal{R} y \}$$

Hiểu là tập hợp các phần tử có quan hệ với $$x$$.
<br/>
**Chú ý**
- $$\mathcal{R}$$ là một quan hệ hai ngôi "đồng nhất", không nhất thiết là quan hệ tương đương.
- Tụi mình biết $$x$$ là gì thì mới định nghĩa được tập hợp trên. Hay lớp tương đương được xác định với mỗi $$x$$.
- Cái này lúc mình hay bị lẫn lộn, mọi người chú ý quan hệ tương đương khác với toán tử tương đương $$\Leftrightarrow$$.
<br/>

**Ví dụ**
- Cho một quan hệ tương đương $$\mathcal{R}$$ có đồ thị $$\Gamma = \{(a,a), (b,b), (c,c), (b,c), (c,b)\}$$ định nghĩa trong tập hợp $$F=\{a,b,c\}$$, có thể ban đầu sẽ hơi thắc mắc vì sao quan hệ trên là quan hệ tương đương?
<br/>
Thứ nhất, quan hệ trên là quan hệ hai ngôi đồng nhất vì đồ thị của nó là tập hợp các cặp có thứ tự.
Thứ hai, quan hệ trên có các tính chất: phản xạ, đối xứng, bắc cầu.<br/>
Tính phản xạ: $$\forall x \in F, x\mathcal{R}y$$, vì các cặp $$(a,a), (b,b), (c,c) \in \Gamma$$ suy ra $$a\mathcal{R}a,\,b\mathcal{R}b,\,c\mathcal{R}c$$.
<br/>
Tính đối xứng: $$\forall (x,y) \in F^2, x \mathcal{R}y \Rightarrow y\mathcal{R}x$$, vì dựa vào đồ thị $$\Gamma$$, ta thấy:
<br/> $$a \mathcal{R}a \Rightarrow a\mathcal{R}a$$ vì $$(a,a) \in \Gamma$$
<br/> $$b \mathcal{R}b \Rightarrow b\mathcal{R}b$$ vì $$(b,b) \in \Gamma$$
<br/> $$c \mathcal{R}c \Rightarrow c\mathcal{R}c$$ vì $$(c,c) \in \Gamma$$
<br/> $$b \mathcal{R}c \Rightarrow c\mathcal{R}b$$ vì $$(b,c), (c,b)\in \Gamma$$
<br/> Chắc sẽ có bạn thắc mắc vì sao không có $$a\mathcal{R}b$$ - ban đầu, mình cũng từng thắc mắc - điều này đơn giản là vì $$(a,b) \notin \Gamma$$
<br/>
Tính bắc cầu:
<br/> $$ c \mathcal{R} b \, \text{và}\, b \mathcal{R} c \Rightarrow c \mathcal{R} c $$. Do $$(c,b), (b,c), (c,c) \in \Gamma$$
<br/> $$ b \mathcal{R} c \, \text{và}\, c \mathcal{R} b \Rightarrow b \mathcal{R} b$$. Do $$(b,c), (c,b), (b,b) \in \Gamma$$
<br/>
Vậy $$\mathcal{R}$$ là quan hệ tương đương trong $$F$$.
<br/>
Tụi mình có, đối với $$a$$, tập hợp các phần tử thuộc $$F$$ có quan hệ $$\mathcal{R}$$ với $$a$$ là $$\{a\}$$. Suy ra, $$cl_\mathcal{R}(a)=\{a\}$$.
<br/> đối với $$b$$, tập hợp các phần tử thuộc $$F$$ có quan hệ $$\mathcal{R}$$ với $$b$$ là $$\{b,c\}$$. Suy ra, $$cl_\mathcal{R}(b)=\{b,c\}$$. Tương tự đối với $$c$$.
<br/>
<br/>
- Trong tập hợp loài người, thì mỗi gia đình là một lớp tương đương của một người đối với quan hệ "ở trong cùng một gia đình".
<br/>
<br/>
- Danh sách bạn bè trên Facebook của bạn là một lớp tương đương của bạn đối với quan hệ "là bạn bè trên Facebook"
<br/>
<br/>
- Danh sách crush của bạn là một lớp tương đương của bạn đối với quan hệ "là người thầm thương, trộm nhớ". Trong trường hợp này $$\mathcal{R}$$ chỉ là quan hệ hai ngôi.
<br/>
<br/>

## Tập thương
>Tập thương của E bởi $$\mathcal{R}$$, kí hiệu là $$E/\mathcal{R}$$, là tập hợp các lớp tương đương đối với quan hệ $$\mathcal{R}. $$
> ## $$ E/\mathcal{R}=\{cl_{\mathcal{R}}(x) : x \in E\}$$

**Ví dụ**
- Lấy ví dụ đầu tiên ở trên, tụi mình sẽ có $$E/\mathcal{R} = \{\{a\},\{b,c\}\}$$

**Chú ý**
- Đối với $$x,y$$ khác nhau và cùng thuộc một tập hợp $$E$$, $$\mathcal{R}$$ là quan hệ tương đương trong $$E$$, thì một là $$cl_\mathcal{R}(x) \cap cl_\mathcal{R}(y) = \varnothing$$ hoặc hai là  $$cl_\mathcal{R}(x) = cl_\mathcal{R}(y) $$
<br/><br/>
Chứng minh:
<br/>
Nếu $$cl_\mathcal{R}(x) \cap cl_\mathcal{R}(y) \neq \varnothing$$
<br/>
Giả sử: $$z \in cl_\mathcal{R}(x) \cap cl_\mathcal{R}(y) \Rightarrow  \begin{cases} x\mathcal{R}z \\ y\mathcal{R}z \end{cases} \Rightarrow \begin{cases} x\mathcal{R}z \\ z\mathcal{R}y  \end{cases} \Rightarrow x\mathcal{R}y $$. Do $$\mathcal{R}$$ là quan hệ tương đương.
<br/>
Với $$\forall t \in cl_\mathcal{R}(x) \Rightarrow x\mathcal{R}t \Rightarrow t\mathcal{R}x$$
<br/> Vì $$ \begin{cases} t\mathcal{R}x \\ x\mathcal{R}y \end{cases} \Rightarrow t\mathcal{R}y \Rightarrow y\mathcal{R}t \Rightarrow  t \in cl_\mathcal{R}(y)$$
<br/>
Vậy, $$\forall t \in cl_\mathcal{R}(x) \Rightarrow t \in cl_\mathcal{R}(y)$$ nên $$cl_\mathcal{R}(x) \subset cl_\mathcal{R}(y)$$
<br/>
Tương tự, cho chiều ngược lại, tụi mình chứng minh dược $$cl_\mathcal{R}(y) \subset cl_\mathcal{R}(x)$$
<br/>
Do đó, $$cl_\mathcal{R}(y) =  cl_\mathcal{R}(x)$$

<br/>
<br/>
Tiếp theo, tụi mình sẽ đến với loại quan hệ phổ biến thứ hai là quan hệ thứ tự. Quan hệ thứ tự RẤT quan trọng vì khi định nghĩa được "thứ tự" từ đó tụi mình mới có thể sắp xếp, thực hiện các công việc được hiệu quả, cũng như quan hệ thứ tự có ý nghĩa quan trọng trong việc hiểu các bài toán cực trị hay các bài toán tối ưu. Các bài toán quan trọng trong Machine Learning.


<br/>
<br/>
# Quan hệ thứ tự
> Quan hệ thứ tự $$\mathcal{R}$$ là một quan hệ hai ngôi "đồng nhất" từ tập hợp F và có các tính chất: phản xạ, phản đối xứng, bắc cầu.

**Chú ý**
- Quan hệ thứ tự thường được kí hiệu là $$\preceq$$ thay cho $$\mathcal{R}$$.

- Hai phần tử gọi là so sánh được khi có quan hệ thứ tự giữa hai phần tử này.

- Một tập hợp $$E$$ cùng với một quan hệ thứ tự $$\preceq$$ được định nghĩa trong nó tạo thành cặp $$(E, \preceq)$$ gọi là một tập hợp được sắp thứ tự.

- Vì các phần tử của tập hợp không nhất thiết phải là số, nên quan hệ thứ tự không nhất thiết phải mang nghĩa thứ tự thông thường như đối với các số. Thứ tự ở đây có thể có ý nghĩa về "gần - xa", "lớn - trẻ", "trước - sau", "trên - dưới", "giống - khác".

- $$\preceq$$ là một **quan hệ thứ tự toàn phần** khi và chỉ khi mọi phần tử của E đều so sánh được với nhau từng đôi.

**Ví dụ**
- Quan hệ $$\leq$$ thông thường trong tập hợp các số tự nhiên là quan hệ thứ tự toàn phần. Vì có:
  - Tính phản xạ. $$\forall x \in \mathbb{N}, x \leq x$$. Ví dụ: $$1 \leq 1$$
  - Tính phản đối xứng. $$\forall (x,y) \in \mathbb{N}^2, \begin{cases} x \leq y \\ y \leq x \end{cases} \Rightarrow x = y $$. Ví dụ: $$ a \leq 0 $$ và $$ 0 \leq a $$ suy ra $$a = 0$$.
  - Tính bắc cầu. $$ \forall (x,y,z) \in \mathbb{N}^3, \begin{cases} x \leq y \\ y \leq z \end{cases}  \Rightarrow x \leq z$$

<br/>
- Quan hệ bao hàm $$\subset$$ là quan hệ thứ tự không toàn phần trong $$\mathfrak{P}(E)$$ với E là tập hơp có nhiều hơn hai phần tử.
<br/>
Giả sử $$E=\{1,2\} \Rightarrow \mathfrak{P}(E)=\{\varnothing, \{1\}, \{2\}, \{1,2\}\}$$. Tụi mình có: $$\varnothing \subset \{1\}, \, \varnothing \subset \{2\}, \, \varnothing \subset \{1,2\}, \, \{1\} \subset \{1,2\}, \{2\} \subset \{1,2\}$$ nhưng $$\{1\} \not\subset \{2\}$$

<br/>
- Quan hệ "chia hết" là quan hệ thứ tự không toàn phần trong tập hợp các số tự nhiên.

<br/>
- Quan hệ "là hậu duệ" trong tập hợp con người không phải quan hệ thứ tự vì không có tính phản xạ thay vào đó nó được gọi là quan hệ thứ tự "nghiêm ngặt".

<br/>
- Quan hệ "đến sớm hơn" là một quan hệ thứ tự trong tập hợp là một hàng người đang chờ để mua hàng.

<br/>
- Quan hệ "xa hơn" dựa trên cách một điểm nào đó một bán kính $$R$$ là một quan hệ thứ tự không toàn phần. Vì các điểm trên cùng một mặt cầu không thể so sánh.

<br/>
- Quan hệ "tốt hơn" trên tập hợp các học sinh trong một lớp được khi học lực và hạnh kiểm của học sinh này đều "lớn hơn" học sinh kia là một quan hệ thứ tự không toàn phần nếu xảy ra trường hợp học lực của học sinh này "lớn hơn" học sinh kia nhưng hạnh kiểm của học sinh này lại "kém hơn" học sinh kia.
<br/> Đây là ví dụ về (quan hệ) thứ tự tích được định nghĩa như sau:
Cho $$(E,\preceq)$$,$$(F,\preceq')$$ là hai tập hợp được sắp thứ tự. $$\mathcal{P}$$ là quan hệ xác định trong $$E\times F$$ bởi:
<br/>
<center> $$(x,y)\mathcal{P}(x',y')\Leftrightarrow \begin{cases} x \preceq x' \\ y \preceq' y'  \end{cases}$$</center>

<br/>
- Quan hệ thứ tự xuất hiện các từ trong từ điển là quan hệ thứ tự. (Quan hệ) thứ tự này được gọi là thứ tự từ điển. Được dùng phổ biến trong từ điển =)), trong các bảng xếp hạng, để so sánh trong các chuỗi trong một ngôn ngữ lập trình nào đó người ta cũng dựa vào thứ tự này. Thứ tự từ điển được định nghĩa như sau, coi mỗi phần tử cần chỉ có 2 "chỉ số" để so sánh:
Cho $$(E,\preceq)$$,$$(F,\preceq')$$ là hai tập hợp được sắp thứ tự. $$\mathcal{L}$$ là quan hệ xác định trên $$E\times F$$ bởi:
<br/>
<center> $$(x,y)\mathcal{L}(x',y')\Leftrightarrow \Big\lbrack\begin{align} x \preceq x' \\ x = x' \, \text{và} \,y \preceq' y'  \end{align}$$</center>
<br/>
<br/>

Qua một loạt ví dụ vừa rồi, mình chỉ muốn nhấn mạnh quan hệ thứ tự ở đây không nhất thiết phải là quan hệ thứ tự thông thường giữa các số. Vì điều này làm mình luẩn quẩn một thời gian.

Bây giờ, mình nghĩ cái mà tụi mình khá quen thuộc đó chính là quan hệ thứ tự toàn phần. Cái rắc rối ở đây chính là quan hệ thứ tự không toàn phần. Vì như những ví dụ ở trên các bạn có thể thấy thứ tự không toàn phần khá phổ biến phải không nào? Thứ tự không toàn còn xuất hiện trong lí thuyết đồ thị có ứng dụng lớn trong việc giải quyết các bài toán phức tạp trong đời sống. Vì vậy, để làm việc, tụi mình cần thêm những khái niệm mới.

<br/>

## Các phần tử đặc biệt trong tập hợp được sắp thứ tự
Các bạn lưu ý nhé, hãy nắm thật rõ các khái niệm này vì tụi mình sẽ gặp nó liên tục.

<br/>Trong các định nghĩa sau, tụi sẽ coi $$(E, \preceq)$$ là một tập hợp được sắp thứ tự.

### Chặn trên và chặn dưới
#### Chặn trên

$$A\in \mathfrak{P}(E), x\in E$$. $$x$$ là một chặn trên hay cận trên của A trong $$E$$ khi và chỉ khi:
> ## $$\forall a \in A, a \preceq x $$

#### Chặn dưới

$$A\in \mathfrak{P}(E), x\in E$$. $$x$$ là một chặn dưới hay cận dưới của A trong $$E$$ khi và chỉ khi:
> ## $$\forall a \in A, x \preceq a $$

Tập hợp các chặn trên của $$A$$ trong $$E$$ là $$Maj_E(A)$$. Tập hợp các chặn dưới của $$A$$ trong $$E$$ là $$Min_E(A)$$. Các bạn nhớ các kí hiệu này vì sau này thay vì viết $$x$$ là cận trên của $$A$$ trong $$E$$, người ta hay viết $$x \in Maj_E(A)$$. Tương tự với cận dưới. Maj là từ viết tắt của "majorant" trong tiếng Pháp nghĩa là chặn trên, Min là từ viết tắt của "minorant" có nghĩa là chặn dưới.


Điều mình thắc mắc đầu tiên đó chính là tại sao không xét quan hệ thứ tự trên tập hợp $$E$$ luôn đi mà phải xét tới tập hợp con $$A$$ của $$E$$? Là do khi làm việc thì tụi mình chỉ làm việc với tập hợp con của một tập hợp lớn. Ví dụ: khi giáo viên muốn làm việc với lớp thì chỉ thường làm việc với ban cán sự lớp. Khi tìm từ "Hair" trong từ điển, tụi mình trong mục "H" ở đâu? hay cụ thể hơn là chữ đầu tiên bắt đầu bằng "H" và chữ cuối cùng kết thúc bằng "H" là ở vị trí nào.

<br/>

**Chú ý**
- $$A$$ là tập hợp con của $$E$$. $$A$$ bị chặn trên (tương ứng: bị chặn dưới) khi và chỉ khi A có ít nhất một chặn trên (tương ứng: chặn dưới) trong $$E$$.

- Để ý là $$x\in E $$ nên $$x$$ có thể có hoặc không thuộc $$A$$, điều này giúp tụi mình phân biệt được với các khái niệm tiếp theo là cực trị và phần tử lớn nhất, nhỏ nhất.

- Một tập hợp có thể có nhiều cận trên và cận dưới hoặc không có cận trên hoặc cận dưới nào.

<br/>
**Ví dụ**
- Coi Việt Nam là một hợp con trên Trái Đất. Chỉ xét theo chiều từ Bắc đến Nam thì những điểm có vĩ độ lớn hơn hoặc bằng tại Lũng Cú (cực bắc Việt Nam) là chặn trên của Việt Nam. Những điểm ở thấp hơn hoặc bằng về phía Nam đối với Mũi Cà Mau (cực Nam Việt Nam) là chặn dưới của Việt Nam.

<br/>
- Đặt một tờ giấy trên mặt bàn, coi tờ giấy là một tập hợp con của mặt bàn, xét quan hệ thứ tự dọc theo chiều dài tờ giấy, thì cận trên của tờ giấy là tất cả các điểm "nằm trên hoặc ở ngay" mép trên của tờ giấy, cận dưới của tờ giấy là tất cả các điểm "nằm dưới hoặc ở ngay" mép dưới tờ giấy.

<br/>
- Xét một hàng người như hình vẽ, xét quan hệ thứ tự từ phải sang trái, tập hợp gồm có {A,B,C,D} là tập con của hàng người trên. Tập hợp này có cận trên là A, và cận dưới là tất cả những người xếp sau D (tính cả D). (Cái hình chữ nhật coi như cái bàn thu ngân, vẽ thêm cho đẹp thôi nhé.)
<br/>
<svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="532px" version="1.1" content="&lt;mxfile userAgent=&quot;Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36&quot; version=&quot;8.0.6&quot; editor=&quot;www.draw.io&quot; type=&quot;google&quot;&gt;&lt;diagram id=&quot;805d03e9-44ca-ffee-f700-259b81aaff4c&quot; name=&quot;Page-1&quot;&gt;1ZdNj9owEIZ/TY5bxXE+4MjHtr1UWolD26NJhsSqE1PjLKG/vk4yISSGFVstKnAA+/V4Mn5m8IBDF3n1RbFt9k0mIBzPTSqHLh3Pm0wm5r0WDq0QEBRSxZNWIr2w4n8ARRfVkiewGxhqKYXm26EYy6KAWA80ppTcD802UgyfumUpWMIqZsJWv/NEZ3iswO31r8DTrHsycXFlzeJfqZJlgc9zPLppXu1yzjpfaL/LWCL3JxJ9duhCSanbUV4tQNRoO2ztvs8XVo9xKyj0NRsi6k/jKGbumiRrfxI9oYdXJkpkscRI9aGj05wPag+uQ+f7jGtYbVlcr+5NORgt07kwM2KGGy7EQgqpzLyQhTGaM8HTwkxjEySo2kYWGouA1i4xBlAaqosHI0dcpgpB5qDVwZjgBm+ChA/HFLXzfZ/PCKXsJJUhagwrKD167imaAYK8EqpnQV08JFQa3BFU34I6f0iovndHUAMLquOFQuPJB3DD36XsFp52DZOZMaDutuoXzSitP2edGxNR66nVb5+xj8jQ9I4yFJ7J0IghFMmsboI9lYTtsgYqGQKEiusfNetPLvFx/vNk7QUUNyHXIJd9uUNidc8RShOOLFUMbzUZG/cJzuAMzk5TIJjmr8MQzjHGJ7xI3pRu1xn8UTanozS1oeOu0945dkRGjqKRI81UCtpy1KT8eOx/q4LoEargv2X4Uu9/d4bd6duObphhYve3D78sx93sFpdnOGpvQWDdncQ7UwvWt+mK29NM+5/ObRL6vyf0+S8=&lt;/diagram&gt;&lt;/mxfile&gt;" onclick="(function(svg){var src=window.event.target||window.event.srcElement;while (src!=null&amp;&amp;src.nodeName.toLowerCase()!='a'){src=src.parentNode;}if(src==null){if(svg.wnd!=null&amp;&amp;!svg.wnd.closed){svg.wnd.focus();}else{var r=function(evt){if(evt.data=='ready'&amp;&amp;evt.source==svg.wnd){svg.wnd.postMessage(decodeURIComponent(svg.getAttribute('content')),'*');window.removeEventListener('message',r);}};window.addEventListener('message',r);svg.wnd=window.open('https://www.draw.io/?client=1&amp;lightbox=1&amp;edit=_blank');}}})(this);" viewBox="0 0 532 171" style="cursor:pointer;max-width:100%;max-height:171px;"><defs/><g transform="translate(0.5,0.5)"><rect x="71" y="55" width="70" height="60" fill="none" stroke="#000000" pointer-events="none"/><g transform="translate(94.5,67.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="22" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 22px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">D</div></div></foreignObject><text x="11" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">D</text></switch></g><rect x="141" y="55" width="70" height="60" fill="none" stroke="#000000" pointer-events="none"/><g transform="translate(164.5,67.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="22" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 22px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">C</div></div></foreignObject><text x="11" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">C</text></switch></g><rect x="211" y="55" width="70" height="60" fill="none" stroke="#000000" pointer-events="none"/><g transform="translate(235.5,67.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="20" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 22px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">B</div></div></foreignObject><text x="10" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">B</text></switch></g><rect x="281" y="55" width="70" height="60" fill="none" stroke="#000000" pointer-events="none"/><g transform="translate(305.5,67.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="20" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 22px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;"><font style="font-size: 30px">A</font></div></div></foreignObject><text x="10" y="23" fill="#000000" text-anchor="middle" font-size="12px" font-family="Helvetica">[Not supported by viewer]</text></switch></g><path d="M 72 115 L 1 115" fill="none" stroke="#000000" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="none"/><path d="M 71 55 L 0 55" fill="none" stroke="#000000" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="none"/><rect x="411" y="0" width="120" height="170" fill="none" stroke="#000000" pointer-events="none"/></g></svg>

- Hình ảnh ví dụ về cận trên, nguồn: Wikipedia
<p><a href="https://commons.wikimedia.org/wiki/File:Illustration_of_supremum.svg#/media/File:Illustration_of_supremum.svg"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/82/Illustration_of_supremum.svg/1200px-Illustration_of_supremum.svg.png" alt="Illustration of supremum.svg"></a></p>

- Một ví dụ về thứ tự không toàn phần. Đây là hình ảnh một cái cây, tụi mình sẽ cho cái cây một quan hệ thứ tự về độ cao, và mỗi nút trên cây có quan hệ thứ tự hay so sánh được khi chúng được nối với nhau như hình vẽ (các bạn có thể thấy không phải nút nào cũng có quan hệ thứ tự, cái đường thẳng ngang ở phía dưới hiểu là mặt đất nhé, chứ không có ý nghĩa gì nhiều đâu :v). Chiều của mũi tên chỉ chiều của quan hệ thứ tự. Từ hình vẽ, bạn có thể thấy,
  - Cận dưới của tập hợp $$\{6,7,8\}$$ là $$1, 6, 0$$ và tập hợp không có cận trên.
<br/>
  - Tập hợp $$\{6,7\}$$ có cận dưới là $$1, 6, 0$$, cận trên là tất cả các nút "lớn hơn" $$7$$
<br/>
  - Tập hợp $$\{0,1,7,8\}$$ không có cận trên và cận dưới.
><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="342px" version="1.1" content="&lt;mxfile userAgent=&quot;Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36&quot; version=&quot;8.0.6&quot; editor=&quot;www.draw.io&quot; type=&quot;google&quot;&gt;&lt;diagram id=&quot;805d03e9-44ca-ffee-f700-259b81aaff4c&quot; name=&quot;Page-1&quot;&gt;7ZrNcpswEICfxsd0AAkbHxM3aS+d6UwObY8Kkg1TjDxCju0+fUWQ+JHiGBhsjMnFYxaxQvvtSrsSE7BY778xtAl+UEyiiWPh/QR8nTiO53niNxUcMoFrS8GKhTgT2YXgOfxHpNCS0m2ISVJpyCmNeLipCn0ax8TnFRlijO6qzZY0qva6QStiCJ59FJnSXyHmgRyWaxXy7yRcBapn25J31kg1loIkQJjuSiLwOAELRinP/q33CxKltlN2yZ57OnI3fzFGYl7ngRmAc3/mI+vFxi/Qm93Z00zFK4q2crTyTflBDZ/E+D61oriKaSyEDwFfR+LKFn+XNOaSGLDEdfY0wYZFi1e084ELhyF0TTg7iCa7wrTKskHJqkrGSIR4+FpVjyThVa4u7+EnDUXHjiWdMdejfHFmVVUkdMt8Ip8qm1JT5M5PKOKIrQg3FIk/pWEXojdSdal5jaj5EUqS0P8YnGj/FEbqbiLenqvnqehHyUptrh01tDVCdkvUYFpVBKcXRD3vHnUduFV3GA1qCPtDrRaJmqgluLqcC88YNmpgaYTgAKNaDbsz1B/M3sfBXz1qbYkF3hBRO5+oa0zg+rzrDHECB92v1TeYlnWGWp8eLpiBO+4n6hao9WBsi9rwmXOiblYiS1QYJQHBklPdHE2W12XMpmNcO3TH62rVPpXpnRP6rBF0Ca4V9IHGdnfJ2UxTdMnYbraR0hDztSPMZ1FledAW4SlfOCfCZhskDREWU++txO3JrKl1+nXBuFWOep41eVjrLQRdAT2VmJ8TqFkl2wZRTva8Si7hjP4lCxpRVsT2UrDTRCgKV3GahwtkRMgfXgnjoY+ie3ljHWKcdvOwC0JOnjfIT/vcMbQRMka3MX5zHOvoLJ8qJPumHqIsb7kVy+fblyUPgu94kA6o7CwVOo1QmFWsGVy3iwJUUeQlSy8ooIECjAcFmGsoeo0Ks+CH40EBvSNLQy8ozILcHREKPe3qdYIyy2RvPCiAe00ozFJ2OiIUWinb77JtlqSz8aBw9MM22CMK2OygdaT79PoWXOuPovo8aIWt9uk/OQ+Os5lzWAbom51dgbZJ43qXm12hNXU9jKfzpQ2XgDh35qbNpSNOWI0dfqfm/iKKAHn9R5q/bjg6Vuaux5Zzt8+Y7ewM1dWP0/Td/tYxKy6LT5iz5sV34ODxPw==&lt;/diagram&gt;&lt;/mxfile&gt;" onclick="(function(svg){var src=window.event.target||window.event.srcElement;while (src!=null&amp;&amp;src.nodeName.toLowerCase()!='a'){src=src.parentNode;}if(src==null){if(svg.wnd!=null&amp;&amp;!svg.wnd.closed){svg.wnd.focus();}else{var r=function(evt){if(evt.data=='ready'&amp;&amp;evt.source==svg.wnd){svg.wnd.postMessage(decodeURIComponent(svg.getAttribute('content')),'*');window.removeEventListener('message',r);}};window.addEventListener('message',r);svg.wnd=window.open('https://www.draw.io/?client=1&amp;lightbox=1&amp;edit=_blank');}}})(this);" viewBox="0 0 342 295" style="cursor:pointer;max-width:100%;max-height:295px;"><defs/><g transform="translate(0.5,0.5)"><path d="M 0 257 L 340 257" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 157.88 194.88 L 114.5 151.5" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><ellipse cx="160" cy="197" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 110.79 147.79 L 118.22 150.27 L 114.5 151.5 L 113.27 155.22 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 161.54 194.43 L 186.72 152.46" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><ellipse cx="160" cy="197" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 189.42 147.96 L 188.82 155.76 L 186.72 152.46 L 182.82 152.16 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 56.04 129.01 L 107.15 146.05" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 51.06 127.35 L 58.81 126.25 L 56.04 129.01 L 56.59 132.89 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><ellipse cx="110" cy="147" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 137.76 72.96 L 111.05 144.19" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 139.61 68.05 L 140.43 75.83 L 137.76 72.96 L 133.87 73.37 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><ellipse cx="110" cy="147" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 190 113.37 L 190 144" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 190 108.12 L 193.5 115.12 L 190 113.37 L 186.5 115.12 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><ellipse cx="190" cy="147" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 192.12 104.88 L 235.5 61.5" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><ellipse cx="190" cy="107" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 239.21 57.79 L 236.73 65.22 L 235.5 61.5 L 231.78 60.27 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 192.34 145.13 L 235.03 110.98" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><ellipse cx="190" cy="147" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 239.13 107.7 L 235.85 114.8 L 235.03 110.98 L 231.47 109.34 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 30 67 L 49.05 124.15" fill="none" stroke="#000000" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="none"/><ellipse cx="50" cy="127" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 139.05 64.15 L 120 7" fill="none" stroke="#000000" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="none"/><ellipse cx="140" cy="67" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 170 17 L 140 67" fill="none" stroke="#000000" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="none"/><path d="M 240 54 L 240 7" fill="none" stroke="#000000" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="none"/><ellipse cx="240" cy="57" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 180 57 L 189.41 104.06" fill="none" stroke="#000000" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="none"/><ellipse cx="190" cy="107" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><g transform="translate(166.5,189.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="16" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 18px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">1</div></div></foreignObject><text x="8" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">1</text></switch></g><g transform="translate(196.5,139.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="16" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 18px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">2</div></div></foreignObject><text x="8" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">2</text></switch></g><g transform="translate(156.5,89.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="16" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 18px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">3</div></div></foreignObject><text x="8" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">3</text></switch></g><g transform="translate(241.5,99.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="16" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 18px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">4</div></div></foreignObject><text x="8" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">4</text></switch></g><g transform="translate(251.5,39.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="16" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 18px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">5</div></div></foreignObject><text x="8" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">5</text></switch></g><g transform="translate(111.5,39.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="16" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 18px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">8</div></div></foreignObject><text x="8" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">8</text></switch></g><g transform="translate(81.5,139.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="16" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 18px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">6</div></div></foreignObject><text x="8" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">6</text></switch></g><g transform="translate(21.5,119.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="16" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 18px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">7</div></div></foreignObject><text x="8" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">7</text></switch></g><path d="M 119.73 254.01 L 110.58 153.34" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><ellipse cx="120" cy="257" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 110.1 148.11 L 114.22 154.77 L 110.58 153.34 L 107.25 155.4 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 119.73 254.01 L 110.27 149.99" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><ellipse cx="120" cy="257" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="110" cy="147" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><g transform="translate(101.5,259.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="16" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 18px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">0</div></div></foreignObject><text x="8" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">0</text></switch></g><path d="M 192.34 145.13 L 237.66 108.87" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><ellipse cx="190" cy="147" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="240" cy="107" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/></g></svg>


<br/>
#### Biên trên
> Biên trên hay cận trên đúng là chặn trên thấp nhất.

Kí hiệu là $$Sup_E(A)$$ - Các bạn nhớ kí hiệu này nhé, hay quên lắm. Sup là từ viết tắt của từ Supremum trong tiếng anh và Borne Supérieure trong tiếng Pháp có nghĩa là biên trên.


#### Biên dưới
> Biên dưới hay cận dưới đúng là chặn dưới lớn nhất.

Kí hiệu là $$Inf_E(A)$$. Inf là viết tắt của từ Infimum trong tiếng anh và Borne Inférieure trong tiếng Pháp có nghĩa là biên dưới.

**Chú ý**
- Biên trên và biên dưới là duy nhất.

**Ví dụ**
- $$E = \mathfrak{P}(F)$$, $$F$$ là một tập hợp, quan hệ bao hàm $$\subset$$ là quan hệ thứ tự trong $$E$$. Với mọi $$(X,Y) \in E^2$$. <br/>
$$Sup_E(\{X,Y\}) = X \cup Y$$ và $$Inf_E(\{X,Y\}) = X \cap Y$$
<br/>
- Hình ảnh mình lấy trên wikipedia ở phía trên có thể hiện biên trên.
<br/>
- Ở ví dụ với cái cây ở trên, tập hợp $$\{6,7,7\}$$ có cận dưới nhưng không có cận dưới đúng.

<br/>
<br/>
## Phần tử lớn nhất, phần tử nhỏ nhất
### Phần tử lớn nhất
>$$A \in \mathfrak{P}(E)$$. $$x$$ là phần tử lớn nhất của $$A$$ khi và chỉ khi:
> ## $$\begin{cases} x \in A \\ \forall a \in A, a \preceq x  \end{cases}$$

### Phần tử nhỏ nhất
>$$A \in \mathfrak{P}(E)$$. $$x$$ là phần tử nhỏ nhất của $$A$$ khi và chỉ khi:
> ## $$\begin{cases} x \in A \\ \forall a \in A, x \preceq a  \end{cases}$$

**Chú ý**
- Để là phần tử lớn nhất hoặc nhỏ nhất thì $$x$$ phải là phần tử của $$A$$.

- Phần tử lớn nhất hoặc nhỏ nhất nếu tồn tại thì là duy nhất.<br/>
Chứng minh: <br/>
$$A \in \mathfrak{P}(E)$$. Cho $$x, x'$$ là hai phần tử nhất của $$A$$. Suy ra, $$x, x'$$ đều thuộc $$A$$ và $$x, x'$$ "lớn hơn hoặc bằng" tất cả các phần tử thuộc A. Nên $$\begin{cases} x \preceq x' \\ x' \preceq x \end{cases} \Rightarrow x = x'$$ (tính chất phản đối xứng).

- Khi cận trên đúng hoặc cận dưới đúng thuộc $$A$$ thì chúng sẽ là phần tử lớn nhất hoặc phần tử nhỏ nhất của $$A$$ theo như định nghĩa về phần tử lớn nhất và phần tử nhỏ nhất.

<br/>
**Ví dụ**
- Cho tập hợp $$\{1,2,3\}$$ là tập con của tập hợp các số tự nhiên, có quan hệ thứ tự thông thường $$\leq$$. Tụi mình có phần tử lớn nhất là 3, phần tử nhỏ nhất là 1.
<br/>
- Tiếp tục với ví dụ cái cây, tập hợp $$\{0,1,6\}$$ có quan hệ thứ tự được định nghĩa như hình vẽ có phần tử lớn nhất là 6 và không có phần tử nhỏ nhất.

<br/>
<br/>
## Phần tử cực đại, phần tử cực tiểu
### Phần tử cực đại
> $$ A \in \mathfrak{P}(E), x \in A$$. $$x$$ là phần tử cực đại của $$A$$ khi và chỉ khi:
> $$ \forall a \in A, x \preceq a \Rightarrow x = a$$

### Phần tử cực tiểu
> $$ A \in \mathfrak{P}(E), x \in A$$. $$x$$ là phần tử cực đại của $$A$$ khi và chỉ khi:
> $$ \forall a \in A, x \preceq a \Rightarrow x = a$$

Thú thật, lúc đầu học mình cũng không hiểu cái định nghĩa ni mô, mình không biết nó "cực đại" hay "cực tiểu" chỗ nào hết, và "cực đại" với "cực tiểu" thì khác chi "lớn nhất" với "nhỏ nhất".

Ta mình có hiểu là đối với phần tử cực đại $$x$$ thì không có phần tử nào "lớn hơn" nó và nếu có phần tử $$ y \in A$$ để có quan hệ thứ tự $$x \preceq y $$ thì chỉ mình $$x$$ mà thôi. Tương tự với phần tử cực tiểu.

<br/>
**Chú ý**
<br/>
- Khái niệm phần tử cực đại (cực tiểu) và phần tử lớn nhất (nhỏ nhất) là giống nhau đối với quan hệ thứ tự toàn phần.
- Có thể có nhiều phần tử cực đại hoặc cực tiểu.

**Ví dụ**
- Cho $$F = \{1,2,3\}. \mathfrak{P}(F) = \{\varnothing, \{1\}, \{2\},\{3\}, \{1,2\}, \{2,3\}, \{1,3\}, \{1,2,3\}\}$$. Quan hệ thứ tự ở đây là quan hệ bao hàm "x là tập con của y". Tụi mình có thể biểu diễn quan hệ thứ tự trên theo mỗi biểu đồ mũi tên như hình dưới. <br/>
  - Dựa vào biểu đồ, tụi mình có thể thấy, tập hợp $$A = \{\{1\},\{2\},\{3\},\{1,3\},\{1,2,3\}\}$$ có 3 phần tử cực tiểu là $$\{1\},\{2\},\{3\}$$ và 1 phần tử cực đại là $$\{1,2,3\}$$. Tại sao lại như vậy? Thì cứ theo định nghĩa, tụi mình sẽ suy ra được. <br/>
    - $$\{1\}$$ là phần tử cực tiểu, vì tụi mình có tìm trong tập hợp $$A$$ có phần tử $$a$$ nào để $$a \preceq \{1\}$$ không? Đáp án là chỉ là có $$\{1\}$$ thôi, $$\{1\}$$ chỉ tham gia vào quan hệ thứ tự trong $$\{1\} \preceq \{1\}, \{1\} \preceq \{1,3\}, \{1\} \preceq \{1,2,3\} \}$$. Xét trong tập hợp các quan hệ thứ tự của $$\{1\}$$, tụi mình có thể thấy $$\{1\}$$ không "lớn hơn" một phần tử nào cả, đó lí do tại sao nói là "cực tiểu". Mặc khác, để có phần tử $$y$$ nào thuộc $$A$$ để $$y\preceq \{1\}$$ thì chỉ có $$\{1\}$$ thôi, do đó không có có phần tử nào là "nhỏ hơn" $$\{1\}$$ nữa. Tương tự, các bạn có thể xem các trường hợp còn lại.  

><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="467px" version="1.1" content="&lt;mxfile userAgent=&quot;Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36&quot; version=&quot;8.0.6&quot; editor=&quot;www.draw.io&quot; type=&quot;google&quot;&gt;&lt;diagram id=&quot;ca112555-f51d-1c1f-40cf-68d71647f4ed&quot; name=&quot;Page-1&quot;&gt;7Zpdc6IwFIZ/DZd1SIKol2rb3Yvdmc70Yi93IkTIFAgT4tf++j0BovLR1rp+rCO9sOGFnECec8ILapFpvP4maRr+FD6LLGz7a4s8WhiP+jZ8amFTCC5GhRBI7hfSnvDK/7BSLPsFC+6zrHKgEiJSPK2KnkgS5qmKRqUUq+phcxFVR01pwBrCq0ejpvqL+yos1KG5LK1/ZzwIzcjILvfMqPcWSLFIyvEsTOb5X7E7piZWeXwWUl+s9iTyZJGpFEIVrXg9ZZGeWjNtRb/nd/Zuz1uyRB3Uoe/h4XA+8Cgh1HHnD2WEJY0WzFxCfqJqYyaHJf5YzzFseRHNMu5ZZBKqOAIBQXMuElUiJTZsZ4pKZXoIiGy0Zx6ZPsUgzG9g2V0I2k4PZB0TMVNyA4esdnwMnnAPjdEki6jiy2p4WqZJsA23HeFFcBgY22VGk0EZp0xoMrKrITKxkB4re+1PeC2QM6wF6tcCwcQETDUCQWPvsndSzvNAtrhje1a2jUDO5diSju1Z2WL3enXrdGyPQnIwW1wLZF+Orfs5W/AIqW7yOHctkyWTioNX+UFnLHoRGVdcJLB/JpQSMRwQ6R2TrROZikjIPJTxIrsY44gHuq8SKag0Sws3NedrBmc8yYccG9U2CrRDpbQXG+vJwM+LNBLU7634G4+Zz2lPyABkvZ3qbWh7Io5FkkFLhYt4Bv+1SvXHU5yqze+MqV621N2QjZ10/VCRe2kSbHNSnz1bfzUrzZJQSxvH0N7LWtyStdh+P0ErGfEV/IMm/sEEWYPHRhbABatqTWdKijdm6CYi0ckxh/qtSbRk7MEEMdkCP+a+r4eZrEKu2GtKPT3mCpw9aHkK6WTI8dfXkRPwaFSf2+RBWnigc/AYtvHAd8WDvOdQr8Fj1MaD3BUPp25hXPd6PFDnM4+z/rfgRVCL0dR3Izy9rxUQuU6FAR5dcQVE/a7izlpxfeeKFXeA/b9HuJ++JbsJuK3mHpTpfRmYfq1S8bB/xeW0xeF3FXfClyn1dRnX37ids+JaHhc6uCdcTq8J1xjjpju9r+V0ewv7H5ZTU2BdxX3xMe7oiruggcHdw/5xpvIm4HaPHsfd4m4CbsujxwdwS1T/SBYC3hRnVOOMjuVcC2Sjy3Fu/b6ieGN3d76o9gSDTP2d3hfB5u4nWgXH3c/gyNNf&lt;/diagram&gt;&lt;/mxfile&gt;" onclick="(function(svg){var src=window.event.target||window.event.srcElement;while (src!=null&amp;&amp;src.nodeName.toLowerCase()!='a'){src=src.parentNode;}if(src==null){if(svg.wnd!=null&amp;&amp;!svg.wnd.closed){svg.wnd.focus();}else{var r=function(evt){if(evt.data=='ready'&amp;&amp;evt.source==svg.wnd){svg.wnd.postMessage(decodeURIComponent(svg.getAttribute('content')),'*');window.removeEventListener('message',r);}};window.addEventListener('message',r);svg.wnd=window.open('https://www.draw.io/?client=1&amp;lightbox=1&amp;edit=_blank');}}})(this);" viewBox="0 0 467 263" style="cursor:pointer;max-width:100%;max-height:263px;"><defs/><g transform="translate(0.5,0.5)"><path d="M 223.82 230.97 L 325.02 194.18" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><ellipse cx="221" cy="232" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 329.95 192.38 L 324.57 198.06 L 325.02 194.18 L 322.17 191.48 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 221 229 L 221 188.37" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><ellipse cx="221" cy="232" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 221 183.12 L 224.5 190.12 L 221 188.37 L 217.5 190.12 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 218.18 230.97 L 116.98 194.18" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><ellipse cx="221" cy="232" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 112.05 192.38 L 119.83 191.48 L 116.98 194.18 L 117.43 198.06 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 109.13 189.66 L 74.98 146.97" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><ellipse cx="111" cy="192" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 71.7 142.87 L 78.8 146.15 L 74.98 146.97 L 73.34 150.53 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><image x="210.5" y="241.5" width="20" height="20" xlink:href="https://upload.wikimedia.org/wikipedia/commons/thumb/a/aa/Empty_set.svg/1024px-Empty_set.svg.png" preserveAspectRatio="none" pointer-events="none"/><g transform="translate(67.5,189.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="36" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 38px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">{1}</div></div></foreignObject><text x="18" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">{1}</text></switch></g><g transform="translate(227.5,179.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="36" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 38px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">{2}</div></div></foreignObject><text x="18" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">{2}</text></switch></g><g transform="translate(317.5,195.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="36" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 38px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">{3}</div></div></foreignObject><text x="18" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">{3}</text></switch></g><path d="M 218.1 181.23 L 77.15 143.64" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><ellipse cx="221" cy="182" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 72.08 142.29 L 79.75 140.71 L 77.15 143.64 L 77.94 147.47 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><g transform="translate(-0.5,119.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="61" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 63px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">{1,2}</div></div></foreignObject><text x="31" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">{1,2}</text></switch></g><path d="M 223.92 181.31 L 384.8 143.46" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><ellipse cx="221" cy="182" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 389.91 142.26 L 383.9 147.27 L 384.8 143.46 L 382.3 140.45 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 333.3 190.08 L 386.11 146.08" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><ellipse cx="331" cy="192" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 390.14 142.72 L 387 149.89 L 386.11 146.08 L 382.52 144.51 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><g transform="translate(405.5,114.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="61" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 63px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">{2,3}</div></div></foreignObject><text x="31" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">{2,3}</text></switch></g><path d="M 113.63 190.56 L 215.41 135.05" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><ellipse cx="111" cy="192" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 220.02 132.54 L 215.55 138.96 L 215.41 135.05 L 212.2 132.81 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 328.37 190.56 L 226.59 135.05" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><ellipse cx="331" cy="192" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 221.98 132.54 L 229.8 132.81 L 226.59 135.05 L 226.45 138.96 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><g transform="translate(135.5,114.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="61" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 63px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">{1,3}</div></div></foreignObject><text x="31" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">{1,3}</text></switch></g><path d="M 73.5 140.34 L 215.7 45.53" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><ellipse cx="71" cy="142" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 220.07 42.62 L 216.19 49.42 L 215.7 45.53 L 212.3 43.59 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 388.41 140.48 L 226.49 45.23" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><ellipse cx="391" cy="142" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 221.96 42.57 L 229.77 43.1 L 226.49 45.23 L 226.22 49.13 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 221 129 L 221 48.37" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><ellipse cx="221" cy="132" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 221 43.12 L 224.5 50.12 L 221 48.37 L 217.5 50.12 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 222 130 L 222 46" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><ellipse cx="222" cy="133" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="222" cy="43" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><g transform="translate(182.5,-0.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="86" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 88px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">{1,2,3}</div></div></foreignObject><text x="43" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">{1,2,3}</text></switch></g></g></svg>

- Cho tập hợp $$E = \mathbb{N} - \{0,1\}$$ cùng với quan hệ thứ tự "là ước của" được định nghĩa trên nó. Xét tập con $$A = \{2,4,6\}$$. Quan hệ thứ tự của các phần tử trong $$A$$ có thể biểu diễn theo biểu đồ mũi tên như hình vẽ phía dưới. Dựa vào biểu đồ, tụi mình có thể thấy 2 vừa là phần tử nhỏ nhất, vừa là phần tử cực tiểu của tập hợp $$A$$. Tập hợp $$A$$ có 2 cực đại là 4 và 6. Tập A không có phần tử lớn nhất.

> <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="252px" version="1.1" content="&lt;mxfile userAgent=&quot;Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36&quot; version=&quot;8.0.6&quot; editor=&quot;www.draw.io&quot; type=&quot;google&quot;&gt;&lt;diagram id=&quot;cd8c614e-01af-1a30-8eca-52dce8e018ef&quot; name=&quot;Page-1&quot;&gt;7ZjBjpswEIafhmMlsCEJx026214qVcqhZwdPwFqDI+ME0qevATvB0HSTarVpl80hwr/tGXu+MR7h4VVef5Fkl30TFLiHfFp7+LOHUBz5+r8Rjp0wQ0EnpJLRTuoJa/YTjGjmpXtGoXQGKiG4YjtXTERRQKIcjUgpKnfYVnDX646kMBLWCeFj9QejKuvUhd1Wo38FlmbWc+Cbng1JnlMp9oXx5yG8bX9dd06sLTO+zAgVVU/Cjx5eSSFU95TXK+BNaG3YunlPF3pP65ZQqGsmzOJoAz4sMI6jMIbNJ2PhQPge7BbahaqjDQ4U9KGJsW4lnJQlSzy8zFTOtRDox60olEGKfd3uDAAdhfy8yOC0dZ1RIHJQ8qiHVOfY29BnvbBbTQInih1c88SkQHoyd/LwXTDtGPkmW0ObdSZZ8dx3TZRiLxMws/rBHBjCoWsIxQNDisgU1MiQfuht+yy1rK7khj64/TW3cHE/bvgmbkKP+zO0Uq9VDYa32hPjdo422GtNBvM9j2f4gXkKpzkaYR5zVlArF26ppHiGleBCaqUQBTTENbqBRDhLi+btrYmB1pcHkIrpquXBdOSM0sbNssqYgvWOJI3PSpdoWmurEmhW7l982TcGob41Qez5WkQuQRv4XgKFv0kg5F/OFQfOLSRmIxKz6ZAI48ERmN+RxHxEIpwOCfQvkVjcdAmZAFNSZm2Egv+7WozCd3C/xFMm+GL9dnUhOCg1kP92BK3raSJ88excizAaIgzeEOFt30jeG8LXqtOHVyN+NYS6ef6C1g0/f6XEj78A&lt;/diagram&gt;&lt;/mxfile&gt;" onclick="(function(svg){var src=window.event.target||window.event.srcElement;while (src!=null&amp;&amp;src.nodeName.toLowerCase()!='a'){src=src.parentNode;}if(src==null){if(svg.wnd!=null&amp;&amp;!svg.wnd.closed){svg.wnd.focus();}else{var r=function(evt){if(evt.data=='ready'&amp;&amp;evt.source==svg.wnd){svg.wnd.postMessage(decodeURIComponent(svg.getAttribute('content')),'*');window.removeEventListener('message',r);}};window.addEventListener('message',r);svg.wnd=window.open('https://www.draw.io/?client=1&amp;lightbox=1&amp;edit=_blank');}}})(this);" viewBox="0 0 252 218" style="cursor:pointer;max-width:100%;max-height:218px;"><defs/><g transform="translate(0.5,0.5)"><path d="M 120 170 L 54.19 94.79" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 50.74 90.84 L 57.98 93.8 L 54.19 94.79 L 52.71 98.41 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 120 170 L 185.81 94.79" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 189.26 90.84 L 187.29 98.41 L 185.81 94.79 L 182.02 93.8 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 118.02 167.74 L 51.98 92.26" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><ellipse cx="120" cy="170" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="50" cy="90" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><path d="M 121.98 167.74 L 188.02 92.26" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><ellipse cx="120" cy="170" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><ellipse cx="190" cy="90" rx="3" ry="3" fill="#000000" stroke="#000000" pointer-events="none"/><g transform="translate(106.5,182.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="16" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 18px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">2</div></div></foreignObject><text x="8" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">2</text></switch></g><g transform="translate(211.5,62.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="16" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 18px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">6</div></div></foreignObject><text x="8" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">6</text></switch></g><g transform="translate(11.5,62.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="16" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 18px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">4</div></div></foreignObject><text x="8" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">4</text></switch></g><path d="M 250 170 L 190 90" fill="none" stroke="#000000" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="none"/><path d="M 50 90 L 20 0" fill="none" stroke="#000000" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="none"/><path d="M 190 90 L 220 10" fill="none" stroke="#000000" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="none"/><path d="M 120 170 L 0 110" fill="none" stroke="#000000" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="none"/></g></svg>


Để tổng hợp lại những gì tụi mình vừa tìm hiểu, hãy làm một bài tập nhỏ coi như là một ví dụ cho tất cả các khái niệm ở trên. <br/>
Cho $$E = \{1,2,3,4,5\}, \mathcal{R}$$ là quan hệ thứ tự xác định trong $$E$$. Xét các tập con của $$E$$ là $$A = \{2,3\}, \, B = \{2,4\}, C = \{1,2,5\}$$. Quan hệ thứ tự được biểu diễn theo biểu đồ mũi tên. Hãy xem thử $$A,B,C$$ có phần tử lớn nhất, phần tử cực đại, biên trên hay không?

> <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="291px" version="1.1" content="&lt;mxfile userAgent=&quot;Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36&quot; version=&quot;8.0.6&quot; editor=&quot;www.draw.io&quot; type=&quot;google&quot;&gt;&lt;diagram id=&quot;045bca11-0fad-1aa9-b005-d0542d26e559&quot; name=&quot;Page-1&quot;&gt;7VhNc9owEP01PqZjSzaGY4C0vXQmM+lM06NiL7YmwqKyCNBfX8mS/Ek+IKR0hnIA62m1Wr99uzL28Gy5/SLIKv/GU2Ae8tOth+ceQpPIV98a2BlghAIDZIKmBmoBd/Q3WNCuy9Y0hbJjKDlnkq66YMKLAhLZwYgQfNM1W3DW3XVFMhgAdwlhQ/QHTWVu0LG7LY1/BZrlbufAtzMPJHnMBF8Xdj8P4UX1MdNL4nxZ+zInKd+0IHzj4ZngXJqr5XYGTFPraDPrPj8zW8ctoJBvWRDjACc4jmIU+xGOgyvr4YmwNbhbqAKVO0cOFOm15liNEkbKkiYenuZyyRQQqMsFL6RNKfbV2DiAdEB5E2RQ37pSFPAlSLFTJpuGe0d93qLdYQIYkfSp655YCWS1u3qHW07Vxsi3ag2d6qxYcex3XZR8LRKwq9pkvuYI9xxJIjKQA0eKTbJrma20QXlAwONOktWF8ehGLU4bqBLCG0WB9ohixKTNdUcdo19r7iauykoF18oA+6ttM6muMv2LnRsVkfFk8IHkJGxlV2SlFPwRZpxxoZCCF6A3pYz1IMJoVmilKq2BwqdPICRVlX5tJ5Y0TfU2001OJdytSKL33Ki2prCqkkHT0ghZO4DtoVK2C/CklzrfumhJPdwjddRTUlvVrbwfllb8v9bR5ES1Xgf4Sq2fohzDDyrH6OLLsa6zc5RjNEhr8AbmBai0kofKQLNiDw9lHU29aK45X0tuUl8tcClgsJB7EiC5ZrpUxNMi+64HcyW45yr9XeyHfv/gnQzYx3vYDz+C/fHpmyFsqbzXc598jO34p07TpyiO7PgWBFXB61qYH9JAVWBVp3pJS+dqsv2qCo9tstGRD1SnaLKTD2qy4cU12UEWz/nM42K5pIeeQT36R9Yj7jfsv1iPwb5/pqcoSHRxBYlG/1JB7vtz+d6Dt1BR3VvCqoE5dutT994ubE5kFJ3u8HVSNdXw0kP8uToC6j/3jo/sCPVC6yjovzs5uiOoYfMazJg3rxrxzR8=&lt;/diagram&gt;&lt;/mxfile&gt;" onclick="(function(svg){var src=window.event.target||window.event.srcElement;while (src!=null&amp;&amp;src.nodeName.toLowerCase()!='a'){src=src.parentNode;}if(src==null){if(svg.wnd!=null&amp;&amp;!svg.wnd.closed){svg.wnd.focus();}else{var r=function(evt){if(evt.data=='ready'&amp;&amp;evt.source==svg.wnd){svg.wnd.postMessage(decodeURIComponent(svg.getAttribute('content')),'*');window.removeEventListener('message',r);}};window.addEventListener('message',r);svg.wnd=window.open('https://www.draw.io/?client=1&amp;lightbox=1&amp;edit=_blank');}}})(this);" viewBox="0 0 291 207" style="cursor:pointer;max-width:100%;max-height:207px;"><defs/><g transform="translate(0.5,0.5)"><path d="M 150 157 L 150 162 Q 150 167 150 157 L 150 123.37" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 150 118.12 L 153.5 125.12 L 150 123.37 L 146.5 125.12 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><g transform="translate(141.5,80.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="16" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 18px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;"><font style="font-size: 30px">3</font></div></div></foreignObject><text x="8" y="23" fill="#000000" text-anchor="middle" font-size="12px" font-family="Helvetica">[Not supported by viewer]</text></switch></g><path d="M 150 77 L 150 43.37" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 150 38.12 L 153.5 45.12 L 150 43.37 L 146.5 45.12 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><g transform="translate(141.5,-0.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="16" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 18px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;"><font style="font-size: 30px">5</font></div></div></foreignObject><text x="8" y="23" fill="#000000" text-anchor="middle" font-size="12px" font-family="Helvetica">[Not supported by viewer]</text></switch></g><g transform="translate(141.5,168.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="17" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 30px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; white-space: nowrap;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;">1</div></div></foreignObject><text x="9" y="32" fill="#000000" text-anchor="middle" font-size="30px" font-family="Helvetica">1</text></switch></g><path d="M 171 189 L 245.29 121.29" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 249.17 117.75 L 246.36 125.06 L 245.29 121.29 L 241.64 119.88 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><g transform="translate(261.5,80.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="16" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 18px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;"><font style="font-size: 30px">4</font></div></div></foreignObject><text x="8" y="23" fill="#000000" text-anchor="middle" font-size="12px" font-family="Helvetica">[Not supported by viewer]</text></switch></g><path d="M 130 187 L 45.03 120.91" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 40.88 117.69 L 48.56 119.22 L 45.03 120.91 L 44.26 124.75 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><g transform="translate(11.5,80.5)"><switch><foreignObject style="overflow:visible;" pointer-events="all" width="16" height="34" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"><div xmlns="http://www.w3.org/1999/xhtml" style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; vertical-align: top; width: 18px; white-space: nowrap; word-wrap: normal; text-align: center;"><div xmlns="http://www.w3.org/1999/xhtml" style="display:inline-block;text-align:inherit;text-decoration:inherit;"><font style="font-size: 30px">2</font></div></div></foreignObject><text x="8" y="23" fill="#000000" text-anchor="middle" font-size="12px" font-family="Helvetica">[Not supported by viewer]</text></switch></g><path d="M 40 93 L 125 25.94" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 129.12 22.69 L 125.79 29.78 L 125 25.94 L 121.46 24.28 Z" fill="#000000" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/></g></svg>

Thay vì kí hiệu $$\mathcal{R}$$, tụi mình sẽ dùng $$\preceq$$ nhé.
Dựa vào biểu đồ này, tụi mình có các quan hệ, mình không liệt kê các quan hệ phản xạ như $$1\preceq 1$$ vào nhé: $$ 1 \preceq 2, 2 \preceq 5, 1\preceq 5, 1 \preceq 3, 3\preceq 5, 1 \preceq 4$$. Ở đây, các con số không phải là các số tự nhiên mà trừu tượng hoá của các đối tượng trong thực tế, ví dụ như các điạ điểm trên bản đồ chẳng hạn. Nên 2 không "nhỏ hơn" 3 hay 4 không "nhỏ hơn" 5 là hợp lí nhé (lúc đầu, mình không hiểu thật đó). <br/>

Đối với tập hợp $$A$$, tụi mình có các quan hệ: $$2\preceq 2, 3 \preceq 3$$. Tập hợp này có $$2, 3$$ là các phần tử cực đại cũng như là phần tử cực tiểu, không có giá trị lớn nhất, có biên trên là $$5$$.
<br/>

Đối với tập hợp $$B$$, tụi mình có các quan hệ: $$2 \preceq 2, 4 \preceq 4$$. Tập hợp này không có biên trên vì chỉ có 2 là "nhỏ hơn" 5 còn 4 thì không, tương tự tập hợp $$A$$, $$2,4$$ vừa là phần tử cực đại vừa là phần tử cực tiểu của $$B$$. Tập hợp $$B$$ không có phần tử lớn nhất. Tập hợp B có biên dưới là 1.
<br/>

Đối với tập hợp $$C$$, tụi mình có các quan hệ:  $$1 \preceq 1, 2 \preceq 2, 5 \preceq 5, 1 \preceq 2, 1\preceq 5, 2\preceq 5$$. Tập hợp $$C$$ có 5 vừa là phần tử lớn nhất, biên trên và phần tử cực đại, 1 vừa là phần tử nhỏ nhất vừa là phần tử cực tiểu.



Kết, hiểu được quan hệ tương đương và đặc biệt là quan hệ thứ tự sẽ giúp các bạn hiểu rõ được các bài toán sắp xếp, tối ưu, lí thuyết đồ thị cũng như các thuật toán "khó nhằng" trong lập trình, chúng đều là những bài toán ứng dụng thực tế cao. Bài viết hơi dài, hi vọng các bạn tìm thấy niềm vui trong việc khám phá ra những điều mới mẻ. 

Ted
<br/>
<br/>



# Tham khảo

[Relations and their types - geeksforgeeks.org](https://www.geeksforgeeks.org/relations-and-their-types/)<br/>
[Equivalence relation - Wikipedia](https://en.wikipedia.org/wiki/Equivalence_relation)<br/>
[Equivalence class - Wikipedia](https://en.wikipedia.org/wiki/Equivalence_class)<br/>
[Order relation - Old Dominion University](http://www.cs.odu.edu/~cs381/cs381content/relation/order/order.html)<br/>
[Maximal and minimal elements - Wikipedia](https://en.wikipedia.org/wiki/Maximal_and_minimal_elements)<br/>
Đại số 1 - Jean-Marie Monier<br/>
Giáo trình Toán - Thầy Bùi Tuấn Khang<br/>
Naive Set Theory - Paul R. Halmos<br/>
Elements of Set Theory - Herbert B. Enderton<br/>
