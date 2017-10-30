# dotnet-mono-docker
[![Docker Build Status](https://img.shields.io/docker/build/johnnyasantoss/dotnet-mono-docker.svg)](https://hub.docker.com/r/johnnyasantoss/dotnet-mono-docker/builds/) [![Docker Pulls](https://img.shields.io/docker/pulls/johnnyasantoss/dotnet-mono-docker.svg)](https://hub.docker.com/r/johnnyasantoss/dotnet-mono-docker) [![Docker Stars](https://img.shields.io/docker/stars/johnnyasantoss/dotnet-mono-docker.svg)](https://hub.docker.com/r/johnnyasantoss/dotnet-mono-docker)

----

Base docker image including the [dotnet cli][dotnet] and [Mono][mono]



## Base operating system

Due to importing from [microsoft/dotnet][hub-dotnet] the operating system is Debian.
Using Debian 8 (Jessie) in 1.1 SDK and Debian 9 (Stretch) in 2.0 SDK images.

## What's included

Mono and .NET Core

## Tags

https://hub.docker.com/r/johnnyasantoss/dotnet-mono-docker/tags/

### SDK tag

Good for building!

- dotnet1.1-mono4.8.1-sdk
  - .NET Core 1.1 SDK
  - Mono (version 4.8.1)
    - mono-complete
    - msbuild (15.1.0.0)
    - ca-certificates-mono
    - referenceassemblies-pcl
  - nuget (latest)
- dotnet2.0-mono5.2-sdk
  - .NET Core 2.0.2 SDK
  - Mono (version 5.2.0.224)
    - mono-complete
    - msbuild (15.3.0.0)
    - ca-certificates-mono
    - referenceassemblies-pcl
  - nuget (4.3.0.4406)

### Runtime tag

Good for running!

- dotnet1.1-mono4.8.1-runtime
  - .NET Core 1.1 Runtime
  - Mono (version 4.8.1)
    - mono-devel
    - mono-xsp4 (to run ASP.NET applications)
    - ca-certificates-mono
    - referenceassemblies-pcl
  - nuget (latest)
- dotnet2.0-mono5.2-runtime
  - .NET Core 2.0.2 Runtime
  - Mono (version 5.2.0.224)
    - mono-devel
    - mono-xsp4
    - ca-certificates-mono
    - referenceassemblies-pcl
  - nuget (4.3.0.4406)

## Thanks to [@cl0sey][cl0sey]

This repo is a fork of [CL0SeY/dotnet-mono-docker][forked-repo]!

Thanks!

 [cl0sey]: https://github.com/CL0SeY
 [forked-repo]: https://github.com/CL0SeY/dotnet-mono-docker
 [dotnet]: https://dot.net
 [mono]: http://www.mono-project.com/
 [hub-dotnet]: https://hub.docker.com/r/microsoft/dotnet
