# HTML Style Guide

## General

### Doctype
Always use `<!DOCTYPE html>` except EDMs.

### Writing
Always use lower case ( small letters ) for all html tags.

**Do**
````html
<html>
  <body>
````

**Don't**
````html
<HTML>
  <Body>
````

### External Resources
Don't use `http:` and `https:` for external URLs (resources).

**Don't**
````html
<link href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/css/bootstrap.min.css">  
<script src="http://www.google.com/js/gweb/analytics/autotrack.js"></script>  
<img src="http://www.google.com.sg/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png">
````

**Do**
````html
<link href="//maxcdn.bootstrapcdn.com/bootstrap/3.3.6/css/bootstrap.min.css">  
<script src="//www.google.com/js/gweb/analytics/autotrack.js"></script>  
<img src="//www.google.com.sg/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png">
````

**Don't**
````css
.icon {
  background: url(http://www.example.com/images/icon.png);
}
````

**Do**
````css
.icon {
  background: url(//www.example.com/images/icon.png);
}
````
