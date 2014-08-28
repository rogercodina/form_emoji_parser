Form emoji parser
=================

This module avoids PDOExceptions when saving data with emojis by erasing them. This module
parses submitted values for every existing form in drupal (to remove all emojis). You just
need to enable the module.

Emojis occupy 4 bytes in utf8, so in mysql we need to user utf8mb4 format or mysql will
return an error.

Thanks
======

I used regular expressions from this post:

http://magp.ie/2011/01/06/remove-non-utf8-characters-from-string-with-php/

Thank you so much!!!

More info
=========

https://www.drupal.org/node/1314214
https://www.drupal.org/node/1910376
http://www.arradi.com/pdoexception-sqlstatehy000-general-error-1366-incorrect-string-value
