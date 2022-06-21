# test
place to play

### and, right now, to practice MathJax

This tutorial is from https://math.meta.stackexchange.com/questions/5020/mathjax-basic-tutorial-and-quick-reference. Just
copied the code over here. But it doesn't seem to display as well in GitHub Markdown as it does in StackOverflow Markdown.


1. To see how any formula was written in any question or answer, including this one, right-click on the expression and choose "Show Math As > TeX Commands". (When you do this, the '$' will not display. Make sure you add these: see the next point. There are also [other ways][2] to view the code for the formula or the whole post.)

2. **For inline formulas, enclose the formula in `$`…`$`.  For displayed formulas, use `$$`…`$$`.**  
These render differently. For example,
type  
`$\sum_{i=0}^n i^2 = \frac{(n^2+n)(2n+1)}{6}$`  
to show $\sum_{i=0}^n i^2 = \frac{(n^2+n)(2n+1)}{6}$ (which is inline mode) or  type  
`$$\sum_{i=0}^n i^2 = \frac{(n^2+n)(2n+1)}{6}$$`   
to show
$$\sum_{i=0}^n i^2 = \frac{(n^2+n)(2n+1)}{6}$$
(which is display mode).

3. For **Greek letters**, use `\alpha`, `\beta`, …, `\omega`: $\alpha$, $\beta$, …, $\omega$.  For uppercase letters, use `\Gamma`, `\Delta`, …, `\Omega`: $\Gamma$, $\Delta$, …, $\Omega$. For other Greek capital letters, use Latin $A, B, E$, and so on. Some Greek letters have variant forms:
`\epsilon \varepsilon` $\epsilon$, $\varepsilon$, `\phi \varphi` $\phi$, $\varphi$, and others. 

4. For **superscripts and subscripts**, use `^` and `_`.  For example, `x_i^2`: $x_i^2$, `\log_2 x`: $\log_2 x$.

5. **Groups**. Superscripts, subscripts, and other operations apply only to the next “group”. A “group” is either a single symbol, or any formula surrounded by curly braces `{`…`}`.  If you do `10^10`, you will get a surprise: $10^10$. But `10^{10}` gives what you probably wanted: $10^{10}$. Use curly braces to delimit a formula to which a superscript or subscript applies: `x^5^6` is an error;  `{x^y}^z` is ${x^y}^z$, and `x^{y^z}` is $x^{y^z}$. Observe the differences between `x_i^2` $x_i^2$, `x_{i^2}` $x_{i^2}$ and `{x_i}^2` ${x_i}^2$.

6. **Parentheses** Ordinary symbols `()[]` make parentheses and brackets $(2+3)[4+4]$. Use `\{` and `\}` for curly braces $\{\}$.

    These do *not* scale with the formula in between, so if you write `(\frac{\sqrt x}{y^3})` the parentheses will be too small: $(\frac{\sqrt x}{y^3})$.    Using `\left(`…`\right)` will make the sizes adjust automatically to the formula they enclose: `\left(\frac{\sqrt x}{y^3}\right)` is $\left(\frac{\sqrt x}{y^3}\right)$.

   `\left` and`\right` apply to all the following sorts of parentheses: `(` and `)` $(x)$, `[` and `]` $[x]$, `\{` and `\}` $\{ x \}$, `|` $|x|$, `\vert` $\vert x \vert$, `\Vert` $\Vert x \Vert$, `\langle` and `\rangle` $\langle x \rangle$,  `\lceil` and `\rceil` $\lceil x \rceil$, and `\lfloor` and `\rfloor` $\lfloor x \rfloor$. `\middle` can be used to add additional dividers. There are also invisible parentheses, denoted by `.`: `\left.\frac12\right\rbrace` is $\left.\frac12\right\rbrace$.

