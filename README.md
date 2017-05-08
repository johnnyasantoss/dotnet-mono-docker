# dotnet-mono-docker
Base docker image including the [dotnet cli][dotnet] and [Mono][mono]


## Base operating system

The base operating system is Debian 8 (Jessie) due to importing from [microsoft/dotnet](hub-dotnet)

## What's included

### SDK tag

Good for building!

- .NET Core 1.1 SDK
- Mono (version 4.8.1)
  - mono-complete
  - ca-certificates-mono
  - referenceassemblies-pcl
  - nuget 3.5.0

### Runtime tag

Good for running!

- .NET Core 1.1 Runtime
- Mono (version 4.8.1)
  - mono-devel
  - mono-xsp4 (to run ASP.NET applications)
  - ca-certificates-mono
  - referenceassemblies-pcl
  - nuget 3.5.0

## Thanks to @cl0sey

This repo is a fork of CL0SeY/dotnet-mono-docker!
Thanks!

 [dotnet]: https://dot.net
 [mono]: http://www.mono-project.com/
 [hub-dotnet]: https://hub.docker.com/r/microsoft/dotnet
