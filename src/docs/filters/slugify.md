---
eleventyNavigation:
  parent: Filters
  key: slugify Filter
  title: '<code>slugify</code>'
  order: 2
  excerpt: '<code>"My string"</code> to <code>"my-string"</code> for permalinks.'
---

# `slugify` Universal Filter {% addedin "1.0.0" %}

{% callout "info", "md" %}In versions prior to 1.0.0, [the `slug` Universal Filter was used](/docs/filters/slug/). To maintain backwards compatibility moving forward, `slug` is still included and supported but `slugify` is now recommended as best practice—it has better default behavior for URLs with special characters.{% endcallout %}

Uses the [`@sindresorhus/slugify` npm package](https://www.npmjs.com/package/@sindresorhus/slugify) to convert a string into a URL slug. Typically used inside of permalinks.

{% raw %}
```
{{ "My Title" | slugify }} -> `my-title`
```
{% endraw %}

* [`slug` Universal Filter](/docs/filters/slug/)
* [← Back to Filters documentation.](/docs/filters/)