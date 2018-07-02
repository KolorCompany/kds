---
title: 'Maths and formulas'
tags: tag1
order: 20
---
Kramdown markdown parser comes with optional support for LaTeX to PNG rendering via [MathJax](https://www.mathjax.org) within math blocks. See the Kramdown documentation on [math blocks](http://kramdown.gettalong.org/syntax.html#math-blocks) and [math support](http://kramdown.gettalong.org/converter/html.html#math-support) for more details. MathJax requires you to include JavaScript or CSS to render the LaTeX, e.g.

​$$ f(x) = 3x²+2 $$

```
$$ f(x) = 3x²+2 $$
```

---


$$ x = {-b \pm \sqrt{b^2-4ac} \over 2a} $$

```
$$ x = {-b \pm \sqrt{b^2-4ac} \over 2a} $$
```


---


When $$a \ne 0$$, there are two solutions to $$(ax^2 + bx + c = 0)$$ and they are
$$x = {-b \pm \sqrt{b^2-4ac} \over 2a}.$$

```
When $$a \ne 0$$, there are two solutions to $$(ax^2 + bx + c = 0)$$ and they are
$$x = {-b \pm \sqrt{b^2-4ac} \over 2a}.$$
```
