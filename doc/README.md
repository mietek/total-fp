Elementary Strong Functional Programming: Summary
=================================================

> _**NOTE:**  This is an archival version of the [ESFP website](http://www.cs.kent.ac.uk/people/staff/dat/esfp/)._
>
> _Unfortunately, Telford’s and Kaganovsky’s home pages have not been included in the Internet Archive._
>
> _**Additional literature**_
>
> * _Total Functional Programming ([PDF](pdf/2004-turner-total-functional-programming.pdf))_

[Professor D. A. Turner](http://www.cs.kent.ac.uk/people/staff/dat/index.html), Computing Laboratory, University of Kent, Canterbury CT2 7NF, UK.

The project, funded by the UK Engineering and Physical Sciences Research Council (EPSRC) from 14.10.96 to 13.10.99 under grant GR/L03279, was undertaken to investigate the practical viability of a discipline of strong functional programming proposed in [8]. The research associate was [~~Alastair Telford~~](http://web.archive.org/web/*/http://www.cs.kent.ac.uk/people/staff/ajt/).

In strong functional programming all expressions are guaranteed to have normal form. In order to retain the possibility of programming with infinite structures, which is an essential feature of pure functional languages such as Haskell, a key part of the methodology of [8] is to maintain a separation in the type system between _data_, which is known to be finite, and _codata_ which is permitted to be infinite. This may be contrasted with the usual situation in lazy functional programming in which infinite lists for example, have the same compile-time type as ordinary finite lists.

The separation between data and codata leads to a distinction between recursion, which to be “safe” must be **well-founded**, and _corecursion_, which must be **productive**. Our main achievements are the development of techniques of abstract interpretation, which we demonstrate can recognise at compile time sufficiently large classes of safe recursion and corecursion to permit a wide range of standard functional algorithms to be accepted in their “natural” form. Previous work on automatic termination detection, based for example on _Walther recursion_, has required even quite simple algorithms, for example _gcd_, to be rewritten in a special style. We believe these results substantially advance the practical viability of strong functional programming.

Our techniques for recognising productivity in corecursive definitions of infinitary structures are presented in [1,2] and those for well-founded recursion over finitary data structures in [3,4].

[~~Alexander Kaganovsky~~](http://web.archive.org/web/*/http://www.cs.kent.ac.uk/people/rpg/ayk1/), a PhD student associated with the group, did outstanding work on the investigation of an important class of corecursive algorithms over infinite lists of integers. The problem area he studied is the efficient implementation of _unbounded precision arithmetic_ on real and complex numbers represented as streams of signed digits. His results, which include algorithms for many analytic functions and are a significant advance on previous work, are described in two papers and his thesis [5,6,7].

For further information contact the [investigator](http://www.cs.kent.ac.uk/people/staff/dat/index.html) at the University of Kent.

Final report. ([PDF](pdf/2000-turner-final-report-elementary-strong-functional-programming.pdf))


References
----------

1. A. J. Telford, D. A. Turner, [“Ensuring Streams Flow”](http://www.cs.ukc.ac.uk/pubs/1997/499/) Johnson, ed, Algebraic Methodology and Software Technology — AMAST ’97. LNCS 1349, pages 509-523, Springer, 1997. ([PDF](pdf/2000-turner-final-report-elementary-strong-functional-programming.pdf))
2. A. J. Telford, D. A. Turner, [“Ensuring the Productivity of Infinite Structures”](http://www.cs.ukc.ac.uk/pubs/1997/551/) Technical Report TR 14-97, 37 pages, Computing Laboratory, University of Kent, March 1998. ([PDF](pdf/1997-telford-turner-ensuring-the-productivity-of-infinite-structures.pdf))
3. A. J. Telford, D. A. Turner, [“Ensuring Termination in ESFP”](http://www.jucs.org/jucs_6_4/ensuring_termination_in_esfp), Journal of Universal Computer Science 6(4):474-488, April 2000 (originally presented at 15th British Colloquium in Theoretical Computer Science, Keele, April 1999). ([PDF](pdf/2000-telford-turner-ensuring-termination-in-esfp.pdf))
4. A. J. Telford, D. A. Turner, [“A Hierarchy of Languages with Strong Termination Properties”](http://www.cs.ukc.ac.uk/pubs/2000/964/), Technical Report TR 2-00, 66 pages, University of Kent Computing Laboratory, January 2000. ([PDF](pdf/2000-telford-turner-a-hierarchy-of-languages-with-strong-termination-properties.pdf))
5. A. Y. Kaganovsky, [“Computing With Exact Real Numbers in a Radix-r System”](http://www.cs.kent.ac.uk/pubs/1999/947/), Electronic Notes in Theoretical Computer Science, Volume 13, 27 Pages, Elsevier 1998. Revised version available as Technical Report TR 19-99, 30 pages, Computing Laboratory, University of Kent, October 1999. ([PDF](pdf/1999-kaganovsky-computing-with-exact-real-numbers-in-a-radix-r-system.pdf))
6. A. Y. Kaganovsky, [“Exact Complex Arithmetic in an Imaginary Radix System”](http://www.cs.ukc.ac.uk/pubs/1999/902/), Technical Report TR 9-99, 30 pages, Computing Laboratory, University of Kent, July 1999. ([PDF](pdf/1999-kaganovsky-exact-complex-arithmetic-in-an-imaginary-radix-system.pdf))
7. A. Y. Kaganovsky, [“Exact Computing in Positional Weighted Systems”](http://www.cs.kent.ac.uk/pubs/2004/1850/), University of Kent PhD Thesis, 212 pages, March 2001. ([PDF](pdf/2001-kaganovsky-exact-computing-in-positional-weighted-systems.pdf))
8. D. A. Turner, [“Elementary Strong Functional Programming”](http://www.cs.kent.ac.uk/people/staff/dat/esfp/nijmegen.html). In R. Plasmeijer, P. Hartel, eds, First International Symposium on Functional Programming Languages in Education, Nijmegen, Netherlands, December 1995. Springer Lecture Notes in Computer Science, vol 1022:1-13, 1995. ([PDF](pdf/1995-turner-elementary-strong-functional-programming.pdf))
