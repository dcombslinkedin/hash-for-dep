# hash-for-dep [![Build Status](https://travis-ci.org/stefanpenner/hash-for-dep.svg?branch=stuff)](https://travis-ci.org/stefanpenner/hash-for-dep) [![Build status](https://ci.appveyor.com/api/projects/status/wf2u3j6lc52hdd21?svg=true)](https://ci.appveyor.com/project/embercli/hash-for-dep)

Generate a hash representing the stats of this module files and all its descendents files.

```js
var hasForDep = require('hash-for-dep');

hasForDep('rsvp'); // if RSVP is a dependency of the current project, you will get a checksum for it
hasForDep('rsvp', 'path/to/other/project'); //  you will get a checksum for RSVP resolved relative to the provided root
```
