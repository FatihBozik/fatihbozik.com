---
layout: post
title: Bulanık Mantık'a Giriş
tags: [Bulanık Mantık, Bulanık Küme]
comments: true
---

{% include _toc.html %}

## Bulanık Küme

Sınırları kesin çizgilerle belirlenmemiş kümelere denir. Bir bulanık kümeyi oluşturan her bir eleman, *kısmen* o kümenin üyesi olabilir. Yani her bir elemanın üyelik derecesi vardır.

<!-- more -->

Bulanık kümeler çeşitli şekillerde gösterilebilir. Kümelerin şekli üçgen, dörtgen olabileceği gibi herhangi bir çokgen olabilir.
<div style="float:left;"><img style="max-width: 50%;" src="/images/bulanik-mantika-giris/triangle form.png" alt="Üçgen formu" height="100"><img style="max-width: 50%;" src="/images/bulanik-mantika-giris/trapezoid form.png" alt="Yamuk formu" height="100"></div>
<br/> <br/> <br/> <br/> <br/> <br/> <br/> <br/> <br/> <br/> <br/>
<div style="float:left;"><img style="max-width: 50%;" src="/images/bulanik-mantika-giris/gaussian form.png" alt="Gaussian formu" height="100"><img style="max-width: 50%;" src="/images/bulanik-mantika-giris/generalized bell form.png" alt="Generalized Bell formu" height="100"></div> <br/> <br/> <br/> <br/> <br/> <br/> <br/> <br/> <br/> <br/> <br/> <br/>

* x ekseni kümemizin elemanlarını gösteriyor. Örneğin kümemizin uzun boylular kümesi olduğunu farz edersek x eksenimizdeki değerler 1,70, 1,80, .. gibi değerler olacak.

* y ekseni x değerlerinin kümenin elemanı olma olasılığını gösteriyor. Bu olasılık 1 ise kümenin elemanıdır, 0 ise kümenin elemanı değildir.

* 0 - 0.5 olasılıkla kümenin elemanı olan x değerlerine `kümenin zayıf elemanıdır` deriz.
 
* 0.5 -  1 olasılıkla kümenin elemanı olan x değerlerine ise `büyük olasılıkla kümenin elemanıdır` deriz.

<br/>
Bir kümeyi bulanık kümelerle ifade etmek istersek aşağıdaki gibi bulanık kümelere bölebiliriz.
<img style="max-width: 100%;" src="/images/bulanik-mantika-giris/bulanık kümeler.png" alt="Bulanık Kümeler" height="300"> <br/>


## Bulanık Kümeler Üzerinde Tanımlanmış İşlemler

Birazdan zikredeceğimiz işlemler <u>üçgen</u> formundaki bulanık kümeler arasında geçerlidir.

* \\( A_\alpha :\\) A bulanık kümesini temsil ediyor. \\( a_1(\alpha) \\) ile \\( a_2(\alpha) \\) A bulanık kümesinin parçalı fonksiyonlarından sırasıyla soldakini ve sağdakini temsil ediyor. <br/>
* \\( B_\alpha :\\) B bulanık kümesini temsil ediyor. \\( b_1(\alpha) \\) ile \\( b_2(\alpha) \\) B bulanık kümesinin parçalı fonksiyonlarından sırasıyla soldakini ve sağdakini temsil ediyor. <br/>

### Bulanık Kümelerde Toplama İşlemi

\begin{align}
A_\alpha \  (+) \  B_\alpha &= [a_1(\alpha), \  a_2(\alpha)] \  (+) \  [b_1(\alpha), \  b_2(\alpha)] \newline
&= [a_1(\alpha) + b_1(\alpha), \ a_2(\alpha) + b_2(\alpha)]
\end{align} 
<br/>

`Örnek:` Aşağıdaki A ve B bulanık kümeleri veriliyor. \\( A \ (+) \ B \\) bulanık kümesinin denklemini bulun ve grafik üzerinde gösterin. <br/>
<img style="max-width: 100%;" src="/images/bulanik-mantika-giris/sample1.png" height="300"> <br/> <br/>

