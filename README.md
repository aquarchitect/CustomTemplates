No Interface Builder (IB)
=========================

This repository includes:

* __Project Templates__:
    - _Minimum Base_: provides a minimum starting point of iOS application projects. The template excludes __Main.storyboard__ and contains __Bridging.h__ to centralize dependencies.
    - _Minimum Application_: starts off from _Minimum Base_ with a slight modification that fits the personal workflow. The template simply gives an option to include [`MyKit`](https://github.com/aquarchitect/MyKit) library.

* __File Templates__:
    - _Licensed Swift File_: provides a minimum starting point of Swift files. The template is designed to work side-by-side with _Minimum Base_ project template by omitting importing frameworks lines (because of __Bridging.h__).

> You can make _Minimum Base_ template available in the project templates' list by changing value of `Concrete` property to the following:

```xml
<key>Concrete</key>
<true/>
```

#### Instruction
Installation directory: `*~/Library/Developer/Templates/`

#### Notes

As the architecture heavily relies on the distinction between data model and view model, directory tree should be structured like below:

<big><pre>
Sources
├── Data
|   ├── Models
|   └── Controllers
├── View
|   ├── Controllers
|   └── Components
└── Extension
Resources
Tests
</pre><big>

> This design is inspired by the directory structure of Swift Package Manager.
> Unfortunately, I am unable to create this structure directly into Xcode project template.

#### License
All content is licensed under the terms of the MIT open source license.
