_This is a draft!_
--------------------
_This document will not be finalized until the end of Release 0.44 -- approximately October 5._

What's New in Release 0.44
--------------------------
* **Split View**
    * **[Vertical & Horizontal Split View](https://trello.com/c/WLeAC84F/1290-splitview-landing-in-master)**: View two files side by side or one above the other. (Note: it is not yet possible to view the same file in both panes).
* **Stylesheet Editing**
    * Fix bug [#9002](https://github.com/adobe/brackets/issues/9002) - Brackets freezes during Live Preview on a line within a CSS/SCSS/LESS block comment that contains nothing but "}" with no indent.
    * Fix bug [#8966](https://github.com/adobe/brackets/issues/8966) - Inline editor is blank if your CSS rule contains a vendor-prefixed property that uses a rgb()-like color value.
* **Files and Folders**
    * [Project tree improvements](https://trello.com/c/R5VQiTnS/1353-project-manager-revamp): Many small bug fixes in the sidebar file tree. Notably, it's now possible to right-click files that Brackets cannot open (such as binary files and non-UTF8 text files).
* **Preferences**
    * [New preference: show cursor in selected text](https://github.com/adobe/brackets/pull/8972): By default, Brackets hides the blinking cursor when you have a text selection; this behavior can now be disabled.
* **Localization**
    * [Extension name/description localization](https://github.com/adobe/brackets/pull/8987): The info displayed in Extension Manager, such as extension name & description, can now be localized via the [`package-i18n` property](https://github.com/adobe/brackets/wiki/Extension-package-format#packagejson-format).


_Full change logs:_ [brackets](https://github.com/adobe/brackets/compare/release-0.43...release-0.44#commits_bucket) and [brackets-shell](https://github.com/adobe/brackets-shell/compare/release-0.43...release-0.44#commits_bucket)


UI Changes
----------
TODO


API Changes
-----------
TODO

New/Improved Extensibility APIs
-------------------------------
TODO - [Working Set View Extensibility](https://github.com/adobe/brackets/pull/9054)


Known Issues
------------
* Activity Monitor in Mavericks (OS X 10.9) says the Brackets Helper process is "Not Responding" even when it's working normally ([#5794](https://github.com/adobe/brackets/issues/5794)). You can safely ignore this unless Brackets is actually failing to respond when you click or type text.
* [#2272](https://github.com/adobe/brackets/issues/2272): Windows Vista may not allow the Brackets installer to run (you may not see _any_ error message). To work around this, right-click the installer file, choose Properties, and click the Unblock button.
* _Debug > Run Tests_ is disabled in the installer/DMG distributions of Brackets, because the unit test code is not included. To run unit tests, [pull Brackets from GitHub](https://github.com/adobe/brackets/wiki/How-to-Hack-on-Brackets#wiki-getcode) instead.


Community contributions to Brackets
-----------------------------------
* [Quick Docs: Support vendor-prefixed CSS properties](https://github.com/adobe/brackets/pull/8739) by [Marcel Gerber](https://github.com/MarcelGerber)
* [Sort Working Files locale-aware](https://github.com/adobe/brackets/pull/8971) by [Marcel Gerber](https://github.com/MarcelGerber)
* [Quick View: Only respond to color _names_ in CSS/SCSS/LESS files](https://github.com/adobe/brackets/pull/8156) by [Marcel Gerber](https://github.com/MarcelGerber)
* [New preference: "showCursorWhenSelecting"](https://github.com/adobe/brackets/pull/8972) by [Marcel Gerber](https://github.com/MarcelGerber)
* [More consistently use "Release" (not "Sprint") to describe version number](https://github.com/adobe/brackets-shell/pull/462) ([part 2](https://github.com/adobe/brackets/pull/8680), [part 3](https://github.com/adobe/brackets-shell/pull/466)) by [Marcel Gerber](https://github.com/MarcelGerber)
* [Switch Extension Manager tabs using Ctrl-(Shift)-Tab](https://github.com/adobe/brackets/pull/8856) (+ [part 2](https://github.com/adobe/brackets/pull/9226)) by [Marcel Gerber](https://github.com/MarcelGerber)
* [Easing editor: Tolerate errant trailing comma in `cubic-bezier()`](https://github.com/adobe/brackets/pull/8910) by [Marcel Gerber](https://github.com/MarcelGerber)
* [Add _Debug > Open Brackets Source_ command](https://github.com/adobe/brackets/pull/8859) by [Marcel Gerber](https://github.com/MarcelGerber)
* [Themes: Allow styling cursor without needing `!important`](https://github.com/adobe/brackets/pull/9061) by [Miguel Castillo](https://github.com/MiguelCastillo)
* [Fix Quick View positioning with Split View](https://github.com/adobe/brackets/pull/8976) by [Marcel Gerber](https://github.com/MarcelGerber)
* [Fix Preferences bug in experimental ES6 Promises branch](https://github.com/adobe/brackets/pull/9047) (not part of Brackets yet) by [Arzhan "kai" Kinzhalin (Intel Corp)](https://github.com/busykai)
* [Cleanup: Remove many unused vars](https://github.com/adobe/brackets/pull/8954) by [Marcel Gerber](https://github.com/MarcelGerber)
* [Cleanup: Fix capitalization in function name](https://github.com/adobe/brackets/pull/9081) by [Arzhan "kai" Kinzhalin (Intel Corp)](https://github.com/busykai)
* [Cleanup: Update comment links to CodeMirror repo](https://github.com/adobe/brackets/pull/9407) by [Marcel Gerber](https://github.com/MarcelGerber)
* [Czech translation update](https://github.com/adobe/brackets/pull/8926) (+ [part 2](https://github.com/adobe/brackets/pull/9100)) by [kvarel](https://github.com/kvarel)
* [Finnish translation update](https://github.com/adobe/brackets/pull/8939) (+ [part 2](https://github.com/adobe/brackets/pull/9156), [part 3](https://github.com/adobe/brackets/pull/9391)) by [valtlait](https://github.com/valtlait)
* [Galician translation update](https://github.com/adobe/brackets/pull/9297) by [Iván Barcia](https://github.com/ivarcia)
* [Italian translation update](https://github.com/adobe/brackets/pull/8964) (+ [part 2](https://github.com/adobe/brackets/pull/9422)) by [Denisov21](https://github.com/Denisov21)
* [Persian translation update](https://github.com/adobe/brackets/pull/9105) (+ [part 2](https://github.com/adobe/brackets/pull/9390)) by [Mohammad Yaghobi](https://github.com/mohammadyaghobi)
* [Romanian translation update](https://github.com/adobe/brackets/pull/9116) by [Micleusanu Nicu](https://github.com/micnic)
* [Spanish translation update](https://github.com/adobe/brackets/pull/9078) by [Jaime Olmo](https://github.com/jamesxv7)
* [Example of using package.json `i18n` field](https://github.com/adobe/brackets/pull/8828) by [Denisov21](https://github.com/Denisov21)


#### Pulling source code from Git
* Rebuilding/updating brackets-shell is _optional_ for this release.
* Some submodules were updated this sprint. Run `git submodule update` to ensure your source tree is fully up to date.


Bugs fixed in Release 0.44
--------------------------
For details on the bugs addressed, please refer to [closed Release 0.44 bugs](https://github.com/adobe/brackets/issues?q=is%3Aclosed+milestone%3A%22Release+0.44%22). Not all fixed bugs will be caught by this search query, however.