`Çözüm:` <br/> <br/> 

\begin{align}
\forall x \in R : \newline
\mu_A(x) &= \frac{(x+5)}{3}, \quad & -5 \leq x \leq -2 \newline
		 &= \frac{-(x-1)}{3},\quad & -2 \leq x \leq 1 \newline
		 &= 0, \quad & di \breve{g} er \newline \newline
\mu_B(x) &= \frac{(x+3)}{7}, \quad & -3 \leq x \leq 4 \newline
		 &= \frac{-(x-12)}{8},\quad & 4 \leq x \leq 12 \newline
		 &= 0, \quad & di \breve{g} er
\end{align}
<br/>

\begin{align}
\alpha& = \frac{(x+5)}{3}&
\alpha& = \frac{-(x-1)}{3} \newline
x& = 3\alpha - 5&
x& = -3\alpha + 1 \newline
A_\alpha& = [a_1(\alpha), \ a_2(\alpha)] \newline
        & = [3\alpha - 5, \ -3\alpha + 1] \newline
\newline \newline
\alpha& = \frac{(x+3)}{7}&
\alpha& = \frac{-(x-12)}{8} \newline
x& = 7\alpha - 3&
x& = -8\alpha + 12 \newline 
B_\alpha& = [b_1(\alpha), \ b_2(\alpha)] \newline
        & = [7\alpha - 3, \ -8\alpha + 12] \newline
\newline
A_\alpha \  (+) \ B_\alpha& = [a_1(\alpha) + b_1(\alpha), \ a_2(\alpha) + b_2(\alpha)] \newline
		     & = [3\alpha - 5, \ -3\alpha + 1] \ (+) \ [7\alpha - 3, \ -8\alpha + 12] \newline
		     & = [10\alpha - 8, -11\alpha + 13]
\end{align}
<br/><br/>

\begin{align}
\mu_{A(+)B}(x) &= \frac{(x+8)}{10}, \quad & -8 \leq x \leq 2 \newline
	       &= \frac{-(x-13)}{11},\quad & 2 \leq x \leq 13 \newline
	       &= 0, \quad & di \breve{g} er
\end{align}<br/>
<img style="max-width: 100%;" src="/images/bulanik-mantika-giris/sample1_result.png" height="300"> <br/> <br/>

### Bulanık Kümelerde Çıkarma İşlemi
Bulanık kümelerde toplama yaparken yaptığımız şeyin aynısını yapıyoruz. Parçalı fonksiyonların artan kısımlarını ve azalan kısımlarını birbirleriyle işleme sokuyoruz. 
<br/>
\begin{align}
A_\alpha \  (-) \  B_\alpha &= [a_1(\alpha), \  a_2(\alpha)] \  (-) \  [b_1(\alpha), \  b_2(\alpha)] \newline
&= [a_1(\alpha) - b_2(\alpha), \ a_2(\alpha) - b_1(\alpha)]
\end{align} 
<br/>

`Örnek:` Aşağıdaki A ve B bulanık kümeleri veriliyor. \\( A \ (-) \ B \\) bulanık kümesinin denklemini bulun ve grafik üzerinde gösterin. <br/>
<img style="max-width: 100%;" src="/images/bulanik-mantika-giris/sample2.png" height="300"> <br/> <br/>

`Çözüm:` <br/> <br/> 
\begin{align}
\mu_A(x) &= \frac{(x-7)}{7}, \quad & 7 \leq x \leq 14 \newline
		 &= \frac{-(x-19)}{5},\quad & 14 \leq x \leq 19 \newline
		 &= 0, \quad & di \breve{g} er \newline
\newline
\mu_B(x) &= \frac{(x-3)}{2}, \quad & 3 \leq x \leq 5 \newline
		 &= \frac{-(x-10)}{5},\quad & 5 \leq x \leq 10 \newline
		 &= 0, \quad & di \breve{g} er
\end{align}
<br/>

