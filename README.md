Xcode Templates
================

[![Platform Support](https://img.shields.io/badge/platforms-iOS%20-lightgrey.svg?style=flat-square)](https://developer.apple.com/xcode/download/)

This repository includes:

* __Project Templates__:
    - _Minimum Base_: provides a minimum starting point of iOS application projects. The template excludes __Main.storyboard__ and contains __Bridging.h__ a bridging header file as to centrally globalize all of needed frameworks.
    - _Minimum Application_: starts off from _Minimum Base_ template with a slight modification that fits my personal work flow. The template simply gives an option of include [`MyKit`](https://github.com/aquarchitect/MyKit) library.

* __File Templates__:
    - _Licensed Swift File_: provides a minimum starting point of empty Swift files with embedded __MIT Licensed__/__Unlicensed__ header. The template is designed to work side-by-side with _Minimum Base_ project template; by omitting importing frameworks lines (because of __Bridging.h__).

> You can make _Minimum Base_ template available in the project templates' list by changing value of `Concrete` property to the following:

```xml
<key>Concrete</key>
<true/>
```

#### Instruction
Installation directory: `*~/Library/Developer/Templates/`

#### License
All content is licensed under the terms of the MIT open source license.