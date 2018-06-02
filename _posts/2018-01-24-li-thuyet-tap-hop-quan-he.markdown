---
layout: post
title:  "Lí thuyết tập hợp - Quan hệ"
subtitle: "Quan hệ là gì?"
date:   2018-01-24
categories: [dai-so]
permalink:
cover:
description:
mathjax: true
---

# Mục tiêu

- ### Quan hệ hai ngôi, quan hệ hai ngôi đồng nhất là gì?
- ### Quan hệ ngược
- ### Các tính chất có thể có của quan hệ hai ngôi
- ### Hợp hai quan hệ

<br/>
Đây đây tới cái phần hồi trước mình bắt đầu "xoắn não" đây =)). Quay lại về khái niệm tập hợp ở trên, khi nhắc đến tập hợp là tụi mình mới với về khái niệm "gom cái gì đó vào một chỗ", để "làm được gì đó" với tập hợp ta vẫn cần phải một _vài thứ khác_. Và đây khái niệm cơ bản khi học về cơ sở dữ liệu sau này.  Như ở bài trước, tụi mình đã định nghĩa về _quan hệ bao hàm_ nhưng chưa có gì đã định nghĩa về _Quan hệ_ cả. Do đó trong phần này tụi mình sẽ tìm hiểu về _quan hệ_, và chủ yếu là _quan hệ hai ngôi_. Tại sao gọi là _quan hệ hai ngôi_? =)) đơn giản là quan hệ giữa hai vật nào đó. Nhưng mình đã nói từ tập hợp chúng ta sẽ có được nhiều thứ, và bây giờ tụi mình sẽ xây dựng _quan hệ hai ngôi_ từ thứ tụi mình đang có: Tập hợp.

# Quan hệ (hai ngôi) là gì?

>$$E,\,F$$ là hai tập hợp. Mọi bộ ba $$(E,\,\Gamma,\, F)$$, trong đó $$\Gamma \in \mathfrak{P}(E \times F)$$, gọi là quan hệ từ $$E$$ đến $$F$$. Cho $$x \in E$$ và $$y \in F$$, nếu $$x$$ có quan hệ $$\mathcal{R}$$ với $$y$$ thì $$(x,y) \in \Gamma$$.

Tụi mình có thể kí hiệu $$x\mathcal{R}y$$ thay cho $$(x,y)\in \Gamma$$.<br/>
$$E$$ gọi là tập nguồn của $$\mathcal{R}$$. $$x \in E$$ <br/>
$$F$$ gọi là tập đích của $$\mathcal{R}$$. $$y \in F$$<br />
$$\Gamma$$ gọi là đồ thị của $$\mathcal{R}$$. <br />

**Chú ý**: khi $$F = E$$ thì ta gọi $$\mathcal{R}$$ là **quan hệ hai ngôi** đồng nhất. Đây là khái niệm quan hệ phổ biến trong toán học.

Bản thân mình thấy định nghĩa trên khá phức tạp, nhưng nó lại khá chặt chẽ vì khi định nghĩa quan hệ, sau này là hàm, phần lớn sẽ quên định nghĩa tập nguồn và tập đích của quan hệ. Từ định nghĩa trên, tụi mình có thể hiểu việc định nghĩa _quan hệ_ dựa trên bộ ba $$E,\Gamma, F$$ là giúp chúng ta luôn nhớ định nghĩa tập nguồn và tập đích của quan hệ. $$\Gamma$$ là tập hợp các $$(x,y) \in E \times F$$ có quan hệ $$\mathcal{R}$$ với nhau. Vậy ta có thể hiểu định nghĩa _quan hệ_ mang tính "tập hợp" hơn.

Quan hệ là tập hợp các cặp có thứ tự $$(x,y) \in E \times F$$ mà các tập nguồn $$E$$ và tập đích $$F$$ được xác định rõ. Như vậy, quan hệ vẫn chỉ là tập hợp nhé, không có gì lạ lẫm hết =)).

Từ đó ta viết các quan hệ $$\in, \subset$$ nhìn có vẻ "toán" hơn =)). <br/>

  $$\in\,  = (E, \,\Gamma,\, \mathfrak{P}(E) )$$. $$\Gamma = \{(x,A): x \, \text{thuộc}\, A\}$$.

Chú ý là tập hợp $$E$$ ở đây không giống như ở trên định nghĩa mà là tập hợp trừu tượng được coi là chứa tất cả mọi thứ. Nhớ lại tụi mình không có định nghĩa là khái niệm "thuộc", mà chỉ chấp nhận nó. Nếu $$x \in E, A\in \mathfrak{P}(E), x\in A \Rightarrow (x,A) \in \Gamma $$.


