---
layout: post
title:  "Glover 1.0.0 released!"
date:   2015-03-22 17:43:11
category: iOS
---
I'm proud to announce that Glover v1.0.0 is released!

The main purpose for creating this framework was to reduce complexity of CoreData's setup when one would want to use multiple context approach to keep the UI responsive even when there are 1000's of data changes being processed. It is achieved by using multiple contexts on separate threads & async saving.

Main highlights of this release are:
  
  * multiple parent-child context approach (requires iOS5+)
  * final data save done in background thread
  * fully compatible with *NSFetchedResultsController* (main context on main thread)
  * spawning additional background worker contexts for large data changes

You can download the framework [here][glover-release]. File all bugs/feature requests at [Glover’s GitHub repo][glover-gh].

[glover-release]: https://github.com/MobileToolkit/Glover-iOS/releases/tag/1.0.0
[glover-gh]:      https://github.com/MobileToolkit/Glover-iOS/
