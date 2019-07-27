This repository contains two packages for testing the resolution of the Nimble package manager issue with multiple downloads of the same package. The two packages are dependencies of the package `issue678` in the Nimble tests directory, and also the `issue678_dependency_1` package is dependency of the `issue678_dependency_2` package.

If the issue [nim-lang/nimble#678](https://github.com/nim-lang/nimble/issues/678) is resolved it is expected on installing the `issue678` package, the two packages to be downloaded and installed only once, otherwise the `issue678_dependency_1` package, which is both first and second level dependency of `issue678`, will be downloaded and installed two times.

See https://github.com/nim-lang/nimble/issues/678
