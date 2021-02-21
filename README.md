# jekyll-bootstrap-slideshow
Jekyll slideshow based on Bootstrap v4.6 carousel and grabs information via post/page front matter

## Prerequisites
This is based on [Bootstrap v4.6](https://getbootstrap.com/docs/4.6/getting-started/introduction/). Bootstrap v5.0 beta is **not** supported.

## How to Use
Make sure that post-slideshow.html is in your Jekyll site's `_includes` folder. The slideshow is defined by the YAML front matter for each post:
```
slideshow-name:
  - image: /path/to/image/url
    caption: "Image caption"
```

The array can be as long as needed, just make sure each image is defined.

The slideshow will be displayed inline in the post/page, and is called thus:

```
{% include post-slideshow.html gallery-id="slideshow-name" %}
```

A post/page can have multiple slideshows. Make sure that `slideshow-name` is different in the post/page front matter and that in the markdown in the page, the `gallery-id` references the right `slideshow-name`.
