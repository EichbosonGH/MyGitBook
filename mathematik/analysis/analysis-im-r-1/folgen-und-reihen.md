---
hidden: true
layout:
  width: default
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
  metadata:
    visible: true
  tags:
    visible: true
---

# Folgen und Reihen

## Definitionen

<table data-full-width="false"><thead><tr><th width="197.13330078125">Name</th><th width="287.63330078125" align="center">Definition</th><th>Bemerkung</th></tr></thead><tbody><tr><td><strong>Folge</strong></td><td align="center"><span class="math">(a_k)_{k\in\N} = (a_0,a_1,a_2,\ldots)</span></td><td>Abbildung <span class="math">a_k:\N→\R</span></td></tr><tr><td><strong>Reihe</strong></td><td align="center"><span class="math">(s_n)_{n\in\N}~~\text{mit}~~ s_n = \sum\limits_{k=0}^{n}a_k</span></td><td>Folge von Partialsummen</td></tr><tr><td><strong>Teleskop-Summe</strong></td><td align="center"><span class="math">a_k = a_0 + \sum\limits_{j=1}^{k} (a_j-a_{j-1})</span></td><td><ul><li>Darstellung Folgeglied <br>als Reihe</li><li>nützlich um Reihen <br>über <span class="math">a_k</span> ﻿ aufzusummieren</li></ul></td></tr><tr><td><strong>Fakultät</strong></td><td align="center"><span class="math">n! = \prod\limits_{k=1}^{n} k = 1\cdot2\cdot\ldots\cdot n</span></td><td><ul><li><span class="math">0!=1</span></li></ul></td></tr><tr><td><strong>Binomial-Koeffizient</strong></td><td align="center"><span class="math">\dbinom{n}{k} = \dbinom{n}{n-k}  =  \dfrac{n!}{k!(n-k)!}</span></td><td><ul><li>Falls <span class="math">0\leq k\leq n</span></li><li>sonst <span class="math">0</span></li></ul></td></tr></tbody></table>

## Sätze

<table><thead><tr><th width="271.63336181640625">Name</th><th align="center">Aussage</th></tr></thead><tbody><tr><td><a data-mention href="folgen-und-reihen.md#quadratzahlen">#quadratzahlen</a></td><td align="center"><span class="math">k^2 = \sum\limits_{j=1}^{k}(2j-1)</span></td></tr><tr><td>Arithmetische Reihe</td><td align="center"><span class="math">\sum\limits_{k=1}^{n}k =\dfrac{n(n+1)}{2} =\dfrac{n^2+n}{2}</span></td></tr><tr><td>Summe über Quadratzahlen</td><td align="center"><span class="math">\sum\limits_{k=1}^{n}k^2= \dfrac{n(n+1)(2n+1)}{6}= \dfrac{n^3}{3} +\dfrac{n^2}{2} +\dfrac{n}{6}</span></td></tr><tr><td>Summe über kubische Zahlen</td><td align="center"><span class="math">\sum\limits_{k=1}^{n}k^3= \bigg[\dfrac{n(n+1)}{2}\bigg]^2= \dfrac{n^4}{4} +\dfrac{n^3}{2} +\dfrac{n^2}{4}</span></td></tr><tr><td>Geometrische Reihe</td><td align="center"><span class="math">\sum\limits_{k=0}^n x^k  = \dfrac{1-x^{n+1}}{1-x} ~,~x\neq1</span></td></tr><tr><td>Binomischer Lehrsatz</td><td align="center">• <span class="math">(x+y)^n =\sum\limits_{k=0}^{n} \dbinom{n}{k}~x^{n-k}~y^k</span></td></tr><tr><td>“Trinomischer Lehrsatz”</td><td align="center">• <span class="math">(x+y+z)^n =\sum\limits_{k_1+k_2+k_3=n} \dfrac{n!}{k_1!k_2!k_3!}~ x^{k_1}y^{k_2}z^{k_3}</span></td></tr><tr><td>Summe über Binom.-Koeff.</td><td align="center">•  <span class="math">\sum\limits_{k=0}^{n}\dbinom{n}{k} = 2^n </span><br>•  <span class="math">\sum\limits_{m=k}^{n}\dbinom{m}{k} = \dbinom{n+1}{k+1} </span></td></tr></tbody></table>

### Bedingte Summation

#### Behauptung

$$
s_n =\sum\limits_{k=1}^{n} \Big(\sum\limits_{j=1}^{k} a_j\Big) =  \sum\limits_{j=1}^{n} (n-j+1)\,a_j
$$

#### Beweis

* Wechsel von zeilenweiser zu spaltenweiser Summation
* in jeder Spalte sinkt die Zahl der Elemente um 1

<p align="center"><span class="math">\begin{matrix} k \backslash j &#x26; 1 &#x26; 2 &#x26; \ldots &#x26; n  \\[0.5em] 1 &#x26; a_1 \\[0.5em] 2 &#x26; a_1 &#x26; a_2 \\[0.5em] ... \\[0.5em] n &#x26; a_1 &#x26; a_2 &#x26; \ldots &#x26; a_n \end{matrix}</span></p>

* Damit folgt

$$
\begin{align*}
\sum_{k=1}^{n}
\bigg(\sum_{j=1}^{k}a_j\bigg)
&= 
\sum_{j=1}^{n}
\bigg(\sum_{k=j}^{n}a_j\bigg)
= \sum_{j=1}^{n}a_j
\bigg(\sum_{k=j}^{n}1\bigg)
\\[2em]
&= \sum_{j=1}^{n}a_j
(n-j+1) \quad \text{q.e.d.}
\end{align*}
$$

### Quadratzahlen

$$
k^2 = \sum\limits_{j=1}^{k}(2j-1)
$$

#### Beweis

* Ein Beispiel für Teleskop-Summe

$$
\begin{align*}
a_k &= a_0 
+ \sum_{i=1}^{k}(a_i-a_{i-1})
~\text{mit}~a_i=i^2\
\\[2em]
k^2 &= 0
+ \sum_{j=1}^{k}\Big[j^2-(j-1)^2\Big] 
= \sum_{j=1}^{k}2j-1
\end{align*}
$$

### Arithmetische Reihe

$$
\sum\limits_{k=1}^n k 
= \frac{n(n+1)}{2}
= \frac{n^2+n}{2}
$$

#### Beweis

* Teleskop-Summe der Summanden

$$
\begin{align*}
a_k &= a_0 
+ \sum_{i=1}^{k}(a_i-a_{i-1})
~\text{mit}~ a_i=i
\\[2em]
k &= 0
+ \sum_{j=1}^{k}\Big[j-(j-1)\Big] 
= \sum_{j=1}^{k}1
\end{align*}
$$

asd

$$
\begin{alignat*}
a
\end{alignat*}
$$

$$
\begin{alignat*}
\sum_{k=1}^{n}k
&= \sum_{k=1}^{n}
\Big(\sum_{j=1}^{k}1\Big)
= \sum_{j=1}^{n}(n-j+1)
\end{align*}
$$

$$
\begin{alignat}{2}
   10&x+&3&y=2\\
   3&x+&13&y=4
\end{alignat}
$$
