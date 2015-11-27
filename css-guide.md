# CSS Style Guide

## Naming

### Class
Class name must be in all small letters. Don't use capitalize for class names.

**Do:**
````html
class="abc defghi"
````

**Don't:**
````html
class="Abc Defghi"
````

Class name cannot start with numbers and special characters.

**Don't:**
````html
class="1abc $abc"
````

Long class names can be divided by "-" dash ( minus ). Don't use underscore ( _ ) for class name dividers.

**Do:**
````html
class="abc-def col-sm-3"
````

**Don't:**
````html
class="abc_def col_sm_3"
````


### Id
Long id should use underscore ( _ ) to divide. Don't use dash ( - ) for id.

( This is the way to differentiate between class and id. )

**Do:**
````html
id="abc_def"
````

**Don't:**
````html
id="abc-def"
````


Don't use camelCase for id. Leave camelCase for Javascript variables or other programming language variables.

**Don't:**
````html
id="someThing doNotUseThis"
````

Other things like capitalize or small letters, numbers and special characters follow class name guide above.


## Include

### Inline
Don't use inline styles.

**Don't:**
````html
<div style="margin-top: 0px;">
````

Inline styles can be used when changing something ( mostly numbers ) from Javascript.

````javascript
$('div').css('height', '100px');
````

*Tip*

For other dynamic styles ( e.g. color changing ), use class names to change the style from Javascript.

````javascript
$('div').addClass('text-green');
````

### External
Always include external stylesheets in `<head>` section.

### Internal
Don't use internal css if not really necessary.


## Writing

### Lines
Use open curly bracket with the same line with selector and close curly bracket in the next line.
Use one space between selector and open bracket.
There should be one line break between each style.

**Do**
````css
.selector {
  background: white;
}

.another-selector {
  color: white;
}
````

**Don't**
````css
.selector
{
  font-weight: bold;
}

.selector{font-weight: bold;}
````

Use another line for multi selectors.

**Do**
````css
.selector-1,
.selector-2 {
  color: red;
}
````

**Don't**
````css
.selector-1, .selector-2 {
  color: red;
}
````

### Spaces ( Indent )
Use soft tab _( 2 spaces )_ for tab. Each declaration must have one tab from left.

**Do**
````css
h1 {
  font-size: 30px;
  font-weight: bold;
}
````

**Don't**
````css
h1 {
font-size: 30px;
}
````

Always use one space between colon separator and value.
But don't use space between property and colon separator.

**Do**
````css
a {
  text-decoration: underline;
}
````

**Don't**
````css
a {
  color :blue;
  text-decoration:underline;
}
````

Use one indent ( one tab ) for nested statements.

````css
@media screen {
  a {
    text-decoration: none;
  }
}
````

## Rules
Don't use `!important` if not really necessary and site-wide.
Use child selectors for specific target.

**Do**
````css
div {
  color: red;
}

div p {
  color: green;
}
````

**Don't**
````css
div {
  color: red;
}

p {
  color: green !important;
}
````
