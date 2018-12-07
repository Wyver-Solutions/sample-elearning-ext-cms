# sample-elearning-ext-cms
Showing how an elearning package can pull content from an external resource

Accessing via /elearning/index.html will take you to an "elearning" package. It just contains one question, and a button to get help.

Help is provided by content stored in /cms/midi.html, which can also be accessed independently.

Ideally the CMS would either be on the same domain as the elearning (to prevent Cross Origin Request issues).

Or the CMS could be set up on a server which allows Cross Origin Requests. That's OK for internal-only servers, but may be problematic for internet-facing servers.

<a href="elearning/index.html">Open Elearning package</a>

<a href="cms/midi.html">Open sample page on content management system</a>

It is restricted to content that is hosted on the same domain, which would be an issue is you're using a SaaS Learning Management System, like Docebo or Cornerstone (although perhaps they could consider providing a content management system alongside their LMS offerings?)

If you have a content management system, and can make changes at a server-level, it might be able to get around the cross-origin security restrictions.

The alternative is to display the content in an iframe, but then you'd end up with all the gubbins (menus etc) around the content, unless your theme pack includes a way to remove those gubbins.

For example:

With gubbins: https://demo.hibbittsdesign.org/grav-open-matter-course-hub/ux-techniques-guide

Without gubbins: https://demo.hibbittsdesign.org/grav-open-matter-course-hub/ux-techniques-guide/chromeless:true
