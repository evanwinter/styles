# @evanwinter/styles

A minimal CSS utility library Evan uses in his personal projects.

### Borders

---

| key  | value   |
| ---- | ------- |
| xxs  | 0.125em |
| xs   | 0.25em  |
| sm   | 0.5em   |
| md   | 1em     |
| lg   | 2em     |
| full | 50%     |

```css
.border {
  border: 1px solid currentColor;
}

.border-thick {
  border-width: 2px solid currentColor;
}

.rounded-{key} {
  border-radius: {value};
}
```

### Breakpoints / Widths

---

| key | value |
| --- | ----- |
| xs  | 20rem |
| sm  | 30rem |
| md  | 48rem |
| lg  | 64rem |
| xl  | 80rem |

```css
--breakpoint-{key}: {value};

.w-{key} {
  width: {value};
}

.maxw-{key} {
  width: min(100%, {value});
}

.minw-{key} {
  width: max(100%, {value});
}

.w-none {
  width: 0;
}

.w-100 {
  width: 100%;
}
```

### Colors

---

| key      | value                     |
| -------- | ------------------------- |
| black    | rgb(33, 33, 33)           |
| black-75 | rgba(33, 33, 33, 0.75)    |
| black-50 | rgba(33, 33, 33, 0.5)     |
| black-25 | rgba(33, 33, 33, 0.25)    |
| black-10 | rgba(33, 33, 33, 0.1)     |
| white    | rgb(247, 247, 247)        |
| white-75 | rgba(247, 247, 247, 0.75) |
| white-50 | rgba(247, 247, 247, 0.5)  |
| white-25 | rgba(247, 247, 247, 0.25) |
| white-10 | rgba(247, 247, 247, 0.1)  |

```css
--color-{key}: {value};

.color-{key} {
  color: {value};
}

.bg-{key} {
  background-color: {value};
}
```

### Flexbox

---

```css
.flex {
  display: flex;
}

/* Direction */

.flex.row {
  flex-direction: row;
}

.flex.column {
  flex-direction: column;
}

.flex.row-reverse {
  flex-direction: row-reverse;
}

.flex.column-reverse {
  flex-direction: column-reverse;
}

/* Justify */

.flex.justify-start {
  justify-content: flex-start;
}

.flex.justify-center {
  justify-content: center;
}

.flex.justify-end {
  justify-content: flex-end;
}

.flex.justify-between {
  justify-content: space-between;
}

.flex.justify-around {
  justify-content: space-around;
}

/* Align */

.flex.align-start {
  align-items: flex-start;
}

.flex.align-center {
  align-items: center;
}

.flex.align-end {
  align-items: flex-end;
}

.flex.align-stretch {
  align-items: stretch;
}

.flex.align-baseline {
  align-items: baseline;
}

/* Gap */

.flex.gap-{spacingKey} {
  gap: {spacingValue};
}
```

### Heights

---

| key   | value |
| ----- | ----- |
| 10vh  | 10vh  |
| 20vh  | 20vh  |
| 30vh  | 30vh  |
| 40vh  | 40vh  |
| 50vh  | 50vh  |
| 60vh  | 60vh  |
| 70vh  | 70vh  |
| 80vh  | 80vh  |
| 90vh  | 90vh  |
| 100vh | 100vh |

```css
.minh-{key} {
  height: auto;
  min-height: {value};
}

.maxh-{key} {
  height: auto;
  max-height: {value};
}

.h-{key} {
  height: {value};
}

.h-none {
  height: 0;
}

.h-100 {
  height: 100%;
}
```

### Misc

---

```css
.sr-only {
  position: absolute;
  width: 1px;
  height: 1px;
  padding: 0;
  margin: -1px;
  overflow: hidden;
  clip: rect(0, 0, 0, 0);
  white-space: nowrap;
  border: 0;
}
```

### Position

---

