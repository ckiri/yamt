{
    "date": "2025-12-05T18:16:07+01:00",
    "title": "Shortcodes",
    "tags": [
	"shortcodes",
	"guide"
    ]
}

Eine Kurze Einführung zu YAMT's integrierten Shortcodes und Layoutmechanismen.
Beispiele sowie deren Ausgabe werden verständlich dargestellt.

{{< toc >}}

----

Unter Shortcodes kann man sich einen erweiterten Funktionsumfang von
Markdown vorstellen. Dabei kann man eigene *Funktionen* erstellen und
diese in Dokumente integrieren[^shortcodes]. Shorcodes befinden sich im
`layouts/shortcodes` Ordner.

[^shortcodes]: Offizielle Shortcodes Dokumentation: <https://gohugo.io/content-management/shortcodes/>.

## Zentriert

Element(e) zentrieren.

How-To:
```
{{%/* centered */%}}

Hello World!

{{%/* /centered */%}}
```

Beispieldarstellung:

{{% centered %}}

Hello World!

{{% /centered %}}

## Abbildungen

Abbildungen sowie deren Attribute anzeigen. 

How-To:
```
{{</* figure
  src="/image/path.jpg"
  alt="Wenn dieser Text sichtbar ist, konnte das Bild nicht geladen werden."
  caption="Beschreibung"
  loading=lazy
*/>}}
```

Beispieldarstellung:

{{< figure
  src="/image/path.jpg"
  alt="Wenn dieser Text sichtbar ist, konnte das Bild nicht geladen werden."
  caption="Beschreibung"
  loading=lazy
>}}
 
## Neuste Beiträge

Eine Liste der letzten fünf Blog-Beiträge anzeigen lassen.

How-To:
```
{{</* recent-posts */>}}
```

Beispieldarstellung:

{{< recent-posts >}}

## Timeline

Nützlich um z.B. einen Lebenslauf oder zeitlichen Ablauf darzustellen.

How-To:
```
{{%/* timeline */%}}

- ### Das neuste Ereignis:
  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam quaerat.
  
- ### Das Ereignis davor:
  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim aeque doleamus.
  
- ### Ein Ereignis dass schon länger her ist:
  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do.

{{%/* /timeline */%}}
```

Beispieldarstellung:

{{% timeline %}}

- #### Das neuste Ereignis:
  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam quaerat.
  
- #### Das Ereignis davor:
  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim aeque doleamus.
  
- #### Ein Ereignis dass schon länger her ist:
  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do.

{{% /timeline %}}

## Inhaltsverzeichnis

Anzeigen aller Überschriften/Kapitel in einem Beitrag.

How-To:
```
{{</* toc */>}}
```

Beispieldarstellung: *Inhaltsverzeichnis zu [Beginn](#TableOfContents) des Beitrags*.

## Spalten

Spalten erlauben es Inhalte strukturierter darzustellen. Der Shortcode `columns` hat
nur das eine Attribute `ratio` mit dem die Breitenverhältnis spezifiziert werden
kann.

**Anmerkung**: Spalten werden auf schmalen Bildschirmen **nicht** dargestellt.

How-To:
```
{{%/* columns ratio="1:2" */%}}

Contents inside the left column

</div>
<div>

Contents inside the right column

</div>
</div>

{{%/* /columns */%}}
```

**Anmerkung**: Es können beliebig viele Spalten hinzugefügt werden.

Spaltenlayout **ohne** Angabe von `ratio`:

{{% columns %}}

- Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim aeque doleamus animo, cum corpore dolemus, fieri.

- Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim aeque doleamus animo, cum corpore dolemus, fieri tamen permagna accessio potest, si aliquod aeternum et infinitum impendere malum nobis opinemur. Quod idem licet transferre in voluptatem, ut postea variari voluptas distinguique possit, augeri amplificarique non possit. At.

{{% /columns %}}

Spaltenlayout mit `ratio="1:2"`:

{{% columns ratio="1:2" %}}

- Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim aeque doleamus animo, cum corpore dolemus, fieri.

- Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim aeque doleamus animo, cum corpore dolemus, fieri tamen permagna accessio potest, si aliquod aeternum et infinitum impendere malum nobis opinemur. Quod idem licet transferre in voluptatem, ut postea variari voluptas distinguique possit, augeri amplificarique non possit. At.

{{% /columns %}}
