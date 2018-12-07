# sample-elearning-ext-cms
Showing how an elearning package can pull content from an external resource

Accessing via /elearning/index.html will take you to an "elearning" package. It just contains one question, and a button to get help.

Help is provided by content stored in /cms/midi.html, which can also be accessed independently.

Ideally the CMS would either be on the same domain as the elearning (to prevent Cross Origin Request issues).

Or the CMS could be set up on a server which allows Cross Origin Requests. That's OK for internal-only servers, but may be problematic for internet-facing servers.
