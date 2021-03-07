# Getting Started
## Prepare vcpkg
See [Quick Start: Windows](https://github.com/microsoft/vcpkg#quick-start-windows).

### To install vcpkg as a sub-module/sub-directory of your project

From the root directory of your project, run:
````shell
> git clone https://github.com/microsoft/vcpkg
> ./vcpkg/bootstrap-vcpkg.bat
````

Then define the following in CLion's project CMake settings in order for CMake to use vcpkg
(Settings > Build, Execution and Deployment > CMake):
````
-DCMAKE_TOOLCHAIN_FILE=vcpkg/scripts/buildsystems/vcpkg.cmake
````

### To install vcpkg globally on your system

Define the following in CLion's project CMake settings in order for CMake to use vcpkg
(Settings > Build, Execution and Deployment > CMake):
````
-DCMAKE_TOOLCHAIN_FILE=C:/vcpkg/scripts/buildsystems/vcpkg.cmake
````

## Using vcpkg

To install the libraries for your project, run:
````shell
> vcpkg install [packages to install]
````

You can also search for the libraries you need with the search subcommand:
````shell
> vcpkg search [search term]
````
