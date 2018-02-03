# CSS Custom Properties (variables)

A simple example with CSS code shown.

`:root` is often used to declare CSS Custom Properties or "variables" that become available throughout the document, for example:

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

Any element can be used (not just the `:root` pseudo-element), so if you want to access your CSS variables in child elements, you need to use their parent element as the selector e.g. using `html` or `body` will also allow any element on the page to have access to your CSS variables.

Custom Properties are obviously not limited to colours.

Bad: no IE support, but Edge is taking over, so let's wait for IE to die completely or use a fallback.

## References:

- [Using CSS custom properties (variables)](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_variables) . 
- [CSS Variables: Why Should You Care?](https://developers.google.com/web/updates/2016/02/css-variables-why-should-you-care)
- As for why `--`, not `$` is used as the variable identifier, see [Let's Talk about CSS Variables](https://www.xanthir.com/blog/b4KT0)

---
Expanded from my [answer on StackOverflow](https://stackoverflow.com/a/48597520/123033) to [what-is-the-css-html-root-element](https://stackoverflow.com/questions/3916824/what-is-the-css-html-root-element/)
