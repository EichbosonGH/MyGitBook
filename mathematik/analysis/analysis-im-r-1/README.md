---
layout:
  width: wide
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

# Analysis im R(1)

***

## Allgemeines

* $$n\in\N = \{0,1,2,3,4,\ldots\}$$
* $$x,y \in \R$$
* Für alle Funktionen gilt: $$y=f(x): D\to\R,~D\sub\R$$

## [Folgen und Reihen](folgen-und-reihen.md)

### Definitionen&#x20;

<table><thead><tr><th width="204.73333740234375">Name</th><th width="297.7666015625">Definition</th><th>Bemerkung</th></tr></thead><tbody><tr><td>Folge</td><td><span class="math">(a_k)_{k\in\N} = (a_0,a_1,a_2,\ldots)</span></td><td>Abbildung <span class="math">a_k:\N→\R</span></td></tr><tr><td>Reihe</td><td><span class="math">(s_n)_{n\in\N}~~\text{mit}~~ s_n = \sum\limits_{k=0}^{n}a_k</span></td><td>Folge von Partialsummen</td></tr><tr><td>Teleskop-Summe</td><td><span class="math">a_k = a_0 + \sum\limits_{j=1}^{k} (a_j-a_{j-1})</span></td><td><ul><li>Darstellung eines Folgeglieds als Reihe</li><li>nützlich um Reihen über <span class="math">a_k</span> ﻿ aufzusummieren</li></ul></td></tr><tr><td>Fakultät</td><td><span class="math">n! = \prod\limits_{k=1}^{n} k = 1\cdot2\cdot\ldots\cdot n</span></td><td><span class="math">0!=1</span></td></tr><tr><td>Binomial-Koeffizient</td><td><span class="math">\dbinom{n}{k} = \dbinom{n}{n-k}  =  \dfrac{n!}{k!(n-k)!}</span></td><td><span class="math">\text{Falls}~~ 0\leq k\leq n</span></td></tr></tbody></table>

### Sätze

<table><thead><tr><th width="291.66668701171875"></th><th></th></tr></thead><tbody><tr><td>"Bedingte Summation"</td><td><span class="math">\sum\limits_{k=1}^{n} \Big(\sum\limits_{j=1}^{k} a_j\Big) =  \sum\limits_{j=1}^{n} (n-j+1)\,a_j</span></td></tr><tr><td>Arithmetische Reihe</td><td><span class="math">\sum\limits_{k=1}^{n}k =\dfrac{n(n+1)}{2} =\dfrac{n^2+n}{2}</span></td></tr><tr><td>Quadratzahlen</td><td><span class="math">k^2 = \sum\limits_{j=1}^{k}(2j-1)</span></td></tr><tr><td>Summe über Quadratzahlen</td><td><span class="math">\sum\limits_{k=1}^{n}k^2= \dfrac{n(n+1)(2n+1)}{6}= \dfrac{n^3}{3} +\dfrac{n^2}{2} +\dfrac{n}{6}</span></td></tr><tr><td>Summe über kubische Zahlen</td><td><span class="math">\sum\limits_{k=1}^{n}k^3= \bigg[\dfrac{n(n+1)}{2}\bigg]^2= \dfrac{n^4}{4} +\dfrac{n^3}{2} +\dfrac{n^2}{4}</span></td></tr><tr><td>Geometrische Reihe</td><td><span class="math">\sum\limits_{k=0}^n x^k  = \dfrac{1-x^{n+1}}{1-x} ~,~x\neq1</span></td></tr><tr><td>Binomischer Lehrsatz</td><td>• <span class="math">(x+y)^n =\sum\limits_{k=0}^{n} \dbinom{n}{k}~x^{n-k}~y^k</span></td></tr><tr><td>“Trinomischer Lehrsatz”</td><td>• <span class="math">(x+y+z)^n =\sum\limits_{k_1+k_2+k_3=n} \dfrac{n!}{k_1!k_2!k_3!}~ x^{k_1}y^{k_2}z^{k_3}</span></td></tr><tr><td>Summe über Binom.-Koeff.</td><td>•  <span class="math">\sum\limits_{k=0}^{n}\dbinom{n}{k} = 2^n </span><br>•  <span class="math">\sum\limits_{m=k}^{n}\dbinom{m}{k} = \dbinom{n+1}{k+1} </span></td></tr><tr><td></td><td>o  <span class="math">\sum\limits_{m=k}^{n}\dbinom{m}{k} = \dbinom{n+1}{k+1}</span><br>o <span class="math">\sum\limits_{m=k}^{n}\dbinom{m}{k} = \dbinom{n+1}{k+1}</span></td></tr></tbody></table>

Test $$(x+y+z)^n =\sum\limits_{k_1+k_2+k_3=n} \dfrac{n!}{k_1!k_2!k_3!}~ x^{k_1}y^{k_2}z^{k_3}$$

## Differentialrechnung

## Integralrechnung&#x20;