Từ đây, ta có thể định nghĩa quan hệ bao hàm của hai tập hợp. $$\subset \, = (E,\Gamma,E)$$, $$ \Gamma = \{(A,B) : \forall x \in A \Rightarrow x \in B  \}$$.


Ví dụ: Chúng ta chưa đề cập đến tập số nguyên, nhưng trong ví dụ này sẽ coi như các bạn đã "biết" về tập hợp số nguyên rồi.
  Quan hệ "bé hơn" trong tập hợp số nguyên: $$<\, = (\mathbb{Z}, \Gamma, \mathbb{Z}) $$ với $$\Gamma = {(x,y) : x < y}$$. Việc làm sao để biết $$x < y$$ thì các bạn sẽ biết khi học về tập hợp số nguyên. Do $$3 < 5 \Rightarrow (3,5) \in \Gamma$$ của $$<$$. <br/>

Ví dụ khác: Ta có thể biễu diễn một quan hệ bằng biểu đồ hình tên, trong đó mũi tên sẽ đi từ $$x$$ đến $$y$$ để mô tả $$x\mathcal{R}y$$. <br/>

![](data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHhtbG5zOnhsaW5rPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5L3hsaW5rIiB3aWR0aD0iNTMxcHgiIGhlaWdodD0iMzYxcHgiIHZlcnNpb249IjEuMSIgY29udGVudD0iJmx0O214ZmlsZSB1c2VyQWdlbnQ9JnF1b3Q7TW96aWxsYS81LjAgKE1hY2ludG9zaDsgSW50ZWwgTWFjIE9TIFggMTBfMTNfMikgQXBwbGVXZWJLaXQvNTM3LjM2IChLSFRNTCwgbGlrZSBHZWNrbykgQ2hyb21lLzYzLjAuMzIzOS4xMzIgU2FmYXJpLzUzNy4zNiZxdW90OyB2ZXJzaW9uPSZxdW90OzguMC4yJnF1b3Q7IGVkaXRvcj0mcXVvdDt3d3cuZHJhdy5pbyZxdW90OyB0eXBlPSZxdW90O2dvb2dsZSZxdW90OyZndDsmbHQ7ZGlhZ3JhbSBpZD0mcXVvdDs4MmVjZTgwMC0yZjY2LTZhYmYtNzE4YS00ZDUzY2FhMWRmMmQmcXVvdDsgbmFtZT0mcXVvdDtQYWdlLTEmcXVvdDsmZ3Q7N1ZoTmM5b3dFUDAxUGlaalNmNkFJNkZKYzBnNm5VbG4yaDRWVzdFMUZaWXJDekQ5OVpVc0diQnNhRW9nSlcwNWdQUjJ0VnJ0UGo4RUhwck82dmNDbC9rOVR3bnpvSi9XSG5yblFUZ09mZld1Z1pVQndqZzJRQ1pvYWlDd0FSN29EMkpCdXk2YjA1UlVIVWZKT1pPMDdJSUpMd3FTeUE2R2hlRExydHNUWjkxZFM1eVJIdkNRWU5aSFA5TlU1Z1lkdGNmUytDMmhXZDd1REh4cmVjVEp0MHp3ZVdIMzh5QjZhbDdHUE1OdExPdGY1VGpseXkwSVhYdG9LamlYWmpTcnA0VHAwclpsTSt0dWRsalhlUXRTeU9jc2lHR1lZb2dBSWpERmFRQXZiSVFGWm5QU0hpRmlLdGJWRTFjaFZjWnlaYXNVZlovejFuQlJOVDJjS0lmQUwrdU5VWTB5L2ZrQno5UVF6MG8xTGg2cjBwaVljYmt4c1kxbkM2ZDA0VUpWaVl2RFUyaWpQQW9YVVJtWTBBTVp2SFMzbDVYdFUrNU5rVGZ4aS93WDFWTHdRTUhPNEFSN3EvNm1UbkxIaSt5ZzNGMFVkbktBalZ3US9VRDZ5cnpNcVNRUEpVNjBkYW5VVldHNW5ERTFBenBUeXRpVU15N1V2T0NGY3JyQ2pHYUZtaWJxbVNjS3Yxb1FJYWtTczRrMVNGNnU5OVUyVXU5VUM3RFdJQ1h0aE0rSUZDdmwwaTVBVnJhc3JJUFl6cGNia1FTQnhmSXRnWVN0STdiQ25LMWpiOFJKRGF3K1BWT3I0RTZ0ZXBsUTNEVlNzRThaK21UK3IxWmFyUVErOEJFNWcrVFBRYWp1TWYwOUtUbGk5UWJQZmV6TmJzM1gyVituak1IWVVVWXdvSXp4Z0RLaTZCVEtpQWFVMGFrdEtkS0p2aW5yOGpCY1ZUVHBscFBVVkg3WkduL1ZYYmdFdWdqTi9DTVJWQ1dxeTlwMHgyeEEwdDdGMmltaFNvTFBSVUwyM1QvN1pkNHFZemhReFJZVGhHRkpGOTBVaGlwcmQvaklhU01adGRNTTIwV0luT2FZMU8ycTdXdTFFeWdZamJ0MGNMc3NzY2lJN0FWcUdyMCs5bUc5RDA3WCsyaEg3MVdIeFVvdnVQQXZmUmkwaUZtR1F0UUNwK1NNK29YWTFIVGZYZUZQOFFxT0hGNEJkQ0N2eGc2djNIdlZDWGtWSG9GWDJ6d0IwT0ZKTk43Rmt6VWZMMzAvN25BeWlJTlgwS056NXBaN0p3OWRxWGt1dDRCRDBoQzhIcmVpSTJwV2p5TWpFQjZpV3hFSS9uWGRlZ1BjVXRQTnYyWEdmZk9QSkxyK0NRPT0mbHQ7L2RpYWdyYW0mZ3Q7Jmx0Oy9teGZpbGUmZ3Q7Ij48ZGVmcy8+PGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC41LDAuNSkiPjxyZWN0IHg9IjAiIHk9IjYwIiB3aWR0aD0iMTQwIiBoZWlnaHQ9IjI3MCIgZmlsbD0ibm9uZSIgc3Ryb2tlPSIjMDAwMDAwIiBwb2ludGVyLWV2ZW50cz0ibm9uZSIvPjxnIHRyYW5zZm9ybT0idHJhbnNsYXRlKDEyLjUsNjcuNSkiPjxzd2l0Y2g+PGZvcmVpZ25PYmplY3Qgc3R5bGU9Im92ZXJmbG93OnZpc2libGU7IiBwb2ludGVyLWV2ZW50cz0iYWxsIiB3aWR0aD0iMTE0IiBoZWlnaHQ9IjIzOCIgcmVxdWlyZWRGZWF0dXJlcz0iaHR0cDovL3d3dy53My5vcmcvVFIvU1ZHMTEvZmVhdHVyZSNFeHRlbnNpYmlsaXR5Ij48ZGl2IHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5L3hodG1sIiBzdHlsZT0iZGlzcGxheTogaW5saW5lLWJsb2NrOyBmb250LXNpemU6IDEycHg7IGZvbnQtZmFtaWx5OiBIZWx2ZXRpY2E7IGNvbG9yOiByZ2IoMCwgMCwgMCk7IGxpbmUtaGVpZ2h0OiAxLjI7IHZlcnRpY2FsLWFsaWduOiB0b3A7IHdpZHRoOiAxMTRweDsgd2hpdGUtc3BhY2U6IG5vd3JhcDsgd29yZC13cmFwOiBub3JtYWw7IHRleHQtYWxpZ246IGNlbnRlcjsiPjxkaXYgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkveGh0bWwiIHN0eWxlPSJkaXNwbGF5OmlubGluZS1ibG9jazt0ZXh0LWFsaWduOmluaGVyaXQ7dGV4dC1kZWNvcmF0aW9uOmluaGVyaXQ7Ij48Zm9udCBzdHlsZT0iZm9udC1zaXplOiA0MHB4Ij5OYW3CoDwvZm9udD48ZGl2PjxzcGFuIHN0eWxlPSJmb250LXNpemU6IDQwcHgiPjxiciAvPjwvc3Bhbj48ZGl2IHN0eWxlPSJmb250LXNpemU6IDQwcHgiPjxmb250IHN0eWxlPSJmb250LXNpemU6IDQwcHgiPlRow6BuaDwvZm9udD48L2Rpdj48ZGl2IHN0eWxlPSJmb250LXNpemU6IDQwcHgiPjxmb250IHN0eWxlPSJmb250LXNpemU6IDQwcHgiPjxiciAvPjwvZm9udD48L2Rpdj48ZGl2IHN0eWxlPSJmb250LXNpemU6IDQwcHgiPjxmb250IHN0eWxlPSJmb250LXNpemU6IDQwcHgiPkxvbmc8L2ZvbnQ+PC9kaXY+PC9kaXY+PC9kaXY+PC9kaXY+PC9mb3JlaWduT2JqZWN0Pjx0ZXh0IHg9IjU3IiB5PSIxMjUiIGZpbGw9IiMwMDAwMDAiIHRleHQtYW5jaG9yPSJtaWRkbGUiIGZvbnQtc2l6ZT0iMTJweCIgZm9udC1mYW1pbHk9IkhlbHZldGljYSI+W05vdCBzdXBwb3J0ZWQgYnkgdmlld2VyXTwvdGV4dD48L3N3aXRjaD48L2c+PHJlY3QgeD0iMzYwIiB5PSIwIiB3aWR0aD0iMTcwIiBoZWlnaHQ9IjM2MCIgZmlsbD0ibm9uZSIgc3Ryb2tlPSIjMDAwMDAwIiBwb2ludGVyLWV2ZW50cz0ibm9uZSIvPjxnIHRyYW5zZm9ybT0idHJhbnNsYXRlKDM5Mi41LDcuNSkiPjxzd2l0Y2g+PGZvcmVpZ25PYmplY3Qgc3R5bGU9Im92ZXJmbG93OnZpc2libGU7IiBwb2ludGVyLWV2ZW50cz0iYWxsIiB3aWR0aD0iMTA0IiBoZWlnaHQ9IjMzNCIgcmVxdWlyZWRGZWF0dXJlcz0iaHR0cDovL3d3dy53My5vcmcvVFIvU1ZHMTEvZmVhdHVyZSNFeHRlbnNpYmlsaXR5Ij48ZGl2IHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5L3hodG1sIiBzdHlsZT0iZGlzcGxheTogaW5saW5lLWJsb2NrOyBmb250LXNpemU6IDEycHg7IGZvbnQtZmFtaWx5OiBIZWx2ZXRpY2E7IGNvbG9yOiByZ2IoMCwgMCwgMCk7IGxpbmUtaGVpZ2h0OiAxLjI7IHZlcnRpY2FsLWFsaWduOiB0b3A7IHdpZHRoOiAxMDRweDsgd2hpdGUtc3BhY2U6IG5vd3JhcDsgd29yZC13cmFwOiBub3JtYWw7IHRleHQtYWxpZ246IGNlbnRlcjsiPjxkaXYgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkveGh0bWwiIHN0eWxlPSJkaXNwbGF5OmlubGluZS1ibG9jazt0ZXh0LWFsaWduOmluaGVyaXQ7dGV4dC1kZWNvcmF0aW9uOmluaGVyaXQ7Ij48c3BhbiBzdHlsZT0iZm9udC1zaXplOiA0MHB4Ij5MYW48L3NwYW4+PGJyIC8+PGRpdj48c3BhbiBzdHlsZT0iZm9udC1zaXplOiA0MHB4Ij48YnIgLz48L3NwYW4+PGRpdiBzdHlsZT0iZm9udC1zaXplOiA0MHB4Ij48Zm9udCBzdHlsZT0iZm9udC1zaXplOiA0MHB4Ij5UcmFuZzwvZm9udD48L2Rpdj48ZGl2IHN0eWxlPSJmb250LXNpemU6IDQwcHgiPjxmb250IHN0eWxlPSJmb250LXNpemU6IDQwcHgiPjxiciAvPjwvZm9udD48L2Rpdj48ZGl2IHN0eWxlPSJmb250LXNpemU6IDQwcHgiPk1haTwvZGl2PjwvZGl2PjxkaXYgc3R5bGU9ImZvbnQtc2l6ZTogNDBweCI+PGJyIC8+PC9kaXY+PGRpdiBzdHlsZT0iZm9udC1zaXplOiA0MHB4Ij5Iw6A8L2Rpdj48L2Rpdj48L2Rpdj48L2ZvcmVpZ25PYmplY3Q+PHRleHQgeD0iNTIiIHk9IjE3MyIgZmlsbD0iIzAwMDAwMCIgdGV4dC1hbmNob3I9Im1pZGRsZSIgZm9udC1zaXplPSIxMnB4IiBmb250LWZhbWlseT0iSGVsdmV0aWNhIj5bTm90IHN1cHBvcnRlZCBieSB2aWV3ZXJdPC90ZXh0Pjwvc3dpdGNoPjwvZz48cGF0aCBkPSJNIDE0MCA5MyBMIDM1Mi43NSA1MS4yMyIgZmlsbD0ibm9uZSIgc3Ryb2tlPSIjMDAwMDAwIiBzdHJva2UtbWl0ZXJsaW1pdD0iMTAiIHBvaW50ZXItZXZlbnRzPSJub25lIi8+PHBhdGggZD0iTSAzNTcuOSA1MC4yMiBMIDM1MS43MSA1NSBMIDM1Mi43NSA1MS4yMyBMIDM1MC4zNiA0OC4xMyBaIiBmaWxsPSIjMDAwMDAwIiBzdHJva2U9IiMwMDAwMDAiIHN0cm9rZS1taXRlcmxpbWl0PSIxMCIgcG9pbnRlci1ldmVudHM9Im5vbmUiLz48cGF0aCBkPSJNIDE0MCA5NCBMIDM0OS43MSAxMjYuMDQiIGZpbGw9Im5vbmUiIHN0cm9rZT0iIzAwMDAwMCIgc3Ryb2tlLW1pdGVybGltaXQ9IjEwIiBwb2ludGVyLWV2ZW50cz0ibm9uZSIvPjxwYXRoIGQ9Ik0gMzU0Ljg5IDEyNi44MyBMIDM0Ny40NSAxMjkuMjMgTCAzNDkuNzEgMTI2LjA0IEwgMzQ4LjUgMTIyLjMxIFoiIGZpbGw9IiMwMDAwMDAiIHN0cm9rZT0iIzAwMDAwMCIgc3Ryb2tlLW1pdGVybGltaXQ9IjEwIiBwb2ludGVyLWV2ZW50cz0ibm9uZSIvPjxwYXRoIGQ9Ik0gMTQxIDE4OCBMIDM1MS44MyAxMzQuNTYiIGZpbGw9Im5vbmUiIHN0cm9rZT0iIzAwMDAwMCIgc3Ryb2tlLW1pdGVybGltaXQ9IjEwIiBwb2ludGVyLWV2ZW50cz0ibm9uZSIvPjxwYXRoIGQ9Ik0gMzU2LjkyIDEzMy4yNyBMIDM1MC45OSAxMzguMzkgTCAzNTEuODMgMTM0LjU2IEwgMzQ5LjI3IDEzMS42IFoiIGZpbGw9IiMwMDAwMDAiIHN0cm9rZT0iIzAwMDAwMCIgc3Ryb2tlLW1pdGVybGltaXQ9IjEwIiBwb2ludGVyLWV2ZW50cz0ibm9uZSIvPjxwYXRoIGQ9Ik0gMTQxIDI4MCBMIDM0OS44NiAyMjIuNjkiIGZpbGw9Im5vbmUiIHN0cm9rZT0iIzAwMDAwMCIgc3Ryb2tlLW1pdGVybGltaXQ9IjEwIiBwb2ludGVyLWV2ZW50cz0ibm9uZSIvPjxwYXRoIGQ9Ik0gMzU0LjkyIDIyMS4zIEwgMzQ5LjEgMjI2LjUyIEwgMzQ5Ljg2IDIyMi42OSBMIDM0Ny4yNSAyMTkuNzcgWiIgZmlsbD0iIzAwMDAwMCIgc3Ryb2tlPSIjMDAwMDAwIiBzdHJva2UtbWl0ZXJsaW1pdD0iMTAiIHBvaW50ZXItZXZlbnRzPSJub25lIi8+PC9nPjwvc3ZnPg==)

