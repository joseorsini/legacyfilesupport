add support for Legacy Files in 3.5.x

As of 3.x, calls to REST API for Legacy Files using Identifiers on the URI don't work. By editing the files on this plugin and overriding the default ones via OSGi plugin enables support for these legacy files

Related to support ticket: https://my.dotcms.com/tickets/detail.dot?id=ec3c46c6-1099-4695-b1fb-455831bb5aac

Fixes:
https://github.com/joseorsini/legacyfilesupport/blob/master/src/main/java/com/dotmarketing/viewtools/FileTool.java#L70

https://github.com/joseorsini/legacyfilesupport/blob/master/src/main/java/com/dotmarketing/viewtools/content/FileMap.java#L46

Still pending:

support for backend js/jsp files (still using identifiers, show as 404)
