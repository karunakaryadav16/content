---
title: color()
slug: Web/CSS/color_value/color
page-type: css-function
browser-compat: css.types.color.color
---

{{CSSRef}}

The **`color()`** functional notation allows a color to be specified in a particular, specified colorspace rather than the implicit sRGB colorspace that most of the other color functions operate in.

Support for a particular colorspace can be detected with the [`color-gamut`](/en-US/docs/Web/CSS/@media/color-gamut) CSS media feature.

The [`@color-profile`](/en-US/docs/Web/CSS/@color-profile) [CSS](/en-US/docs/Web/CSS) [at-rule](/en-US/docs/Web/CSS/At-rule) can be used to define and names a color profile to be used in the `color()` function to specify a color.

## Syntax

```css
color(display-p3 1 0.5 0);
color(display-p3 1 0.5 0 / .5);
```

### Values

- Functional notation: `color( [ [<ident> | <dashed-ident>]? [ <number-percentage>+ ] [ / <alpha-value> ]? ] )`

  - : `[<ident> | <dashed-ident>]` is an optional {{cssxref("ident")}} or {{cssxref("dashed-ident")}} denoting the colorspace. If this is an `<ident>` it denotes one of the predefined colorspaces (such as display-p3); if it is a `<dashed-ident>` it denotes a custom colorspace, defined by a [`@color-profile`](/en-US/docs/Web/CSS/@color-profile) rule.

    `[ <number-percentage>+ ]` is one or more {{cssxref("number")}} or {{cssxref("percentage")}} values providing the parameter values that the colorspace takes.

    `/ <alpha-value>` (alpha) can be a {{cssxref("&lt;number&gt;")}} between `0` and `1`, or a {{cssxref("&lt;percentage&gt;")}}, where the number `1` corresponds to `100%` (full opacity).

### Formal syntax

{{csssyntax}}

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- [Wide Gamut Color in CSS with Display-p3](https://webkit.org/blog/10042/wide-gamut-color-in-css-with-display-p3/)