Dựa vào biểu đồ trên, tụi mình có đồ thị $$\Gamma$$ của $$\mathcal(R)$$ là $$\Gamma= \{(Nam,Lan), (Nam,Trang),(Thành,Trang),(Long,Mai)\}$$. Để ý là chiều của mũi tên chỉ có từ $$E$$ đến $$F$$, điều đó nhắc lại cho tụi mình là đồ thị của quan hệ được định nghĩa từ những cặp có thứ tự, khi nói về quan hệ ta chỉ mang tính "một chiều" từ tập đích đến tập nguồn. Điều đó có nghĩa là Nam "thích" Trang nhưng ngược lại Trang "thích" Nam thì chưa chắc. Các bạn nam cũng nên nhớ điều này =)).

Từ đây, tụi mình có thể định nghĩa **quan hệ n ngôi** như sau: <br />

>Với $$E_1, E_2, ..., E_n$$ là những tập hợp. Quan hệ n ngôi là một bộ (n+1) $$(E_1,E_2,...,E_n,\Gamma)$$. Với $$\Gamma \in \mathfrak{P}(E_1 \times E_2 ... \times E_n)$$. <br/>

**Chú ý:** Nếu các bạn để ý thì ở phần định nghĩa quan hệ hai ngôi ở trên thì mình có thêm chữ "đồng nhất", điều này có nghĩa là
tập đích bằng tập nguồn.