\begin{align}
\alpha& = \frac{(x-7)}{7}&
\alpha& = \frac{-(x-19)}{5} \newline
x& = 7\alpha + 7&
x& = -5\alpha + 19 \newline
A_\alpha& = [a_1(\alpha), \ a_2(\alpha)] \newline
        & = [7\alpha + 7, \ -5\alpha + 19] \newline
\newline \newline
\alpha& = \frac{(x-3)}{2}&
\alpha& = \frac{-(x-10)}{5} \newline
x& = 2\alpha + 3&
x& = -5\alpha + 10 \newline 
B_\alpha& = [b_1(\alpha), \ b_2(\alpha)] \newline
        & = [2\alpha + 3, \ -5\alpha + 10] \newline
\newline
A_\alpha \  (-) \ B_\alpha& = [a_1(\alpha) - b_2(\alpha), \ a_2(\alpha) - b_1(\alpha)] \newline
		     & = [7\alpha + 7, \ -5\alpha + 19] \ (-) \ [2\alpha + 3, \ -5\alpha + 10] \newline
		     & = [12\alpha - 3, -7\alpha + 16]
\end{align}
<br/><br/>

\begin{align}
\mu_{A(-)B}(x) &= \frac{(x+3)}{12}, \quad & -3 \leq x \leq 9 \newline
	       &= \frac{-(x-16)}{7},\quad & 9 \leq x \leq 16 \newline
	       &= 0, \quad & di \breve{g} er
\end{align}<br/>

<img style="max-width: 100%;" src="/images/bulanik-mantika-giris/sample2_result.png" height="300"> <br/> <br/>

### Bulanık Kümelerde Çarpma İşlemi
\begin{align}
A_\alpha \  (.) \  B_\alpha &= [a_1(\alpha), \  a_2(\alpha)] \  (.) \  [b_1(\alpha), \  b_2(\alpha)] \newline
&= [a_1(\alpha) \ . \  b_1(\alpha), \ a_2(\alpha) \  . \ b_2(\alpha)]
\end{align} 
<br/>

`Örnek:` Aşağıdaki A ve B bulanık kümeleri veriliyor. \\( A \ (.) \ B \\) bulanık kümesinin denklemini bulun ve grafik üzerinde gösterin. <br/>
<img style="max-width: 100%;" src="/images/bulanik-mantika-giris/sample3.png" height="300"> <br/> <br/>

`Çözüm:` <br/> <br/> 
\begin{align}
\mu_A(x) &= x-2, \quad & 2 \leq x \leq 3 \newline
		 &= \frac{-(x-5)}{2},\quad & 3 \leq x \leq 5 \newline
		 &= 0, \quad & di \breve{g} er \newline \newline
\mu_B(x) &= \frac{(x-3)}{2}, \quad & 3 \leq x \leq 5 \newline
		 &= -(x-6),\quad & 5 \leq x \leq 6 \newline
		 &= 0, \quad & di \breve{g} er
\end{align}
<br/>

\begin{align}
\alpha& = x-2&
\alpha& = \frac{-(x-5)}{2} \newline
x& = \alpha + 2&
x& = -2\alpha + 5 \newline
A_\alpha& = [a_1(\alpha), \ a_2(\alpha)] \newline
        & = [\alpha + 2, \ -2\alpha + 5] \newline
\newline \newline
\alpha& = \frac{(x-3)}{2}&
\alpha& = -(x-6) \newline
x& = 2\alpha + 3&
x& = -\alpha + 6 \newline
B_\alpha& = [b_1(\alpha), \ b_2(\alpha)] \newline
        & = [2\alpha + 3, \ -\alpha + 6] \newline
\newline
A_\alpha \  (.) \ B_\alpha& = [a_1(\alpha) \ . \ b_1(\alpha), \ a_2(\alpha) \ . \ b_2(\alpha)] \newline
		     & = [\alpha + 2, \ -2\alpha + 5] \ (.) \ [2\alpha + 3, \ -\alpha + 6] \newline
		     & = [2\alpha^{2} + 7\alpha + 6,\ 2\alpha^{2} -17\alpha + 30]
\end{align}
<br/><br/>