7. **Sums and integrals** `\sum` and `\int`; the subscript is the lower limit and the superscript is the upper limit, so for example `\sum_1^n` $\sum_1^n$. Don't forget `{`…`}` if the limits are more than a single symbol.  For example, `\sum_{i=0}^\infty i^2` is $\sum_{i=0}^\infty i^2$. Similarly, `\prod` $\prod$, `\int` $\int$, `\bigcup` $\bigcup$, `\bigcap` $\bigcap$, `\iint` $\iint$, `\iiint` $\iiint$, `\idotsint` $\idotsint$.

8. **Fractions** There are [three ways to make these][3]. `\frac ab` applies to the next two groups, and produces $\frac ab$; for more complicated numerators and denominators use `{`…`}`: `\frac{a+1}{b+1}` is $\frac{a+1}{b+1}$. If the numerator and denominator are complicated, you may prefer `\over`, which splits up the group that it is in: `{a+1\over b+1}` is ${a+1\over b+1}$.
For continued fractions, [use `\cfrac` instead of `\frac`][4].

9. **Fonts** 

  * Use `\mathbb` or `\Bbb` for "blackboard bold": $\mathbb{CHNQRZ}$.
  * Use `\mathbf` for boldface: $\mathbf{ABCDEFGHIJKLMNOPQRSTUVWXYZ}$  $\mathbf{abcdefghijklmnopqrstuvwxyz}$. 
    * For expression based characters, use `\boldsymbol` instead: $\boldsymbol{\alpha}$
  * Use `\mathit` for italics: $\mathit{ABCDEFGHIJKLMNOPQRSTUVWXYZ}$ $\mathit{abcdefghijklmnopqrstuvwxyz}$.
  * Use `\pmb` for boldfaced italics: $\pmb{ABCDEFGHIJKLMNOPQRSTUVWXYZ}$ $\pmb{abcdefghijklmnopqrstuvwxyz}$.
  * Use `\mathtt` for "typewriter" font: $\mathtt{ABCDEFGHIJKLMNOPQRSTUVWXYZ}$ $\mathtt{abcdefghijklmnopqrstuvwxyz}$.
  * Use `\mathrm` for roman font: $\mathrm{ABCDEFGHIJKLMNOPQRSTUVWXYZ}$  $\mathrm{abcdefghijklmnopqrstuvwxyz}$.
  * Use `\mathsf` for sans-serif font: $\mathsf{ABCDEFGHIJKLMNOPQRSTUVWXYZ}$  $\mathsf{abcdefghijklmnopqrstuvwxyz}$.
  * Use `\mathcal` for "calligraphic" letters: $\mathcal{ ABCDEFGHIJKLMNOPQRSTUVWXYZ}$ (Uppercase only.)
  * Use `\mathscr` for script letters: $\mathscr{ABCDEFGHIJKLMNOPQRSTUVWXYZ}$ $\mathscr{abcdefghijklmnopqrstuvwxyz}$
  * Use `\mathfrak` for "Fraktur" (old German style) letters: $\mathfrak{ABCDEFGHIJKLMNOPQRSTUVWXYZ}$ $\mathfrak{abcdefghijklmnopqrstuvwxyz}$.

10. **Radical signs / roots** Use `sqrt`, which adjusts to the size of its argument: `\sqrt{x^3}` $\sqrt{x^3}$; `\sqrt[3]{\frac xy}` $\sqrt[3]{\frac xy}$. For complicated expressions, consider using `{...}^{1/2}` instead.

11. Some **special functions** such as "lim", "sin", "max", "ln", and so on are normally set in roman font instead of italic font. Use `\lim`, `\sin`, etc. to make these: `\sin x` $\sin x$, not `sin x` $sin x$. Use subscripts to attach a notation to `\lim`: `\lim_{x\to 0}` $$\lim_{x\to 0}$$ Nonstandard function names can be set with `\operatorname{foo}(x)` $\operatorname{foo}(x)$.