Một vài ví dụ về quan hệ <br/>

Quan hệ 3 ngôi: Để diễn tả một quan hệ, trước hết, tụi mình định nghĩa 3 tập hợp như sau: tập hợp 3 chàng trai $$E = \{Dũng,\, Thanh,\, Chinh\}$$, tập hợp 3 cô gái $$F = \{Đào,\, Mai,\, Phượng\}$$, tập họp 4 món quà $$G=\{Hoa,\, Gấu,\, Kẹo,\, Bánh\}$$.
Ta có bộ 3 $$(Dũng,\, Đào,\, Gấu)$$ diễn tả quan hệ 3 ngôi Dũng tặng Đào bằng Gấu. Quan hệ 3 ngôi được dùng khi không thể diễn tả trực tiếp quan hệ giữa các phần tử của các tập hợp. Tương tự đối với các quan hệ n-ngôi khác. Tương tự ví dụ này, ta có ví dụ: Một giáo viên dạy học sinh trong một lớp học nào đó chẳng hạn.

<br/>
Hoặc một ví dụ về toán học, với một quan hệ $$\mathcal{R} = (\mathbb{Z},\, \mathbb{Z},\, \mathbb{Z},\, \Lambda)$$ với một bộ ba số nguyên $$(a,\,b,\,c) \in \Gamma$$ thì $$ a < b < c$$. Vậy $$(1,2,3) \in \Gamma$$, $$(2,1,3) \notin \Gamma$$.

