# passprotect-js

**Stop using bad passwords.**


## What is PassProtect?

PassProtect is a developer library you can drop into any web page which
dramatically improves the security of users accessing your website.

PassProtect works by binding itself to all `input` elements on the page of type 
`email` or `password` inputs. Whenever a user enters a new value into
one of these `input` elements, PassProtect will check the user's email /
password against the fabulous https://haveibeenpwned.com/ API service to see
whether or not the user's email OR password has been breached in the past.

Finally, if appropriate, PassProtect will inform the user that their credentials
were previously breached, give them some useful information, and ask them to
update their password as soon as they can to reduce the risk that their account
will be compromised.

PassProtect is a new, experimental way to proactively notify users about data
breaches and help casual web users take a more practice stance in their own data
security by informing them and encouraging them to take action to secure their
accounts.


## How to Use PassProtect

To use PassProtect in your website, simply copy the following script tag
anywhere on your page. Don't worry about where you put it: anywhere is fine. It
will run once the page has loaded and will initialize itself without any
configuration necessary.

```html
<html>
  <head>
    <!-- ... -->
  </head>
  <body>
    <!-- ... -->
    <script src="TODO"></script>
  </body>
</html>
```

You'll ideally want to include the PassProtect script tag on every page that
contains an `input` element. There is almost no performance penalty for
including PassProtect on all pages of your site -- if a page doesn't contain any
`input` elements, PassProtect won't do anything and will immediately exit.

To keep things simple, our recommended approach is to just include the
PassProtect script on every page of your site.


## Is PassProtect Secure?

**YES!**

PassProtect never sends or stores password information over the network. It uses
[k-Anonymity](https://www.troyhunt.com/ive-just-launched-pwned-passwords-version-2/)
to safely communicate your sensitive data over the internet without risk.

PassProtect is also completely free, open source, and maintained by [Randall
Degges](https://twitter.com/rdegges). If you want to audit the source, or have
ideas about how to do things better, please open a
[GitHub issue](https://github.com/okta/passprotect-js) or [email me](mailto:randall.degges@okta.com) directly.


## Changelog

**May 21, 2018**

- First release! Yey.
