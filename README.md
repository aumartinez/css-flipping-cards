# css-flipping-cards

CSS only animated flipping card

## An implementation issue

This is a revised example from the W3School sample at: https://www.w3schools.com/howto/howto_css_flip_card.asp, when used on a project noticed that this one doesn't work in IE, since 
```css
transform-style: preserve-3d;
```
is not supported, preventing to nest 3D transformed elements.

### The workaround

The solution is to "mimic" the transition by transpointing the elements using z-index positionning.