<br/>
Hay cái danh sách học sinh của tụi mình chính là một ví dụ cho quan hệ n-ngôi.

[![Untitled 2](https://farm5.staticflickr.com/4694/39842421762_a4348ef05f_z.jpg)](https://www.flickr.com/photos/142260172@N08/39842421762/in/dateposted-public/ "Untitled 2")

Vậy là tụi mình đã biết được $$x$$ có quan hệ với $$y$$, vậy thì $$y$$ có quan hệ gì với $$x$$? Từ đó, ta bắt đầu nghĩ đến khái niệm _quan hệ ngược_.

<br/>
# Quan hệ ngược
$$E,F$$ là hai tập hợp, $$\mathcal{R}$$ là một quan hệ từ $$E$$ đến $$F$$. Quan hệ ngược của $$\mathcal{R}$$, kí hiệu $$\mathcal{R}^{-1}$$, là quan hệ từ $$F$$ đến $$E$$, được định nghĩa bởi:
> $$\forall (x,y) \in E \times F, y \mathcal{R}^{-1} x \Leftrightarrow x\mathcal{R}y$$

Định nghĩa trên có nghĩa là gì? Kí hiệu $$\Leftrightarrow$$ ở đây chỉ phép toán logic "tương đương". Mệnh đề $$A \Leftrightarrow B $$ là đúng khi hai mệnh đề A,B cùng đúng hoặc cùng sai. Ở đây, $$ y \mathcal{R}^{-1} x \Leftrightarrow x\mathcal{R}y $$ có nghĩa là khi  $$ y \mathcal{R}^{-1} x $$ đúng, mà khi nào thì $$ y \mathcal{R}^{-1} x $$ đúng? Đó là khi cặp $$(y,x)$$ thuộc đồ thị của $$\mathcal{R}^{-1}$$. Khi  $$ y \mathcal{R}^{-1} x $$ đúng thì $$ x\mathcal{R}y $$ đúng điều này có nghĩa là $$(x,y)$$ thuộc đồ thị của $$\mathcal{R}$$. Vậy tóm gọn lại là $$ y \mathcal{R}^{-1} x \Leftrightarrow x\mathcal{R}y$$ có nghĩa khi tụi mình có quan hệ $$x\mathcal{R}y$$ thì cặp $$(y,x)$$ thuộc đồ thị của $$\mathcal{R}^{-1}$$ sẽ cho tụi mình định nghĩa về quan hệ $$\mathcal{R}^{-1}$$.

<br/>
**Ví dụ** '<' là quan hệ 2 ngôi ngược với quan hệ '>' trong $$\mathbb{N}$$. <br/>
Quan hệ có $$\Gamma = \{(1,A), (2,B), (3,C)\}$$ là quan hệ ngược đối với quan hệ có $$\Gamma=\{(A,1), (B,2), (C,3)\}$$ với E là tập hợp chữ số, F là tập hợp chữ cái. <br/>

**Chú ý:** Với mỗi quan hệ bất kì, sẽ luôn tồn tại quan hệ ngược đối với nó.
<br/>

Ví du: Bạn 'crush' T, thì quan hệ ngược lại giữa T với bạn là 'bị crush'. :3  
<br/>


# Các tính chất mà quan hệ hai ngôi có thể có

Một quan hệ hai ngôi $$\mathcal{R}$$ trong một tập hợp $$E$$ được gọi là: <br/>
**phản xạ** khi và chỉ khi: $$\forall x \in E, x\mathcal{R}x$$<br/>
**đối xứng** khi và chỉ khi: $$\forall (x,y) \in E^2, x\mathcal{R}y \Rightarrow y\mathcal{R}x $$ <br/>
**phản đối xứng** khi và chỉ khi: $$\forall (x,y) \in E^2, \begin{cases} x\mathcal{R}y \\ y\mathcal{R}x \end{cases} \Rightarrow x = y $$ <br />
**bắc cầu** khi và chỉ khi: $$\forall (x,y,z) \in E^3, \begin{cases} x\mathcal{R}y \\ y\mathcal{R}z \end{cases} \Rightarrow x\mathcal{R}z $$

<br />
<br/>
Oh trời, một loạt tính chất răn mà nhớ nỗi trời, thực ra mình nghĩ các bạn bây giờ không cần phải thuộc các khái niệm trên, chỉ cần đọc đi đọc lại vài lần là quen thôi. Và mình chú ý là các tính chất trên không phải tất cả quan hệ hai ngôi nào cũng có. Vậy tại sao cần phải biết nó? vì không phải quan hệ hai ngôi nào cũng có tất cả các tính chất trên nên ta có thể dùng các tính chất trên để phân biệt các quan hệ với nhau.

<br/>
Một vài ví dụ về các tính chất trên

phản xạ: trong tập E là tập hợp loài người thì quan hệ "thích" có tính phản xạ. Vì mình nghĩ, tất cả mọi người, ai có cũng "thích" bản thân mình hết.
<br/>
Một chút toán hơn, quan hệ bao hàm $$\subset$$ trong tập hợp $$E$$ chứa tất cả các tập hợp có tính phản xạ, $$A\subset A$$, vì $$\forall x \in A \Rightarrow x \in A$$ =)).
<br/>
đối xứng: quan hệ '=' trong tập hợp số nguyên.
<br/>
phản đối xứng: quan hệ $$\le$$ trong tập hợp số tự nhiên.
<br/>
bắc cầu: quan hệ 'song song' của 2 đường thẳng trong một mặt phẳng. Hay quan hệ 'là họ hàng ruột' trong tập hợp loài người.  <br/>

