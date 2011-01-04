// $Id: README.txt,v 1.1.2.1 2009/01/31 12:51:59 cptncauliflower Exp $

DESCRIPTION
-----------

Define which cck fields should be able to keep private.


INSTALL
-------

Follow these steps:
1. Untar the tarball into your module directory (sites/all/modules)
2. Enable the module.  CCK must also be enabled.
3. Create your content types and additional fields with the cck module
5. Go to admin/content/privacy and enable the fields which should be able to
keep private (only users with 'administer privacy' rights are able to do this)
6. When a user creates a node, he can check if a field should be private or
not.

Definition of 'private':
- Only the author of the node or the users with 'administer privacy' or 'view
  all privacy' rights are able to see hidden fields.

How does this differ from CCK's content permissions module?
  When you use the 'content_permissions' module, you can define if a role is able to see or edit the field.
  With this privacy module, you can define if an author of a node is able to set a field to private. So other users, even if they have the same role of the author, won't be able to see this field when the author has marked it as private.
  You can, roughly, see it as: content_permissions is role based, privacy is user based.

CREDITS
-------

This module is developed by the webteam of jeugdwerknet.be (Pieter, Wouter and
Wim) and is based on http://drupal.org/project/cck_field_privacy and
http://drupal.org/project/profile_privacy (the difference is that this module
is not dependent on the profile, friendlist and jquery_impromptu module)
