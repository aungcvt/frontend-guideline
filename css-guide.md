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
&lt;div style="margin-top: 0px;"&gt;
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
