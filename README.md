# SGS
> Responsive, Fluid, Semantic and Non-Semantic grid system written in stylus

## Features

- Responsive automatic and manual integration
- Box Sizing with border-box integrated
- Semantic and Non-semantic mode
- Gutter, Container and more items are configurable
- Non-semantic classes are configurable
- Don't have support for IE7

## Starting
Import the `sgs.styl` file:

```css
@import "path/to/sgs"
```
## Semantic Usage
### #1 method
In #1 method, the responsive design has to be made manually.

```css
.my-div
  column(8)
  @media tablet
   column(7)

.my-other-div
  column(4)
  @media tablet
   column(5)
```

### #2 method
In #2 method, the responsive is automatically. Is used `@extend` stylus method.

```css
.my-div
  @extend .sgs8

.my-other-div
  @extend .sgs4
```

## Non-Semantic Usage
Is used classes from `1` to `12` (max colums configurable) for markup in your html. The `sgs` prefix name also is configurable.

```html
<div class="container">
    <div class="sgs3">.sgs3</div>
    <div class="sgs3">.sgs3</div>
    <div class="sgs3">.sgs3</div>
    <div class="sgs3">.sgs3</div>
</div>
```

## Credits
- Made with ❤︎ by [Diogo Moretti](http://github.com/diogomoretti)
- The **SGS** was inspired in [semantic.gs](http://semantic.gs)