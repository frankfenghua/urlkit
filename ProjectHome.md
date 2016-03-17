# UrlKit Project Page #

UrlKit supports Adobe Flex applications that need to expose URLs and window titles in the browser to represent their state.  These URLs can be bookmarked, accessed via the Back button, etc.  Such states typically represents some notion of location within the app, but in general can be mapped to any aspect of the application.

Specifically, UrlKit provides:

  * a Javascript library for deep linking in Flex 2 (in Flex 3, this is provided by the platform)

  * a library of declarative rule objects that describes the lexical elements of the application's URL and bidirectionally binds them to variables

  * a sample application

Joe Berkovitz developed UrlKit in collaboration with Todd Rein of Adobe.  To find out why, read the [Rationale](Rationale.md).

## Latest News ##

Version 0.92 fixes a distribution script error in version 0.91 that failed to copy the JavaScript files for the sample application into the orrect directory.

Version 0.91 now uses back-ported Flex 3 deep linking in its Flex 2 version, providing good cross-browser support for IE7 and Safari.  The new `enabled` property of `FlexBrowserManagerAdapter` permits applications to delay the initialization of UrlKit until their application reaches a fully initialized state.  The new `navigate()` method permits applications to optionally navigate by directly specifying a URL rather than by modifying a navigational model.