# Cheat Sheet

[:arrow_backward: Algebra / Web Designer / Module 2 - HTML](./)

---

## Document structure

**Basic HTML5 document structure**

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <meta http-equiv="X-UA-Compatible" content="ie=edge">
        <title>My HTML5 document</title>
    </head>
    <body>
    </body>
</html>
```

**Common structural semantic elements**

```
article, aside, footer, header, main, nav, section
```

**Non-semantic structural elements**

```
div, span
```

## Tables

**Table with column headings**

```html
<table>
    <caption>Table with column headings</caption>
    <tr>
        <th scope="col">First name</th>
        <th scope="col">Last name</th>
        <th scope="col">Secret identity</th>
    </tr>
    <tr>
        <td>Peter</td>
        <td>Parker</td>
        <td>Spider-Man</td>
    </tr>
    <tr>
        <td>Bruce</td>
        <td>Wayne</td>
        <td>Batman</td>
    </tr>
</table>
```

**Table with row headings**

```html
<table>
    <caption>Table with row headings</caption>
    <tr>
        <th scope="row">Year</th>
        <td>2018</td>
        <td>2019</td>
        <td>2020</td>
    </tr>
    <tr>
        <th scope="row">GDP</th>
        <td>14,178.0</td>
        <td>14,151.2</td>
        <td>14.242.1</td>
    </tr>
</table>
```