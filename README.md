# Open3D-iOS

Swift package to use Open3D in iOS apps. This repository is a fork of https://github.com/kewlbear/Open3D.git, while the original repository is not working on xcode 15 and lack of maintaining. Therefore, I decided to fork it here, and keep a working version.

## Installation

In xcode, add this repository as a Swift Package.
```
https://github.com/thomas-graphopti/Open3D-iOS.git
```

## Usage

### Use with Python-iOS
```
import Open3DSupport
import NumPySupport
import PythonSupport
import PythonKit

PythonSupport.initialize()
Open3DSupport.sitePackagesURL.insertPythonPath()
NumPySupport.sitePackagesURL.insertPythonPath()
let o3d = Python.import("open3d")
...
```

Above code requires `https://github.com/pvieito/PythonKit.git` package.

See Example directory for more.

If you want to build XCFrameworks yourself, see https://github.com/kewlbear/Open3D.

### Use with Objective-C
We can also use the objct-C wrapper of Open3D. Just include <Open3D/Open3D.h> in your .mm wrapper file. You can use ChatGPT/Claude to guide you for further integration.

## Acknowledgement
This repository is a fork of https://github.com/kewlbear/Open3D.git, all credits go to the original authors.

## License
MIT

