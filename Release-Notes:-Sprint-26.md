_This is a draft!_
--------------------
_This document will not be finalized until the end of Sprint 26 -- approximately June 10._

What's New in Sprint 26
-----------------------
* **Extensions**
    * [Easier extension updating](https://trello.com/card/2-extension-listing-update/4f90a6d98f77505d7940ce88/877): When installing a newer version of an extension you already have installed, Brackets will automatically replace the older version.
* **File Management**
    * [Save As](https://trello.com/card/3-create-file-w-save-as/4f90a6d98f77505d7940ce88/286): Just what it sounds like!
    * [Polish on delete file/folder](https://trello.com/card/2-delete-file-folder/4f90a6d98f77505d7940ce88/382): Better handling of unsaved changes... now with unit tests!
* **Overall UI**
    * [Status bar redesign](https://trello.com/card/1-ux-implement-status-bar/4f90a6d98f77505d7940ce88/808): Added separators, changed JSLint results icon to more standard colors (green = passing, yellow = warnings).
* **Architecture**
    * [Upgrade Brackets source to jQuery 2.0, Bootstrap 2.3.1, LESS 1.3.3](https://trello.com/card/3-upgrade-jquery-less-bootstrap/4f90a6d98f77505d7940ce88/813): From jQuery 1.7, Bootstrap 1.4.0, LESS 1.3.0


_Full change logs:_ [brackets](https://github.com/adobe/brackets/compare/sprint-25...sprint-26#commits_bucket) and [brackets-shell](https://github.com/adobe/brackets-shell/compare/sprint-25...sprint-26#commits_bucket)


UI Changes
----------
**Status bar / JSLint icon** - _TODO_


API Changes
-----------
**jQuery API changes** - _TODO - link to jQuery info on removed/changed APIs_

**Bootstrap API / CSS changes** - _TODO - is there a Bootstrap migration doc we can link to?_

New/Improved Extensibility APIs
-------------------------------


Known Issues
------------
* Mountain Lion (OS X 10.8) by default will not allow Brackets to run since it's not digitally signed yet. To work around this, right click the Brackets app and choose Open. You only need to do that once -- afterward, launching Brackets the normal way will work also.
* [#2272](https://github.com/adobe/brackets/issues/2272): Windows Vista may not allow the Brackets installer to run (you may not see _any_ error message). To work around this, right-click the installer file, choose Properties, and click the Unblock button.
* [#3458](https://github.com/adobe/brackets/issues/3458): Quick View does not yet support the latest CSS gradient syntax (using `to` keyword, unprefixed `radial-gradient`, `repeating-linear-gradient` or `repeating-radial-gradient`).
* [#3570](https://github.com/adobe/brackets/issues/3570): Mac only - Quick View popover may not appear after resizing window or going fullscreen. Move the mouse to the top of the screen to fix.
(https://github.com/adobe/brackets/wiki/How-to-Hack-on-Brackets#wiki-getcode) instead.
* [#3207](https://github.com/adobe/brackets/issues/3207): If you use a Sprint 21 or earlier build after using this build at least once, a few preferences such as Recent Projects may get reset. (You can back up your [[cache folder]] if you're concerned about this).
* _Debug > Run Tests_ is disabled in the installer/DMG distributions of Brackets, because the unit test code is not included. To run unit tests, [pull Brackets from GitHub](https://github.com/adobe/brackets/wiki/How-to-Hack-on-Brackets#wiki-getcode) instead.


Community contributions to Brackets
-----------------------------------

Contributions _from_ the Brackets community
-------------------------------------------
**Contributions to [CodeMirror](https://github.com/marijnh/CodeMirror):**
* ...

Bugs fixed in Sprint 26
-----------------------
For details on the bugs addressed, please refer to [closed sprint 26 bugs](https://github.com/adobe/brackets/issues?labels=&milestone=13&state=closed). A few of the fixed bugs might not be caught by this search query, however.