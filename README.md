# jQuery Star Rating

The Star Rating Plugin is a plugin for the jQuery Javascript library that creates a non-obstrusive star rating control based on a set of radio input boxes.

---
 
## Installation
`npm install @virtualidentity/jquery-star-rating --save`

---
 
## Basic Usage

### Simple stars
Just add the `class="star"` to your radio boxes:
```html
<input name="star1" type="radio" class="star"/>
<input name="star1" type="radio" class="star"/>
<input name="star1" type="radio" class="star"/>
<input name="star1" type="radio" class="star"/>
<input name="star1" type="radio" class="star"/>
```
#### Specifying a default value
Use the `checked` property to specify the initial/default value of the control
```html
<input name="star2" type="radio" class="star"/>
<input name="star2" type="radio" class="star"/>
<input name="star2" type="radio" class="star" checked="checked"/>
<input name="star2" type="radio" class="star"/>
<input name="star2" type="radio" class="star"/>
```
#### Read-only stars
Use the `disabled` property to use a control for display purposes only
```html
<input name="star3" type="radio" class="star" disabled="disabled"/>
<input name="star3" type="radio" class="star" disabled="disabled"/>
<input name="star3" type="radio" class="star" disabled="disabled" checked="checked"/>
<input name="star3" type="radio" class="star" disabled="disabled"/>
<input name="star3" type="radio" class="star" disabled="disabled"/>
```
#### Split-stars with the metadata plugin
Use the <a href="https://github.com/jquery-archive/jquery-metadata">`metadata` plugin</a> to pass advanced settings to the plugin via the class property.
The example below creates 4 total stars with a selected value of 1.25 (1 and a quarter star).
The total number of stars is the number of radios divided by the split, in this case 16/4 = 4.
The number of stars selected is the ordinal value of the radio selected divided by the split, in this case 5/4 = 1.25
```html
<input name="adv1" type="radio" class="star {split:4}"/>
<input name="adv1" type="radio" class="star {split:4}"/>
<input name="adv1" type="radio" class="star {split:4}"/>
<input name="adv1" type="radio" class="star {split:4}"/>
<input name="adv1" type="radio" class="star {split:4}" checked="checked"/>
<input name="adv1" type="radio" class="star {split:4}"/>
<input name="adv1" type="radio" class="star {split:4}"/>
<input name="adv1" type="radio" class="star {split:4}"/>
<input name="adv1" type="radio" class="star {split:4}"/>
<input name="adv1" type="radio" class="star {split:4}"/>
<input name="adv1" type="radio" class="star {split:4}"/>
<input name="adv1" type="radio" class="star {split:4}"/>
<input name="adv1" type="radio" class="star {split:4}"/>
<input name="adv1" type="radio" class="star {split:4}"/>
<input name="adv1" type="radio" class="star {split:4}"/>
<input name="adv1" type="radio" class="star {split:4}"/>
```
