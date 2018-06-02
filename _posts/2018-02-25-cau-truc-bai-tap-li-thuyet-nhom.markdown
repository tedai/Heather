---
layout: post
title:  "Bài tập về nhóm"
subtitle: "Tụi mình đã biết được những gì về nhóm?"
date:   2018-02-25
categories: [dai-so]
permalink:
cover:
description:
mathjax: true


---

# Mục tiêu

- ### Làm quen khái niệm nhóm và nhóm con

# Bài tập
Các bài tập này mình lấy trong sách Giải tích 1 của Jean Marie Monier. Các bạn có thể tìm sách mà đọc nhé.

## Luật hợp thành trong

### Bài tập 1
Cho $$* $$ là một luật hợp thành trong xác định trên $$\mathbb{R} $$ bởi: <br/>
### <center>$$x * y = xy + (x^2 - 1)(y^2-1)$$</center>
Kiểm chứng $$* $$ có tính giao hoán, không có tính kết hợp và có phần tử trung hoà <br/>


_Lời giải_

_Tính giao hoán_

Cho $$(x,y) \in \mathbb{R}^2$$, $$y*x = yx + (y^2 -1 )(x^2 -1) = xy +(x^2-1)(y^2-1)=x*y$$. <br/>Suy ra $$* $$ có tính giao hoán

_Tính kết hợp_

Lấy một phản ví dụ:<br/>
$$0 * (2 * 3) = 0*(2.3 + (2^2-1)(3^2-1)) = 0*30 = 0.30 + (0^2-1)(30^2-1) = 899$$ <br/>
$$(0*2)* 3 = (0.2 + (0^2-1)(2^2-1))* 3 = -3*3 = -3.3 + ((-3)^2-1)(3^2-1)= 55 \neq 899$$

Suy ra $$ * $$ không có tính kết hợp.

_Phần tử trung hoà_

Gọi $$e $$ là phần tử trung hoà của $$* $$.

$$\forall x \in \mathbb{R} \Rightarrow x*e = e*x = x \Rightarrow \begin{cases} x*e = e*x \\ x*e = x \end{cases} \Rightarrow \begin{cases}  xe + (x^2 - 1)(e^2-1) =  ex + (e^2 - 1)(x^2-1) \\  xe + (x^2 - 1)(e^2-1) = x \end{cases} $$<br/>
$$\begin{cases}  0x = 0 \,\,\, \text{luôn đúng}\\  (e-1)(x+(x^2 - 1)(e+1)) = 0 \end{cases} \Rightarrow e = 1$$<br/>

Thử lại với $$e = 1$$.

$$\forall x \in \mathbb{R}, x*1 = x.1 + (x^2-1)(1^2-1) = x$$.

Vậy $$1$$ là phần tử trung hoà đối với $$* $$.

<br/>
<br/>
### Bài tập 2
$$X, E$$ là các tập hợp. $$* $$ là luật hợp thành trong $$ E$$. $$\diamond $$ là luật hợp thành trong $$E^X$$ được xác định bởi:
### <center> $$\forall f,g \in E^X, f\diamond g \Leftrightarrow \forall x \in X, \quad (f \diamond g)(x) = f(x) * g(x)$$</center>
Chứng minh rằng:

a. Nếu $$* $$ có tính kết hợp thì $$ \diamond $$ có tính kết hợp.<br/>
b. Nếu $$* $$ có tính giao hoán thì $$\diamond $$ có tính giao hoán.<br/>
c. Nếu $$* $$ có phần tử trung hoà thì $$\diamond $$ có phần tử trung hoà. <br/>

_Lời giải_

a.

$$* $$ có tính kết hợp $$\Rightarrow f, g, h \in E^X, \forall x \in X, f(x)* (g(x) * h(x)) = (f(x)* g(x))* h(x)$$

