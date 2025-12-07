{
    "date": "2025-12-06T15:17:02+01:00",
    "title": "Render-Test",
    "tags": [
	"theme",
	"test",
	"guide"
    ]
}

Render-Test zum Testen der Darstellung typischer Markdownfunktionen.

{{< toc >}}

---

# H1 Überschrift

Einleitungsparagraph mit **fettem Text**, *kursivem Text* und `Inline Code`.  
Zeilenumbruch von der oberen Zeile (zwei Leerzeichen am Ende der Zeile). Hier
ein normaler Zeilenumbruch. ~~Durchgestrichen~~.

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam quaerat voluptatem.

## H2 Unterüberschrift

Ein regulärer Paragraph. Lorem ipsum to check wrapping and spacing.

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim aeque doleamus animo, cum corpore dolemus, fieri tamen permagna accessio potest, si.

### H3 Unterunterüberschrift

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam quaerat voluptatem[^1]. Ut enim aeque doleamus animo, cum corpore dolemus, fieri tamen permagna accessio potest, si aliquod aeternum et infinitum impendere malum nobis opinemur[^2]. Quod idem licet transferre in voluptatem, ut[^3].

[^1]: Testen der Fußzeile. Lorem ipsum dolor sit amet.

[^2]: Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam quaerat.

[^3]: Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do.

- Ungeordnete Liste erster Punkt
- Ungeordnete Liste zweiter Punkt
  - Verschachtelte Liste Punkt A
  - Verschachtelte Liste Punkt B

1. Geordnet, erstes Item
2. Geordnet, zweites Item
3. Geordnet, drittes Item

- [x] Aufgabe erledigt
- [ ] Aufgabe noch nicht erledigt
- [ ] Eine anderer offener Punkt

## Links

Inline Link: [Beispiel Link](https://ckiri.com "Chris' Webseite").

[md-guide]: https://www.markdownguide.org

## Zitate (Blockquotes)

> Einfaches Zitat auf einer Zeile zum Testen des Stylings.
>
> Mehrfach-Zeilen-Zitat mit **fettem Text**, *kursivem Text* und einem
> [Link](https://ckiri.com).
>
> > Verschachteltes Zitat auf zweitem Level.

## Codeblöcke

Inline code: `console.log("hello markdown");`.

Indented code block:

    function indentedExample() {
        return 42;
    }

Codeblock:
```JavaScript {linenos=inline hl_lines=["4-5", 7] style=none}
function fencedExample(name) {
  console.log(Hello, someSemanticallyMeaninglessButVeryLongIdentifier ${name}!);
}

console.log(Hi)

fencedExample("World");
```

## Tabellen

Einfache Tabelle:

| Spalte A | Spalte B | Spalte C |
| -------- | -------- | -------- |
| A1       | B1       | C1       |
| A2       | B2       | C2       |

Tabelle mit Ausrichtung:

| Linksbündig   | Zentriert     | Rechtsbündig  |
| :---------    | :----------:  | -----------:  |
| Text          | Text          | Text          |
| Längerer Text | Längerer Text | Längerer Text |

| Lorem                                                                                                                                                                    | ipsum                                                                                                                                                                                                       |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim aeque doleamus. | Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim aeque doleamus.                                    |
| Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore.                                                                     | Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim aeque doleamus animo, cum corpore dolemus, fieri.  |
| someSemanticallyMeaninglessButVeryLongIdentifier                                                                                                                         |                                                                                                                                                 someSemanticallyMeaninglessButVeryLongIdentifier                                                             |
---

## Trennlinie

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim aeque doleamus animo, cum corpore dolemus, fieri.

Aufteilen der Inhalte durch Verwendung horizontaler Linien:

---

Ein weiterer Abschnitt nach einer Trennlinie.

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam quaerat.

---

## Listen mit Paragraph und Codeblock

- Listenelement mit eigenem Paragraphen.  
  Still the same list item, different paragraph.

- Listenelement mit Codeblock:
  ```
  function fencedExample(name) {
    console.log(Hello, someSemanticallyMeaninglessButVeryLongIdentifier ${name}!);
  }
  
  fencedExample("World");
  ```

## Katex

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam
quaerat voluptatem. This is inline Notation: \(a^2 + b^2 = c^2\). Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed
do eiusmod tempor incididunt ut labore et dolore magnam aliquam

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam
eine weitere inline Notation mit Brüchen und Wurzel: \(\sqrt{1 + \frac{1}{x^2}} \cdot e^{i\pi} + \int_0^1 x^2 \, dx\).
do eiusmod tempor incididunt ut labore et dolore magnam aliquam Lorem ipsum dolor sit amet, consectetur adipiscing elit,
sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam

Blockgleichung mit Grenzen:

\[
\lim_{x \to 0} \frac{\sin x}{x} = 1
\]

Blockgleichung mit Summe und Produkt:

\[
\sum_{n=1}^{\infty} \frac{1}{n^2}
\quad\text{und}\quad
\prod_{k=1}^{n} \left(1 + \frac{1}{k}\right)
\]

\[
f(x) = \frac{ax^2 + bx + c}{\sqrt{1 + x^2}} \,,\qquad
\hat{\theta},\ \bar{x},\ \vec{v},\ \overrightarrow{AB}
\]

Einfache Matrix:

\[
A = \begin{bmatrix}
1 & 2 & 3 \\
4 & 5 & 6
\end{bmatrix}
\]

Spaltenvektor:

\[
\mathbf{v} = \begin{pmatrix}
v_1 \\ v_2 \\ v_3
\end{pmatrix}
\]

\[
f(x) =
\begin{cases}
x^2, & \text{wenn } x \ge 0, \\
-x,  & \text{wenn } x < 0
\end{cases}
\]

\[
\alpha, \beta, \gamma, \delta, \lambda, \mu, \sigma, \Omega,\quad
\forall x \in \mathbb{R},\ \exists y \le 0:\ x + y = 0
\]
