# Custom Checkbox Radio

CSS based custom checkboxes and radios; a CSS module solution.

![Swanky](posterity/custom-checkbox-radio.gif)

## Install

    npm i custom-checkbox-radio

## Include

Depending on your current directory and frontend stack, you'll want something along the lines of one of:

```scss
@import "custom-checkbox-radio";
```

## Add

Note, your labels must proceed the inputs and all have suitable name/id/for attributes.

````scss
@use 'custom-checkbox-radio-scss/variables' with (
  $background: #f00 // Override any variables
);
@use 'custom-checkbox-radio-scss' as ccr;
.checkbox {
  @include ccr.checkbox;
}
.radio {
  @include ccr.radio;
}
```

```jsx

import customCheckboxRadio from "custom-checkbox-radio/ccr.module.css";

() => (
    <>
      <legend>Checkboxes</legend>
      <p className="{customCheckboxRadio.ccr}">
          <input type="checkbox" name="lorem-1" id="lorem-1" />
          <label htmlFor="lorem-1">Lorem</label>
      </p>

      <legend>Radios</legend>
      <p className="{customCheckboxRadio.ccr}">
          <input type="radio" name="ipsum" id="ipsum-1" />
          <label htmlFor="ipsum-1">Lorem</label>
      </p>
    </>
);
````

## Customise

Written in a non-invasive kinda way, so you can add your own styles to, say, `input[type="radio"] + label::after`, or simply override the various variables set in [the SCSS file](https://github.com/entozoon/custom-checkbox-radio/blob/master/_ccr.module.css).

## Browser Support

IE9 +
