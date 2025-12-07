{
    "date": "2025-12-06T15:17:06+01:00",
    "title": "Render Test",
    "tags": [
	"theme",
	"test",
	"guide"
    ]
}

Rendering test to showcase Markdown functions and styling.

{{< toc >}}

---

# H1 Heading

Intro paragraph with **bold text**, *italic text*, and `inline code`.  
Hard line break above (two spaces at end of line). Normal line break here.
~~Strik-trough~~.

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam quaerat voluptatem.

## H2 Heading

Regular paragraph. Lorem ipsum to check wrapping and spacing.

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim aeque doleamus animo, cum corpore dolemus, fieri tamen permagna accessio potest, si.

### H3 Heading

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam quaerat voluptatem[^1]. Ut enim aeque doleamus animo, cum corpore dolemus, fieri tamen permagna accessio potest, si aliquod aeternum et infinitum impendere malum nobis opinemur[^2]. Quod idem licet transferre in voluptatem, ut[^3].

[^1]: Lorem ipsum dolor sit amet.

[^2]: Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam quaerat.

[^3]: Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do.

- Unordered list item one
- Unordered list item two
  - Nested list item A
  - Nested list item B

1. Ordered item one
2. Ordered item two
3. Ordered item three

- [x] Completed task
- [ ] Open task
- [ ] Another open task

## Links

Inline link: [Example link](https://ckiri.com "Chris' Website").

[md-guide]: https://www.markdownguide.org

## Blockquotes

> Single-line blockquote to test quote styling.
>
> Multi-line blockquote with **bold text**, *italic text*, and a [link](https://example.com).
>
> > Nested blockquote level 2.

## Code blocks

Inline code: `console.log("hello markdown");`.

Indented code block:

    function indentedExample() {
        return 42;
    }

Code block:
```JavaScript {linenos=inline hl_lines=["4-5", 7] style=none}
function fencedExample(name) {
  console.log(Hello, someSemanticallyMeaninglessButVeryLongIdentifier ${name}!);
}

console.log(Hi)

fencedExample("World");
```

## Tables

Simple table:

| Column A | Column B | Column C |
| -------- | -------- | -------- |
| A1       | B1       | C1       |
| A2       | B2       | C2       |

Table with alignment:

| Left align | Center align | Right align |
| :--------- | :----------: | ----------: |
| text       | text         | text        |
| longer     | longer       | longer      |

| Lorem                                                                                                                                                                    | ipsum                                                                                                                                                                                                       |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim aeque doleamus. | Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim aeque doleamus.                                    |
| Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore.                                                                     | Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim aeque doleamus animo, cum corpore dolemus, fieri.  |
| someSemanticallyMeaninglessButVeryLongIdentifier                                                                                                                         |                                                                                                                                                 someSemanticallyMeaninglessButVeryLongIdentifier                                                             |
---

## Horizontal rules

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim aeque doleamus animo, cum corpore dolemus, fieri.

Above and below are thematic breaks:

---

Another section of content after the rule.

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam quaerat.

---

## Lists with paragraphs and code

- List item with a paragraph.

  Still the same list item, different paragraph.

- List item with code:

## Katex

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam
quaerat voluptatem. This is inline math: \(a^2 + b^2 = c^2\). Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed
do eiusmod tempor incididunt ut labore et dolore magnam aliquam

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam
Another inline expression with fractions and roots: \(\sqrt{1 + \frac{1}{x^2}} \cdot e^{i\pi} + \int_0^1 x^2 \, dx\).
do eiusmod tempor incididunt ut labore et dolore magnam aliquam Lorem ipsum dolor sit amet, consectetur adipiscing elit,
sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam

Block equation with limits:

\[
\lim_{x \to 0} \frac{\sin x}{x} = 1
\]

Block equation with sum and product:

\[
\sum_{n=1}^{\infty} \frac{1}{n^2}
\quad\text{and}\quad
\prod_{k=1}^{n} \left(1 + \frac{1}{k}\right)
\]

\[
f(x) = \frac{ax^2 + bx + c}{\sqrt{1 + x^2}} \,,\qquad
\hat{\theta},\ \bar{x},\ \vec{v},\ \overrightarrow{AB}
\]

Simple matrix:

\[
A = \begin{bmatrix}
1 & 2 & 3 \\
4 & 5 & 6
\end{bmatrix}
\]

Column vector:

\[
\mathbf{v} = \begin{pmatrix}
v_1 \\ v_2 \\ v_3
\end{pmatrix}
\]

\[
f(x) =
\begin{cases}
x^2, & \text{if } x \ge 0, \\
-x,  & \text{if } x < 0
\end{cases}
\]

\[
\alpha, \beta, \gamma, \delta, \lambda, \mu, \sigma, \Omega,\quad
\forall x \in \mathbb{R},\ \exists y \le 0:\ x + y = 0
\]
