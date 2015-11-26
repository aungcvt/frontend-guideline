# Naming

## Class
Class name must be in all small letters. Don't use capitalize for class names.

> e.g. class="abc defghi"

> Don't: class="Abc Defghi"

Class name cannot start with numbers and special characters.

> Don't: class="1abc $abc"

Long class names can be divided by "-" dash ( minus ). Don't use underscore ( _ ) for class name dividers.

> e.g. class="abc-def col-sm-3"

> Don't: class="abc_def col_sm_3"


## Id
Long id should use underscore ( _ ) to divide. Don't use dash ( - ) for id.

( This is the way to differentiate between class and id. )

> e.g. id="abc_def"

> Don't: id="abc-def"


Don't use camelCase for id. Leave camelCase for Javascript variables or other programming language variables.

> Don't: id="someThing doNotUseThis"

Other things like capitalize or small letters, numbers and special characters follow class name guide above.


# Include

## Inline
Don't use inline styles.

> Don't: &lt;div style="margin-top: 0px;"&gt;

Inline styles can be used when changing something ( working on dynamic styles ) from Javascript.

Even don't use that way. For best practice, try changing class name from Javascript.
