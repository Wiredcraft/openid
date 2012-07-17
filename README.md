# Handle the CNAME

The __CNAME__ file is used by github to allow the Github pages to respond to a specific CNAME. The content of the file is the domain name you want to use.

# Create HTML files for the users

For each of the users that will be using OpenID, create an html file that will contain the following template.

```
<html>
  <head>
    <link rel="openid2.provider" href="https://www.google.com/accounts/o8/ud?source=profiles">
    <link rel="openid2.local_id" href="https://profiles.google.com/[Google+ profile ID]">
  </head>
</html>
```

Replace __[Google+ profile ID]__ by the actual Google+ profile ID of the user.

A file named bob.html will then be available directly (depending on the chosen CNAME) as http://openid.wiredcraft.com/bob