Tại sao nó giúp chúng ta phân biệt quan hệ?
<br/>
So sánh hai quan hệ $$\in$$ và $$\subset$$, thấy quan hệ $$\in$$ không có tính phản xạ và bắc cầu, ta có đưa ra một phản ví dụ: tập hợp các số nguyên $$\mathbb{Z} = \{...,-1,0,1,...\}$$, ta có thể thấy $$\mathbb{Z}$$ không phải là phần tử của $$\mathbb{Z}$$. Quan hệ $$\in$$ không có tính bắc cầu,
ta cũng có một phản ví dụ: $$3\in \mathbb{Z} \wedge \mathbb{Z} \in A =\{\mathbb{Z}, \mathbb{Q}, \mathbb{R}\}$$ nhưng $$3 \notin A$$. Trong khi đó, quan hệ $$\subset$$ lại có tính phản xạ và bắc cầu. <br/>
Hay trong tập hợp loài người, coi trong tập hợp này mỗi người chỉ được làm một công việc. Ta có quan hệ "là đồng nghiệp" là quan hệ có tính bắt cầu. Còn quan hệ "là người yêu" thì không có tính bắc cầu =)). À mà, nãy giờ lấy ví dụ là về quan hệ hai ngôi nhé các bạn. <br/>
Và các bạn có thể để thấy các ví dụ nãy giờ của mình về quan hệ luôn nhắc đến tập đích và tập nguồn của quan hệ. <br/>
Trước khi về một vài loại quan hệ "đặc biệt" thì tụi mình hãy nói về kiểu quan hệ 'lồng ghép' vào nhau. Kiểu như bạn có quan hệ 'là bạn trai' đối với Phương. Quang có quan hệ 'là người yêu cũ' đối với Phương. Vậy, Bạn có quan hệ gì đối với Quang?<br/>
Từ bài toán kiểu như thế, ta nghĩ đến khái niệm về _quan hệ hợp_.