12. There are a very large number of **special symbols and notations**, too many to list here; see the short listing [$\LaTeX$ and $\mathcal{A}_{\Large\mathcal{M}}\mathcal{S}$-$\LaTeX$ Symbols][5] prepared by Dr. Emre Sermutlu, or the exhaustive listing [The Comprehensive $\LaTeX$ Symbol List][6] by Scott Pakin. Some of the most common include: 
  * `\lt \gt \le \leq \leqq \leqslant \ge \geq \geqq \geqslant \neq` $\lt$, $\gt$, $\le$, $\leq$, $\leqq$, $\leqslant$, $\ge$, $\geq$, $\geqq$, $\geqslant$, $\neq$.  You can use `\not` to put a slash through almost anything: `\not\lt` $\not\lt$ but it often looks bad.
  * `\times \div \pm \mp` $\times$, $\div$, $\pm$, $\mp$. `\cdot` is a centered dot: $x\cdot y$
  * `\cup \cap \setminus \subset \subseteq \subsetneq \supset \in \notin \emptyset \varnothing` $\cup$, $\cap$, $\setminus$, $\subset$, $\subseteq$, $\subsetneq$, $\supset$, $\in$, $\notin$, $\emptyset$, $\varnothing$ 
  * `{n+1 \choose 2k}` or `\binom{n+1}{2k}` ${n+1 \choose 2k}$ 
  * `\to \gets \rightarrow \leftarrow \Rightarrow \Leftarrow \mapsto \implies \iff` $\to$, $\gets$, $\rightarrow$, $\leftarrow$, $\Rightarrow$, $\Leftarrow$, $\mapsto$, $\implies$, $\iff$
  * `\land \lor \lnot \forall \exists \top \bot \vdash \vDash` $\land$, $\lor$, $\lnot$, $\forall$, $\exists$, $\top$, $\bot$, $\vdash$, $\vDash$
  * `\star \circledast \ast \oplus \circ \bullet` $\star$, $\circledast$, $\ast$, $\oplus$, $\circ$, $\bullet$ 
  * `\approx \sim \simeq \cong \equiv \prec \lhd \rhd` $\approx$, $\sim $, $\simeq$, $\cong$, $\equiv$, $\prec$, $\lhd$, $\rhd$ 
  * `\infty \aleph_0` $\infty\, \aleph_0$ `\nabla \partial` $\nabla$, $\partial$ `\Im \Re` $\Im$, $\Re$
  * For modular equivalence, use `\pmod` like this: `a\equiv b\pmod n` $a\equiv b\pmod n$.  For the binary mod operator, use `\bmod` like this: `a\bmod 17` $a\bmod 17$.
  * Use `\dots` for the triple dots in $a_1, a_2, \dots, a_n$ and  $a_1+a_2+\dots+a_n$
  * Script lowercase l is `\ell` $\ell$.

    [Detexify][7] lets you draw a symbol on a web page and then lists the $\TeX$ symbols that seem to resemble it.  These are not guaranteed to work in MathJax, but it's a good place to start.  To check that a command is supported, note that MathJax.org maintains a [list of currently supported $\LaTeX$ commands][8], and one can also check Dr. Carol JVF Burns's page of [$\TeX$ Commands Available in MathJax][9].

13. **Spaces** MathJax usually decides for itself how to space formulas, using a complex set of rules. Putting extra literal spaces into formulas will not change the amount of space MathJax puts in: `a␣b` and `a␣␣␣␣b` are both $a    b$. To add more space, use `\,` for a thin space $a\,b$; `\;` for a wider space $a\;b$.  `\quad` and `\qquad` are large spaces: $a\quad b$, $a\qquad b$.

    To set plain text, use `\text{…}`: $\{x\in s\mid x\text{ is extra large}\}$. You can nest `$…$` inside of `\text{…}`, for example to access spaces.

14. **Accents and diacritical marks** Use `\hat` for a single symbol $\hat x$, `\widehat` for a larger formula $\widehat{xy}$. If you make it too wide, it will look silly. Similarly, there are `\bar` $\bar x$ and `\overline` $\overline{xyz}$, and `\vec` $\vec x$ and `\overrightarrow` $\overrightarrow{xy}$ and `\overleftrightarrow` $\overleftrightarrow{xy}$. For dots, as in $\frac d{dx}x\dot x =  \dot x^2 +  x\ddot x$,  use `\dot` and `\ddot`.

