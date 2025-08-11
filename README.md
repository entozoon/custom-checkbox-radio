# Custom Checkbox Radio

CSS based custom checkboxes and radios; a CSS module solution.

![Swanky](posterity/custom-checkbox-radio.gif)

## Install

    npm i custom-checkbox-radio

## Usage

Note, your labels must proceed the inputs and all have suitable name/id/for attributes.

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
```

## Customise

Written in a non-invasive kinda way, so you can add your own styles or simply override the various CSS variables set in [the CSS file](https://github.com/entozoon/custom-checkbox-radio/blob/main/ccr.module.css#L1).

## Browser Support

IE9 +