\begin{align}
\mu_{A\ (.)\ B}(x) &= \frac{-7+\sqrt{1+8x}}{4}, \quad & 6 \leq x \leq 15 \newline
	       &= \frac{17 - \sqrt{49 + 8x}}{4},\quad & 15 \leq x \leq 30 \newline
	       &= 0, \quad & di \breve{g} er
\end{align}<br/>

<img style="max-width: 100%;" src="/images/bulanik-mantika-giris/sample3_result.png" height="300"> <br/> <br/>

### Bulanık Kümelerde Bölme İşlemi
\begin{align}
A_\alpha \  (:) \  B_\alpha &= [a_1(\alpha), \  a_2(\alpha)] \  (:) \  [b_1(\alpha), \  b_2(\alpha)] \newline
&= [a_1(\alpha) \ / \  b_2(\alpha), \ a_2(\alpha) \  / \ b_1(\alpha)], \quad b_2(\alpha) > 0
\end{align} 
<br/>

`Örnek:` Aşağıdaki A ve B bulanık kümeleri veriliyor. \\( A \ (:) \ B \\) bulanık kümesinin denklemini bulun ve grafik üzerinde gösterin. <br/>
<img style="max-width: 100%;" src="/images/bulanik-mantika-giris/sample4.png" height="300"> <br/> <br/>

`Çözüm:` <br/> <br/> 
\begin{align}
\mu_A(x) &= \frac{(x-18)}{4}, \quad & 18 \leq x \leq 22 \newline
		 &= \frac{-(x-33)}{11},\quad & 22 \leq x \leq 33 \newline
		 &= 0, \quad & di \breve{g} er \newline \newline
\mu_B(x) &= x-5, \quad & 5 \leq x \leq 6 \newline
		 &= \frac{-(x-8)}{2},\quad & 6 \leq x \leq 8 \newline
		 &= 0, \quad & di \breve{g} er
\end{align}
<br/>

\begin{align}
\alpha& = \frac{x-18}{4}&
\alpha& = \frac{-(x-33)}{11} \newline
x& = 4\alpha + 18&
x& = -11\alpha + 33 \newline
A_\alpha& = [a_1(\alpha), \ a_2(\alpha)] \newline
        & = [4\alpha + 18, \ -11\alpha + 33] \newline
\newline \newline
\alpha& = x-5&
\alpha& = \frac{-(x-8)}{2} \newline
x& = \alpha + 5&
x& = -2\alpha + 8 \newline
B_\alpha& = [b_1(\alpha), \ b_2(\alpha)] \newline
        & = [\alpha + 5, \ -2\alpha + 8] \newline
\newline
A_\alpha \  (:) \ B_\alpha& = [a_1(\alpha) \ : \ b_2(\alpha), \ a_2(\alpha) \ : \ b_1(\alpha)] \newline
		     & = [4\alpha + 18, \ -11\alpha + 33] \ (:) \ [\alpha + 5, \ -2\alpha + 8] \newline
		     & = \left[\frac{4\alpha + 18}{-2\alpha + 8},\ \frac{-11\alpha + 33}{-11\alpha + 13}\right]
\end{align}
<br/><br/>

\begin{align}
\mu_{A\ (:)\ B}(x) &= \frac{(8x-18)}{(2x+4)}, \quad & \frac{9}{4} \leq x \leq \frac{11}{3} \newline
	       &= \frac{(-5x+33)}{(x+11)},\quad & \frac{11}{3} \leq x \leq \frac{33}{5} \newline
	       &= 0, \quad & di \breve{g} er
\end{align}<br/>
<img style="max-width: 100%;" src="/images/bulanik-mantika-giris/sample4_result.png" height="300"> <br/> <br/>

### Bulanık Kümelerde Minimum ve Maksimum İşlemleri

\\( A \ (\land) \ B : \\)  A minimum B <br/>
\\( A \ (\lor) \ B : \\)  A maksimum B <br/>

Belirli bir \\( \alpha \\) için \\( x \\) değerlerine bakılır. \\( A \ (\land) \ B \\) için x değeri küçük olanlar, \\( A \ (\lor) \ B \\) için büyük olanlar seçilir.

