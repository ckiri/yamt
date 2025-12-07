{
    "date": "2025-12-05T18:16:11+01:00",
    "title": "Shortcodes",
    "tags": [
	"shortcodes",
	"guide"
    ]
}

A small guide/how-to on YAMT's integrated shortcodes and layouts with simple
examples and their rendered outputs.

{{< toc >}}

----

I think of shortcodes as a custom extension of the default markdown
functionality. Shortcodes let you embedd elements that are cusom
defined[^shortcodes]. Shortcodes are located inside the `layouts/_shortcodes`
directory.

[^shortcodes]: Read more about shortcodes via the official documentation page: <https://gohugo.io/content-management/shortcodes/>.

## Centered

Simply center Elements.

How-To:
```
{{%/* centered */%}}

Hello World!

{{%/* /centered */%}}
```

Rendered example:

{{% centered %}}

Hello World!

{{% /centered %}}

## Figure

Display an image while also specifying its attributes. 

How-To:
```
{{</* figure
  src="/image/path.jpg"
  alt="This text is displayed if the image can't be loaded."
  caption="Your caption"
  loading=lazy
*/>}}
```

Rendered example:

{{< figure
  src="/image/path.jpg"
  alt="This text is displayed if the image can't be loaded."
  caption="Your caption"
  loading=lazy
>}}
 
## Recent-Posts

Render a list of your five most recent blog posts.

How-To:
```
{{</* recent-posts */>}}
```

Rendered example:

{{< recent-posts >}}

## Timeline

Use a timeline to visualize events that need to be ordered in a timely manner.

How-To:
```
{{%/* timeline */%}}

- #### Most recent event:
  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam quaerat.
  
- #### Second most recent event:
  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim aeque doleamus.
  
- #### Something that happend a while back:
  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do.

{{%/* /timeline */%}}
```

Rendered example:

{{% timeline %}}

- #### Most recent event:
  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam quaerat.
  
- #### Second most recent event:
  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim aeque doleamus.
  
- #### Something that happend a while back:
  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do.

{{% /timeline %}}

## TOC

Table of Contents gives you an overview of all headings inside the current
document.

How-To:
```
{{</* toc */>}}
```

Rendered example: *TOC at the [beginning/top](#TableOfContents) of this document*.


## Columns

Using columns helps to better structure a page.

**Note**: columns are not rendered on narrow screens.

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

**Note**: You can add as many columns as you like.

Rendered **without** specifying the `ratio` attribute:

{{% columns %}}

- Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim aeque doleamus animo, cum corpore dolemus, fieri.

- Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim aeque doleamus animo, cum corpore dolemus, fieri tamen permagna accessio potest, si aliquod aeternum et infinitum impendere malum nobis opinemur. Quod idem licet transferre in voluptatem, ut postea variari voluptas distinguique possit, augeri amplificarique non possit. At.

{{% /columns %}}

Columns rendering with `ratio="1:2"`:

{{% columns ratio="1:2" %}}

- Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim aeque doleamus animo, cum corpore dolemus, fieri.

- Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim aeque doleamus animo, cum corpore dolemus, fieri tamen permagna accessio potest, si aliquod aeternum et infinitum impendere malum nobis opinemur. Quod idem licet transferre in voluptatem, ut postea variari voluptas distinguique possit, augeri amplificarique non possit. At.

{{% /columns %}}
