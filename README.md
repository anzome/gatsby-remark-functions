# gatsby-remark-function

A work-in-progress plugin I'll use to avoid placing duplicated markup and texts.

The plugin will allow me to reuse complex and repeatable parts as through the generic snippets.

```text
# About pictures

Sometime picture is more than the <img/> tag.

FN:picture(
    url: '/omg.png',
    alt: 'OMG',
    width: 120,
    height: 140
    caption: `an OMG example, check <a href="https://omg.com">to know more</a>`
)
```

The snippet, discovered by the plugin, could output something this.

```html
<figure class="picture" style="max-width: 120px;">
    <div class="picture__holder" style="padding-top: calc(140 / 120 * 100%);">
        <img class="picture__image" src="/omg.png" alt="OMG" />
    </div>
    <figcaption> an OMG example, check <a href="https://omg.com">to know more</a> </figcaption>
</figure>
```