### $$\forall (f,g,h) \in (E^X)^3, f \diamond (g \diamond h) \Leftrightarrow \forall x \in X, (f \diamond (g \diamond )) (x)=f(x)* (g \diamond h)(x) $$

$$= f(x)* (g(x) * h(x)) = (f(x)* g(x))* h(x) = (f\diamond g)(x)* h(x) = ((f \diamond g) \diamond h)(x)$$.

### $$(f \diamond g) \diamond h$$

Suy ra $$ \forall (f,g,h) \in (E^X)^3, f\diamond (g \diamond h) = (f \diamond g)\diamond h$$. Vậy $$\diamond $$ có tính kết hợp.

b.

Chứng minh tương tự trường hợp có tính kết hợp.

c.

Gọi $$e$$ là phần tử trung hoà của $$* \Rightarrow \forall x \in X,f \in E^X,  f(x)* e = e * f(x) = f(x)$$

Giả sử $$e'$$ là phần trung hoà của $$ \diamond \Rightarrow \forall f\in E^X, f\diamond e' = e' \diamond f = f$$

Điều này tương đương $$\begin{cases} f \diamond e' = f \diamond e' \\ f \diamond e' = f \end{cases} \Leftrightarrow \forall x \in X, \begin{cases} f(x) * e'(x) = f(x) * e'(x) \\ f(x) * e'(x) = f(x) \end{cases} \Leftrightarrow f(x)* e'(x) = e'(x) * f(x) = f(x) $$

Nếu $$e'$$ là ánh xạ hằng thì $$e'(x)$$ là phần tử trung hoà đối với $$* $$ trên $$E$$.

Trên $$E$$, phần tử trung hoà $$e$$ là duy nhất $$\Rightarrow \forall x \in X, e'(x) = e$$. Suy ra ánh xạ $$e': \underset{x \rightarrow e}{X \rightarrow E}$$ là phần tử trung hoà trên $$E^X$$.

Kiểm chứng<br/>
$$f \diamond e' \Rightarrow \forall x \in X, f(x)* e = f(x) \Rightarrow f$$. Suy ra $$f \diamond e' = f$$. <br/>
Tương tự $$ e' \diamond f = f$$. Vậy e' là phần tử trung hoà trên $$E^X$$.

<br/>
<br/>
### Bài tập 3
Cho $$ E $$ là tập hợp cùng với luật hợp thành trong $$* $$ trên nó. $$A \in \mathfrak{P}(E) $$ <br/> $$A = \{ x \in E; \forall (y,z) \in E^2, (x* y) * z = x* (y* z) \}$$.

Chứng minh luật hợp thành trong $$* $$ có tính ổn định trong $$A$$.

_Lời giải_

Tụi mình cần chứng minh: $$\forall (x,y)\in A^2: x * y \in A$$. Vậy tụi mình cần chứng minh: $$\forall (y,z) \in E^2, ((x*y)* z) * t = (x*y)* (z * t) $$.

$$\forall (x,y) \in A^2, \forall (y,z) \in E^2, ((x*y)* z)* t = x* (y*z) * t = (x* y)* (z * t) \Rightarrow x*y \in A$$.

Vậy $$* $$ có tính ổn định đối với $$A$$.

<br/>
<br/>
## Nhóm và nhóm con