<br/>
# Quan hệ hợp
_$$E,F,G$$ là các tập hợp. $$\mathcal{R}$$ là một quan hệ từ $$E$$ đến $$F$$. $$\mathcal{S}$$ là một quan hệ từ $$F$$ đến $$G$$. Quan hệ hợp của $$\mathcal{R}$$ và $$\mathcal{S}$$, kí hiệu $$\mathcal{S}\circ \mathcal{R}$$, là quan hệ từ $$E$$ đến $$G$$ được xác định bởi:_
> $$\forall (x,z) \in E \times G, \, x \mathcal{S} \circ \mathcal{R} z \Leftrightarrow \exists y \in F, \begin{cases} x \mathcal{R} y \\ y \mathcal{S} z \end{cases} $$

Ví dụ:
Lấy lại 3 tập hợp E,F,G ở phần quan hệ 3 ngôi ở trên: $$E = \{Dũng,\, Thanh,\, Chinh\}$$, $$F = \{Đào,\, Mai,\, Phượng\}$$, $$G=\{Hoa,\, Gấu,\, Kẹo,\, Bánh\}$$. $$\mathcal{R}$$ là quan hệ "là bạn trai" từ E đến F. $$\mathcal{S}$$ là quan hệ "thích" từ F đến G. Vậy quan hệ "mua" từ E đến G chính là quan hệ hợp $$S \circ R$$

