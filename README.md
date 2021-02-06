# airplay-receiver
Test implementation of an AirPlay receiver based on data found at https://nto.github.io/AirPlay.html

# Getting Started
## Prepare vcpkg
See [Quick Start: Windows](https://github.com/microsoft/vcpkg#quick-start-windows).

From the root directory, run:
````shell
> git clone https://github.com/microsoft/vcpkg
> ./vcpkg/bootstrap-vcpkg.bat
````

To install the libraries for your project, run:
````shell
> ./vcpkg/vcpkg install [packages to install]
````

You can also search for the libraries you need with the search subcommand:
````shell
> ./vcpkg/vcpkg search [search term]
````

Define the following in CLion's project CMake settings in order for CMake to use vcpkg 
(Settings > Build, Execution and Deployment > CMake):
````
-DCMAKE_TOOLCHAIN_FILE=cmake/scripts/buildsystems/vcpkg.cmake
````