15. Special characters  used for MathJax interpreting can be escaped using the `\` character: \\\$ $\$$, `\{` $\{$, `\}` $\}$,  `\_` $\_$, `\#` $\#$, `\&` $\&$. If you want `\` itself, you should use `\backslash` (symbol) or `\setminus` ([binary operation][10]) for $\backslash$, because `\\` is for a new line. 

(Tutorial ends here.)

-------------

It is important that this note be reasonably short and not suffer from too much bloat. To include more topics, please create short addenda and post them as answers instead of inserting them into this post.

## Contents

Alphabetical list of links to MathJax topics, by title:

 - [Absolute values and norms][11] • [Additional symbolic decorations][12] • [Aligning Equations][13]
 - [Alternative Ways of Writing in LaTeX][14] • [Annotations of reasoning][15] • [Arbitrary operators][16]
 - [Arrays][17] • [Big braces][18] • [Colors][19]
 - [Commutative diagrams][20] • [Continued fractions][4] • [Crossing things out][21]
 - [Definitions by cases (piecewise functions)][22] • [Degree symbol][23] • [Display style][24]
 - [Equation numbering][25] • [Fussy spacing issues][26] • [Highlighting expressions][27]
 - [Left and right arrows][28] • [Limits][29] • [Linear programming][30]
 - [Long division][31] • [Math Programming][32] • [Matrices][33]
 - [Markov Chains][34] • [Mixing code and MathJax formatting on lines][35] • [The \newcommand function][36] 
 - [Numbering Equations][37] • [Overlaying Symbols][38] • [Packs of cards][39]
 - [Symbols][40]
• [System of equations][41] • [Tables][42]
 - [Tags and references][43] • [Tensor indices][44] • [Units][45]
 - [Vertical spacing][46]


  [1]: https://www.mathelounge.de/509545/mathjax-latex-basic-tutorial-und-referenz-deutsch
  [2]: /questions/659/how-to-view-latex-source-of-equations
  [3]: /questions/12978/should-dfrac-be-edited-in
  [4]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/5058#5058
  [5]: https://pic.plover.com/MISC/symbols.pdf
  [6]: https://www.ctan.org/tex-archive/info/symbols/comprehensive/symbols-a4.pdf
  [7]: https://detexify.kirelabs.org/classify.html
  [8]: https://docs.mathjax.org/en/latest/input/tex/macros/index.html
  [9]: https://www.onemathematicalcat.org/MathJaxDocumentation/TeXSyntax.htm
  [10]: https://tex.stackexchange.com/questions/511328/difference-between-commands-setminus-and-backslash/511332#511332
  [11]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/15078#15078
  [12]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/13081#13081
  [13]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/5024#5024
  [14]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/27910#27910
  [15]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/21258#21258
  [16]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/15077#15077
  [17]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/5044#5044
  [18]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/11423#11423
  [19]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/10116#10116
  [20]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/16888#16888
  [21]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/13183#13183
  [22]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/5025#5025
  [23]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/19678#19678
  [24]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/25054#25054
  [25]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/27793#27793
  [26]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/5057#5057
  [27]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/22395#22395
  [28]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/13310#13310
  [29]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/12850#12850
  [30]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/27756#27756
  [31]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/21096#21096
  [32]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/27756#27756
  [33]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/5023#5023
  [34]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/31141#31141
  [35]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/25251#25251
  [36]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/11638#11638
  [37]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/11491#11491
  [38]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/32210#32210
  [39]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/22516#22516
  [40]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/11284#11284
  [41]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/6267#6267
  [42]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/29979#29979
  [43]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/11491#11491
  [44]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/30661#30661
  [45]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/27212#27212
  [46]: /questions/5020/mathjax-basic-tutorial-and-quick-reference/25048#25048
