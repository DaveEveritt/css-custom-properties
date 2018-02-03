# CSS Custom Properties (variables)

A simple example with CSS code shown.

The `:root` selector is often used in examples showing CSS Custom Properties or "variables" to make them available throughout the document, for example:

```CSS
:root {
  --darkGreen: #051;
  --myPink: #fce;
}

section {
  color: var(--darkGreen);
  background: var(--myPink);
}

article h3 {
  color: var(--darkGreen);
}
```

**However, any element** can be used as the selector for CSS Custom Properties (not just the `:root` pseudo-element), but if you want access to them for child elements, you need to use their *parent element* as the selector, so `html` or `body` as the selectors for your CSS variables will also allow *any element on the page* to have access to them. For an example, [see the GitHub page for this repo](https://daveeveritt.github.io/css-custom-properties/).

Custom Properties are obviously not limited to colours.

**Bad:** no IE support, but Edge is taking over, so let's wait for IE to die completely or use a fallback.

## References:

- [Using CSS custom properties (variables)](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_variables) . 
- [CSS Variables: Why Should You Care?](https://developers.google.com/web/updates/2016/02/css-variables-why-should-you-care)
- As for why `--`, not `$` is used as the variable identifier, see [Let's Talk about CSS Variables](https://www.xanthir.com/blog/b4KT0)

---
Expanded from my [answer on StackOverflow](https://stackoverflow.com/a/48597520/123033) to [what-is-the-css-html-root-element](https://stackoverflow.com/questions/3916824/what-is-the-css-html-root-element/)