### Bài tập 4
Cho $$(G,\top), (G',\bot)$$ là hai nhóm, $$* $$ là luật hợp thành trong $$G \times G'$$ xác định bởi:
### <center>$$(x,y)* (x',y') = (x \top x', y \bot y')$$</center>

a. Chứng minh $$(G \times G', * )$$ là một nhóm.<br/>
b. Chứng minh rằng, nếu $$H, H'$$ lần lượt là nhóm con của $$G, G'$$ thì $$H \times H'$$ là nhóm con  của $$G \times G'$$.

_Lời giải_

a.<br/>
_Tính kết hợp_

### $$\forall (u,v,w) \in (G \times G')^3, (u*v)* w \Leftrightarrow ((x,y)* (x',y'))* (x",y") = (x \top x', y \bot y')* (x",y")$$
$$ = ((x \top x')\top x", (y \bot y')\bot y")= (x \top (x'\top x"), y \bot (y'\bot y")) = (x,y)* (x'\top x", y'\bot y")$$
$$=(x,y)* ((x',y') * (x",y")) \Leftrightarrow u*(v * w) $$

Suy ra $$* $$ có tính kết hợp trong $$G \times G'$$.

_Phần tử trung hoà_

Cho $$e, e'$$ lần lượt là phần tử trung hoà trong mỗi nhóm $$G, G'$$.

Tụi mình có $$\forall (x,y) \in G \times G', (e, e') * (x,y) = (e \top x, e' \bot y) = (x,y)$$<br/>
Tương tự: $$ (x,y)* (e, e') = (x,y)$$.

Vậy $$(e,e')$$ là phần tử trung hoà trong $$G \times G'$$.

_Phần tử khả nghịch_

Cho $$x^{-1}$$ là phần tử nghịch đảo của $$x \in G$$, $$y^{-1}$$ là phần tử nghịch đảo của $$y \in G'$$.

$$\forall (x,y) \in G \times G'$$. Tụi mình có $$(x^{-1}, y^{-1}) * (x,y) = (x^{-1} \top \,x, y^{-1} \bot\, y) = (e, e')$$<br/>
Tương tự:  $$(x,y)* (x^{-1}, y^{-1}) = (e,e')$$.

Suy ra mọi phần tử trong $$G \times G'$$ đều khả nghịch.

Vậy $$G \times G'$$ là một nhóm.

b.<br/>
_Tính đóng_

### $$\forall ((x,y),(x',y')) \in (H \times H')^2, (x,y)* (x',y') = (x \top x', y \bot y')$$

Vì $$H, H'$$ lần lượt là các nhóm con của $$G, G'$$ nên $$ x \top x' \in H$$ và $$y \bot y' \in H'$$ do tính đóng của nhóm con.

Suy ra $$(x,y)* (x',y') \in H \times H'$$

_Phần tử trung hoà_

### $$e \in H, e' \in H' \Rightarrow (e,e') \in H\times H'$$

_Phần tử khả nghịch_

### $$x \in H \Leftrightarrow x^{-1} \in H, y \in H' \Leftrightarrow y^{-1} \in H'$$<br/>
Suy ra $$\forall (x,y) \in H \times H' \Rightarrow (x^{-1}, y^{-1}) \in H\times H'$$

<br/>
<br/>
### Bài tập 5

Cho $$G = \mathbb{R}^* \times \mathbb{R}$$ và $$* $$ là luật hợp thành trong $$G$$ xác định bởi:
### <center> $$(x,y)* (x',y')=(xx',xy'+y)$$</center>

a. Chứng minh $$(G, * ) $$ là một nhóm không giao hoán.<br/>
b. Chứng minh $$\mathbb{R}_+^* \times \mathbb{R}$$ là một nhóm con của $$G$$.

_Lời giải_

a.

_Tính kết hợp_

$$\forall ((x,y),(x',y'),(x",y")) \in G^3, ((x,y)* (x',y'))* (x", y")= (xx',xy'+y)* (x", y") = ((xx')x", (xx')y" + (xy'+y))$$.

$$(x,y)* ((x',y')* (x", y")) = (x,y)* (x'x",x'y"+y') = (x(x'x"), x(x'y"+y') + y) = ((xx')x", (xx')y" + (xy'+y))$$.

Suy ra $$\forall ((x,y),(x',y'),(x",y")) \in G^3, ((x,y)* (x',y'))* (x", y")=(x,y)* ((x',y')* (x", y"))$$

Vậy $$* $$ có tính kết hợp.

_Phần tử trung hoà_

Giả sử $$G$$ có phần tử trung hoà là $$e = (x_0, y_0)$$

Tụi mình có: $$(x_0,y_0) * (x,y) = (x,y) \Rightarrow (x_0 x,x_0 y + y_0) = (x,y) \Rightarrow \begin{cases} x_0x = x \\ x_0 y + y_0 = y \end{cases} \Rightarrow e = (1,0)$$

$$(x,y) * (x_0,y_0) = (x,y) \Rightarrow (xx_0,xy_0 + y) = (x,y) \Rightarrow \begin{cases} xx_0 = x \\ xy_0 + y = y \end{cases} \Rightarrow e = (1,0)$$<br/>

Kiểm chứng:<br/>
$$\forall (x,y) \in G:$$

$$(x,y)* (1,0) = (x.1, x.0 + y) = (x,y)$$.<br/>
$$(1,0)* (x,y) = (1.x, 1.y + 0) = (x,y)$$.

Vậy $$(1,0)$$ là phần tử trung hoà của $$G$$.

_Phần tử khả nghịch_

Giả sử $$(x',y')$$ là phần tử nghịch đảo của $$(x,y)$$.

$$\forall (x,y) \in G:$$<br/>
$$(x',y')* (x,y) = (1,0) \Rightarrow (x'x,x'y+y') = (1,0) \Rightarrow \begin{cases} x'x=0 \\ x'y + y' = 0 \end{cases} \Rightarrow \begin{cases} x'=x^{-1} \\ y' = -x^{-1}y \end{cases}$$ <br/>
$$\Rightarrow (x',y') = (x^{-1}, -x^{-1}y)$$

$$(x,y)* (x',y') = (1,0) \Rightarrow (xx',xy'+y) = (1,0) \Rightarrow \begin{cases} xx'=0 \\ xy' + y = 0 \end{cases} \Rightarrow \begin{cases} x'=x^{-1} \\ y' = -x^{-1}y \end{cases}$$ <br/>
$$\Rightarrow (x',y') = (x^{-1}, -x^{-1}y)$$

Rõ ràng là $$x' = x^{-1} \in \mathbb{R}^* , y= -x^{-1}y \in \mathbb{R}$$

Nên $$(x',y') \in G$$

Vậy $$G$$ là một nhóm

_Tính giao hoán_

Tụi mình tìm các phản ví dụ.

$$(2,3)* (1,2) = (2.1,2.2+3) = (2,7)$$<br/>
$$(1,2)* (2,3) = (1.2,1.3+2) = (2, 5) \neq (2,7)$$

Vậy $$G$$ là nhóm không giao hoán.

b.
Đặt $$H = \mathbb{R}_+^* \times \mathbb{R}$$<br/>
Rõ ràng $$H \subset G$$.

_Tính đóng_

$$\forall ((x,y),(x',y')) \in H^2, (x,y)* (x',y') = (xx',xy'+y)$$.

$$x, x' \in \mathbb{R}_+^* \Rightarrow xx' > 0 $$ hay $$ xx' \in \mathbb{R}_+^* $$<br/>
$$xy'+y \in \mathbb{R}$$

Suy ra $$(xx',xy'+y) \in H$$ hay $$(x,y)* (x',y') \in H$$

_Phần tử trung hoà_

$$(1,0) \in H$$.

_Phần tử khả nghịch_

$$\forall (x,y) \in H, (x^{-1}, -x^{-1}y) \in H$$.

Suy ra, $$H$$ là một nhóm con của $$G$$.

<br/>
<br/>
Mục đích của bài viết chỉ là giúp tụi mình có thể nhớ lại những gì tụi mình biết về nhóm nên mình không chú tâm vào các bài khó vì thấy không cần thiết. Hi vọng bài viết này giúp ích được các bạn.


> It is the fight alone that pleases us, not the victory. - Blaise Pascal

Ted

<br/>
<br/>
# Tham khảo

Đại số 1 - Jean-Marie Monier<br/>
Giáo trình Toán - Thầy Bùi Tuấn Khang<br/>