Không biết các bạn có giống mình không lúc đầu cái kí hiệu $$\mathcal{S} \circ \mathcal{R}$$ cảm thấy nó bị ngược ngược răn á =)). Sau ni mình mới để ý là bọn mình sẽ định nghĩ hàm từ quan hệ, và tụi mình cũng sẽ có khái niệm <i>hàm hợp</i>.
Giống như quan hệ hợp, nếu như tụi mình có 2 hàm f, g thì hàm hợp sẽ được kí hiệu: $$f \circ g$$, khi đó ta sẽ có: $$x g \circ f z$$, cái này viết lại $$z = g\circ f(x) = g(f(x))$$. Và cái gì trong ngoặc sẽ thực hiện trước đúng không nào? Nghĩa là
f sẽ "tác động" lên x trước sau đó đến g "tác động" lên f(x). Như vậy, sẽ thấy 'thuận thuận' đúng không? Và việc viết g trước f sẽ không thay đổi thứ tự khi ta thay đổi cách viết hàm hợp. Do đó, việc viết $$\mathcal{S}$$ trước $$\mathcal{R}$$, sẽ
cũng có nghĩa chúng ta sẽ quan tâm đến quan hệ $$x\mathcal{R}y$$ trước quan hệ $$y\mathcal{S}z$$. Vì quan hệ hợp vẫn là quan hệ nên nó vẫn là một tập hợp và quan hệ hợp có đồ thị $$\Gamma = \{(x,z): \exists y \in F, \begin{cases} x \mathcal{R} y \\ y \mathcal{S} z \end{cases} \}$$  <br />
<br/>
Và một trong những điều lưu ý đối với quan hệ hợp là quan hệ ngược đối với một quan hệ hợp.<br/>

<br/>
## Quan hệ ngược của một quan hệ hợp
_$$E,F,G$$ là các tập hợp. $$\mathcal{R}$$ là một quan hệ từ $$E$$ đến $$F$$. $$\mathcal{S}$$ là một quan hệ từ $$F$$ đến $$G$$. Ta có:_
>$$(\mathcal{S} \circ \mathcal{R})^{-1} = \mathcal{R}^{-1} \circ \mathcal{S}^{-1}$$

Chứng minh
<br/>
$$\forall (x,z) \in E \times G$$:<br/>
$$z(\mathcal{S}\circ\mathcal{R})^{-1} \Leftrightarrow x\mathcal{S} \circ \mathcal{R} z \Leftrightarrow \exists y \in F: \begin{cases} x\mathcal{R}y \\ y\mathcal{S}z\end{cases} \Leftrightarrow
\exists y \in F, \begin{cases} z\mathcal{S}^{-1}y \\ y\mathcal{R}^{-1}x\end{cases} \Leftrightarrow \mathcal{R}^{-1} \circ \mathcal{S}^{-1}$$

Cũng hơi dài rồi nên để các nội dung còn lại sang bài viết khác. Chúc các bạn vững bước trên con đường của mình.

<br/>
Ted

<br/>

# Tham khảo

Đại số 1 - Jean-Marie Monier <br/>
Giáo trình toán - thầy Bùi Tuấn Khang<br/>
Naive Set Theory - Paul R. Halmos<br/>
Elements of Set Theory - Herbert B. Enderton<br/>
[N-ary relationship types - vertabelo.com](http://www.vertabelo.com/blog/technical-articles/n-ary-relationship-types)