| key      | value    |
| -------- | -------- |
| absolute | absolute |
| fixed    | fixed    |
| relative | relative |
| sticky   | sticky   |
| static   | static   |

```css
.{key} {
  position: {value};
}

.top-{spacingKey} {
  top: {spacingValue};
}
.bottom-{spacingKey} {
  bottom: {spacingValue};
}
.left-{spacingKey} {
  left: {spacingValue};
}
.right-{spacingKey} {
  right: {spacingValue};
}

.inset-0 {
  inset: 0;
}
```

### Spacing

---

| key  | value  |
| ---- | ------ |
| auto | auto   |
| none | 0      |
| xxs  | 0.25em |
| xs   | 0.5em  |
| sm   | 1em    |
| md   | 2em    |
| lg   | 4em    |
| xl   | 8em    |
| xxl  | 12em   |

```css
--space-{key}: {value};

/* Margin */

.m-{key} {
  margin: {value};
}

.mt-{key} {
  margin-top: {value};
}

.mr-{key} {
  margin-right: {value};
}

.mb-{key} {
  margin-bottom: {value};
}

.ml-{key} {
  margin-left: {value};
}

.mx-{key} {
  margin-left: {value};
  margin-right: {value};
}

.my-{key} {
  margin-top: {value};
  margin-bottom: {value};
}

/* Padding */

.p-{key} {
  padding: {value};
}

.pt-{key} {
  padding-top: {value};
}

.pr-{key} {
  padding-right: {value};
}

.pb-{key} {
  padding-bottom: {value};
}

.pl-{key} {
  padding-left: {value};
}

.px-{key} {
  padding-left: {value};
  padding-right: {value};
}

.py-{key} {
  padding-top: {value};
  padding-bottom: {value};
}

```

### Typography

---

#### Alignments

| key    | value  |
| ------ | ------ |
| center | center |
| left   | left   |
| right  | right  |

```css
.text-{key} {
  text-align: {value};
}
```

#### Weights

| key      | value |
| -------- | ----- |
| light    | 300   |
| normal   | 400   |
| semibold | 600   |
| bold     | 700   |

```css
--text-{key}: {value};

.text-{key} {
  font-weight: {value};
}
```

#### Sizes

| key   | value |
| ----- | ----- |
| small | 0.9em |
| large | 1.2em |

```css
--text-{key}: {value};

.text-{key} {
  font-size: {value};
}
```

#### Decoration

```css
.underline {
  text-decoration: underline;
}
```

### CSS Reset

---

```css
// Modern CSS Reset
// https://github.com/andy-piccalilli/modern-css-reset
// (amended by me)

* {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

/* Box sizing rules */
*,
*::before,
*::after {
  box-sizing: border-box;
}

/* Remove list styles on ul, ol elements with a list role, which suggests default styling will be removed */
ul[role="list"],
ol[role="list"] {
  list-style: none;
}

/* Set core root defaults */
html:focus-within {
  scroll-behavior: smooth;
}

/* Set core body defaults */
body {
  min-height: 100vh;
  text-rendering: optimizeSpeed;
  line-height: 1.5;
  margin: 0;
}

/* A elements that don't have a class get default styles */
a:not([class]) {
  text-decoration-skip-ink: auto;
}

/* Make images easier to work with */
img,
picture {
  max-width: 100%;
  display: block;
}

/* Inherit fonts for inputs and buttons */
input,
button,
textarea,
select {
  font: inherit;
}

/* Remove all animations and transitions for people that prefer not to see them */
@media (prefers-reduced-motion: reduce) {
  html:focus-within {
    scroll-behavior: auto;
  }
  *,
  *::before,
  *::after {
    animation-duration: 0.01ms !important;
    animation-iteration-count: 1 !important;
    transition-duration: 0.01ms !important;
    scroll-behavior: auto !important;
  }
}

ul {
  list-style: none;
  padding: 0;
  margin: 0;
}
```