`Örnek:` Aşağıdaki A ve B bulanık kümeleri veriliyor. \\( A \ (\land) \ B \\) ve \\( A \ (\lor) \ B \\) bulanık kümelerinin denklemini bulun ve grafik üzerinde gösterin. <br/>
<img style="max-width: 100%;" src="/images/bulanik-mantika-giris/sample5.png" height="300"> <br/> <br/>

`Çözüm:` <br/> <br/> 
\begin{align}
\mu_A(x) &= \frac{(x+2)}{2}, \quad & -2 \leq x \leq 0 \newline
		 &= \frac{-(x-6)}{6},\quad & 0 \leq x \leq 6 \newline
		 &= 0, \quad & di \breve{g} er \newline
A_\alpha &= [2\alpha - 2, -6\alpha + 6] \newline
\newline
\mu_B(x) &= \frac{(x+4)}{7}, \quad & -4 \leq x \leq 3 \newline
		 &= \frac{-(x-5)}{2},\quad & 3 \leq x \leq 5 \newline
		 &= 0, \quad & di \breve{g} er \newline
B_\alpha &= [7\alpha - 4, -2\alpha + 5]
\end{align}
<br/>

\begin{align}
A_\alpha \land B_\alpha &= [(2\alpha-2) \land (7\alpha-4),\ (-6\alpha+6) \land (-2\alpha+5)] \newline
A_\alpha \land B_\alpha &= [7\alpha-4, \ -2\alpha + 5], \quad 0 \leq \alpha \leq 0.25 \newline
						&= [7\alpha-4, \ -6\alpha + 6], \quad 0.25 \leq \alpha \leq 0.4 \newline
						&= [2\alpha-2, \ -6\alpha + 6], \quad 0.4 \leq \alpha \leq 1 \newline
\newline
A_\alpha \lor B_\alpha &= [(2\alpha-2) \lor (7\alpha-4),\ (-6\alpha+6) \lor (-2\alpha+5)] \newline
A_\alpha \lor B_\alpha &= [2\alpha-2, \ -6\alpha + 6], \quad 0 \leq \alpha \leq 0.25 \newline
					   &= [2\alpha-2, \ -2\alpha + 5], \quad 0.25 \leq \alpha \leq 0.4 \newline
					   &= [7\alpha-4, \ -2\alpha + 5], \quad 0.4 \leq \alpha \leq 1
\end{align}
<br/><br/>

<img style="max-width: 100%;" src="/images/bulanik-mantika-giris/sample5_result.png" height="300"> <br/> <br/>

\begin{align}
\mu_{A(\land)B}(x) &= \frac{(x+4)}{7}, \quad & -4 \leq x \leq -1.2 \newline
	               &= \frac{(x+2)}{2},\quad & -1.2 \leq x \leq 0 \newline
	               &= \frac{-(x-6)}{6},\quad & 0 \leq x \leq 4.5 \newline
	               &= \frac{-(x-5)}{2},\quad & 4.5 \leq x \leq 5 \newline
	               &= 0, \quad & di \breve{g} er \newline
\newline
\mu_{A(\lor)B}(x)  &= \frac{(x+2)}{2}, \quad & -2 \leq x \leq -1.2 \newline
	               &= \frac{(x+4)}{7},\quad & -1.2 \leq x \leq 3 \newline
	               &= \frac{-(x-5)}{2},\quad & 3 \leq x \leq 4.5 \newline
	               &= \frac{-(x-6)}{6},\quad & 4.5 \leq x \leq 6 \newline
	               &= 0, \quad & di \breve{g} er
\end{align}

<br/><br/><br/><br/>

**Kaynaklar:**

* [Kaufman, A. 1991. Introduction to Fuzzy Arithmetic](http://www.amazon.com/Introduction-Fuzzy-Arithmetic-Arnold-Kaufman/dp/0442008996/) <br/>
* [YRD.DOÇ.DR.Oğuzhan Öztaş Bulanık Mantık ders notları](http://www.oguzhanoztas.com/bm/1_Bulanik_Mantik.pdf)
