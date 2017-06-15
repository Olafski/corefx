<<<<<<< HEAD
### Latest News and Announcements

* [Announcement: Driving towards zero 2.0 bugs by **2017/5/10** (ZBB)](https://github.com/dotnet/corefx/issues/17619)



# .NET Core Libraries (CoreFX)

This repo contains the library implementation (called "CoreFX") for .NET Core. It includes System.Collections, System.IO, System.Xml, and many other components.
The corresponding [.NET Core Runtime repo](https://github.com/dotnet/coreclr) (called "CoreCLR") contains the runtime implementation for .NET Core. It includes RyuJIT, the .NET GC, and many other components.
Runtime-specific library code ([mscorlib](https://github.com/dotnet/coreclr/tree/master/src/mscorlib)) lives in the CoreCLR repo. It needs to be built and versioned in tandem with the runtime. The rest of CoreFX is agnostic of runtime-implementation and can be run on any compatible .NET runtime (e.g. [CoreRT](https://github.com/dotnet/corert)).



## .NET Core

Great starting page: http://dotnet.github.io

* [How to use .NET Core](https://github.com/dotnet/core/#get-started) (with VS, VS Code, command-line CLI)
  * [Install official releases](https://www.microsoft.com/net/core)
  * [Documentation](https://docs.microsoft.com/en-us/dotnet) (Get Started, Tutorials, Porting from .NET Framework, API reference, ...)
    * [Deploying apps](https://docs.microsoft.com/en-us/dotnet/articles/core/preview3/deploying)
* [Roadmap](https://github.com/dotnet/core/blob/master/roadmap.md)
* [Releases](https://github.com/dotnet/core/tree/master/release-notes)
* [Bringing more APIs to .NET Core](https://github.com/dotnet/corefx/blob/master/Documentation/project-docs/porting.md) (and why some APIs will be left out)



## How to Engage, Contribute and Provide Feedback

Some of the best ways to contribute are to try things out, file bugs, join in design conversations, and fix issues.

* [Dogfooding daily builds](https://github.com/dotnet/corefx/blob/master/Documentation/project-docs/dogfooding.md)
* If you have a question or idea, [file a new issue](https://github.com/dotnet/corefx/issues/new).

If you are having issues with the "full" .NET Framework (also called "Desktop"), the best way to file a bug is at [Connect](http://connect.microsoft.com/VisualStudio) or through [Product Support](https://support.microsoft.com/en-us/contactus?ws=support) if you have a contract.

### Issue Guide

This section is **in progress** here: [New contributor Docs - Issues](https://github.com/dotnet/corefx/wiki/Issues) (feel free to make it better - it's easy-to-edit wiki with RW permissions to everyone!)

### Contributing Guide

This section is **in progress** here: [New contributor Docs - Contributing](https://github.com/dotnet/corefx/wiki/Contributions) (feel free to make it better - it's easy-to-edit wiki with RW permissions to everyone!) 

### Useful Links

* CoreFX source index: https://source.dot.net
* API Reference docs: https://docs.microsoft.com/en-us/dotnet/core/api
* .NET API Catalog: http://apisof.net (incl. APIs from daily builds and API usage info)
* "Full" .NET Framework source index: https://referencesource.microsoft.com

### Community

* General .NET OSS discussions: [.NET Foundation forums](http://forums.dotnetfoundation.org)
* Chat with other community members [![Join the chat at https://gitter.im/dotnet/corefx](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/dotnet/corefx?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) [![.NET Slack Status](https://aspnetcoreslack.herokuapp.com/badge.svg?2)](http://tattoocoder.com/aspnet-slack-sign-up)

This project has adopted the code of conduct defined by the [Contributor Covenant](http://contributor-covenant.org/)
to clarify expected behavior in our community. For more information, see the [.NET Foundation Code of Conduct](http://www.dotnetfoundation.org/code-of-conduct).

### Reporting security issues and security bugs

Security issues and bugs should be reported privately, via email, to the
Microsoft Security Response Center (MSRC) <secure@microsoft.com>. You should
receive a response within 24 hours. If for some reason you do not, please follow
up via email to ensure we received your original message. Further information,
including the MSRC PGP key, can be found in the
[Security TechCenter](https://technet.microsoft.com/en-us/security/ff852094.aspx).



## License

.NET Core (including the corefx repo) is licensed under the [MIT license](LICENSE).



## .NET Foundation

.NET Core is a [.NET Foundation](http://www.dotnetfoundation.org/projects) project.

There are many .NET related projects on GitHub.

- [.NET home repo](https://github.com/Microsoft/dotnet) - links to 100s of .NET projects, from Microsoft and the community.
- [ASP.NET Core home](https://github.com/aspnet/home) - the best place to start learning about ASP.NET Core.



## CoreFX Project

### Daily Builds

Daily builds of .NET Core components are published to [dotnet-core MyGet gallery](https://dotnet.myget.org/gallery/dotnet-core).
The latest version number of each library can be seen in that gallery.

### Build & Test Status

|    | Inner x64 Debug | Inner x64 Release | Outer x64 Debug | Outer x64 Release |
|:---|----------------:|------------------:|----------------:|------------------:|
|**CentOS 7.1**|[![x64-debug](https://ci.dot.net/job/dotnet_corefx/job/master/job/centos7.1_debug/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/centos7.1_debug/lastCompletedBuild/testReport)|[![x64-release](https://ci.dot.net/job/dotnet_corefx/job/master/job/centos7.1_release/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/centos7.1_release/lastCompletedBuild/testReport)|[![x64-debug](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_centos7.1_debug/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_centos7.1_debug/lastCompletedBuild/testReport)|[![x64-release](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_centos7.1_release/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_centos7.1_release/lastCompletedBuild/testReport)|
|**Debian 8**|[![x64-debug](https://ci.dot.net/job/dotnet_corefx/job/master/job/debian8.4_debug/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/debian8.4_debug/lastCompletedBuild/testReport)|[![x64-release](https://ci.dot.net/job/dotnet_corefx/job/master/job/debian8.4_release/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/debian8.4_release/lastCompletedBuild/testReport)|[![x64-debug](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_debian8.4_debug/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_debian8.4_debug/lastCompletedBuild/testReport)|[![x64-release](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_debian8.4_release/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_debian8.4_release/lastCompletedBuild/testReport)|
|**Fedora 24**|[![x64-debug](https://ci.dot.net/job/dotnet_corefx/job/master/job/fedora24_debug/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/fedora24_debug/lastCompletedBuild/testReport)|[![x64-release](https://ci.dot.net/job/dotnet_corefx/job/master/job/fedora24_release/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/fedora24_release/lastCompletedBuild/testReport)|[![x64-debug](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_fedora24_debug/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_fedora24_debug/lastCompletedBuild/testReport)|[![x64-release](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_fedora24_release/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_fedora24_release/lastCompletedBuild/testReport)|
|**openSUSE 42.1**|[![x64-debug](https://ci.dot.net/job/dotnet_corefx/job/master/job/opensuse42.1_debug/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/opensuse42.1_debug/lastCompletedBuild/testReport)|[![x64-release](https://ci.dot.net/job/dotnet_corefx/job/master/job/opensuse42.1_release/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/opensuse42.1_release/lastCompletedBuild/testReport)|[![x64-debug](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_opensuse42.1_debug/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_opensuse42.1_debug/lastCompletedBuild/testReport)|[![x64-release](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_opensuse42.1_release/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_opensuse42.1_release/lastCompletedBuild/testReport)|
|**OS X 10.12**|[![x64-debug](https://ci.dot.net/job/dotnet_corefx/job/master/job/osx10.12_debug/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/osx10.12_debug/lastCompletedBuild/testReport)|[![x64-release](https://ci.dot.net/job/dotnet_corefx/job/master/job/osx10.12_release/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/osx10.12_release/lastCompletedBuild/testReport)|[![x64-debug](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_osx_debug/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_osx_debug/lastCompletedBuild/testReport)|[![x64-release](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_osx_release/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_osx_release/lastCompletedBuild/testReport)|
|**Red Hat 7.2**|[![x64-debug](https://ci.dot.net/job/dotnet_corefx/job/master/job/rhel7.2_debug/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/rhel7.2_debug/lastCompletedBuild/testReport)|[![x64-release](https://ci.dot.net/job/dotnet_corefx/job/master/job/rhel7.2_release/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/rhel7.2_release/lastCompletedBuild/testReport)|[![x64-debug](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_rhel7.2_debug/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_rhel7.2_debug/lastCompletedBuild/testReport)|[![x64-release](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_rhel7.2_release/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_rhel7.2_release/lastCompletedBuild/testReport)|
|**Ubuntu 14.04**|[![x64-debug](https://ci.dot.net/job/dotnet_corefx/job/master/job/ubuntu14.04_debug/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/ubuntu14.04_debug/lastCompletedBuild/testReport)|[![x64-release](https://ci.dot.net/job/dotnet_corefx/job/master/job/ubuntu14.04_release/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/ubuntu14.04_release/lastCompletedBuild/testReport)|[![x64-debug](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_ubuntu14.04_debug/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_ubuntu14.04_debug/lastCompletedBuild/testReport)|[![x64-release](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_ubuntu14.04_release/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_ubuntu14.04_release/lastCompletedBuild/testReport)|
|**Ubuntu 16.04**|[![x64-debug](https://ci.dot.net/job/dotnet_corefx/job/master/job/ubuntu16.04_debug/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/ubuntu16.04_debug/lastCompletedBuild/testReport)|[![x64-release](https://ci.dot.net/job/dotnet_corefx/job/master/job/ubuntu16.04_release/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/ubuntu16.04_release/lastCompletedBuild/testReport)|[![x64-debug](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_ubuntu16.04_debug/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_ubuntu16.04_debug/lastCompletedBuild/testReport)|[![x64-release](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_ubuntu16.04_release/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_ubuntu16.04_release/lastCompletedBuild/testReport)|
|**Ubuntu 16.10**|[![x64-debug](https://ci.dot.net/job/dotnet_corefx/job/master/job/ubuntu16.10_debug/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/ubuntu16.10_debug/lastCompletedBuild/testReport)|[![x64-release](https://ci.dot.net/job/dotnet_corefx/job/master/job/ubuntu16.10_release/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/ubuntu16.10_release/lastCompletedBuild/testReport)|[![x64-debug](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_ubuntu16.10_debug/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_ubuntu16.10_debug/lastCompletedBuild/testReport)|[![x64-release](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_ubuntu16.10_release/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_ubuntu16.10_release/lastCompletedBuild/testReport)|
|**PortableLinux**|[![x64-debug](https://ci.dot.net/job/dotnet_corefx/job/master/job/portablelinux_debug/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/portablelinux_debug/lastCompletedBuild/testReport)|[![x64-release](https://ci.dot.net/job/dotnet_corefx/job/master/job/portablelinux_release/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/portablelinux_release/lastCompletedBuild/testReport)|[![x64-debug](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_portablelinux_debug/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_portablelinux_debug/lastCompletedBuild/testReport)|[![x64-release](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_portablelinux_release/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_portablelinux_release/lastCompletedBuild/testReport)|
|**Windows 7**| | |[![x64-debug](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_win7_debug/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_win7_debug/lastCompletedBuild/testReport)|[![x64-release](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_win7_release/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_win7_release/lastCompletedBuild/testReport)|
|**Windows 8.1**|(x86) [![x64-debug](https://ci.dot.net/job/dotnet_corefx/job/master/job/windows_nt_debug/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/windows_nt_debug/lastCompletedBuild/testReport)|[![x64-release](https://ci.dot.net/job/dotnet_corefx/job/master/job/windows_nt_release/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/windows_nt_release/lastCompletedBuild/testReport)|[![x64-debug](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_windows_nt_debug/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_windows_nt_debug/lastCompletedBuild/testReport)|[![x64-release](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_windows_nt_release/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_windows_nt_release/lastCompletedBuild/testReport)|
|**Windows 10**| | |[![x64-debug](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_win10_debug/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_win10_debug/lastCompletedBuild/testReport)|[![x64-release](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_win10_release/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netcoreapp_win10_release/lastCompletedBuild/testReport)|
|**Windows Nano Server 2016**| | |[![x64-debug](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_winnano16_debug/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_winnano16_debug/lastCompletedBuild/testReport)|[![x64-release](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_winnano16_release/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_winnano16_release/lastCompletedBuild/testReport)|
|**Code Coverage (Windows)**| | |[![code coverage](https://ci.dot.net/job/dotnet_corefx/job/master/job/code_coverage_windows/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/code_coverage_windows/Code_Coverage_Report)|
|**Desktop**|||[![x64-debug](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netfx_windows_nt_debug/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netfx_windows_nt_debug/lastCompletedBuild/testReport)|[![x64-release](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netfx_windows_nt_release/badge/icon)](https://ci.dot.net/job/dotnet_corefx/job/master/job/outerloop_netfx_windows_nt_release/lastCompletedBuild/testReport)||
=======
﻿# .NET Core Home

The core repository is the starting point to engage in and learn about the
.NET Core stack. 

> **Note:** please note that this repository is not for filing product issues.
> If you run into an issue using .NET Core, there are multiple repos where you can 
> file an issue:
> * [dotnet/cli](https://github.com/dotnet/cli) - for CLI tools and questions
> * [dotnet/corefx](https://github.com/dotnet/corefx) - for API issues and questions
> * [dotnet/coreclr](https://github.com/dotnet/coreclr) - for runtime issues
> * [dotnet/docs](https://github.com/dotnet/docs) - for .NET documentation issues and questions
> * [dotnet/sdk](https://github.com/dotnet/sdk) - for .NET Core SDK (used by Visual Studio and CLI) issues and questions
> * [dotnet/standard](https://github.com/dotnet/standard) - for .NET Standard issues and questions
> * [nuget/home](https://github.com/nuget/home) - for NuGet questions and issues
> * [aspnet/home](https://github.com/aspnet/home) - for ASP.NET Core questions and issues.
> * [aspnet/Docs](https://github.com/aspnet/Docs) - for ASP.NET and ASP.NET Core documentation issues and questions
> * [dotnet/netcorecli-fsc](https://github.com/dotnet/netcorecli-fsc) - for F# questions and issues

> 
> We will be removing the ability to file issues on this repo in the near future.

## Get Started

If you're new to .NET Core and have 10 minutes to try it, start here: 
- [What is .NET Core?](https://www.microsoft.com/net/core/platform)
- [Get Started with the Official releases of .NET Core on Windows, OSX and Linux](https://www.microsoft.com/net/core)

If you have some more time and want to go deeper or get the latest builds:
- [Get the latest builds of .NET Core on Windows, OSX and Linux](https://github.com/dotnet/core-setup/blob/master/README.md)
- [Get the latest builds of ASP.NET Core on Windows, OSX and Linux](https://github.com/aspnet/home)

## .NET Core Platform

The .NET Core platform is made of several components, which includes the
managed compilers, the runtime, the base class libraries, and numerous application models such as
ASP.NET.

* [Roadmap](roadmap.md)
* [.NET Core Framework](https://github.com/dotnet/corefx)
* [.NET Core Runtime](https://github.com/dotnet/coreclr)
* [.NET Compiler Platform ("Roslyn")](https://github.com/dotnet/roslyn)
* [ASP.NET Core](https://github.com/aspnet/home)

## How to Engage, Contribute and Provide Feedback

All projects accept contributions:

* [.NET Core Contributing Guide](https://github.com/dotnet/corefx/blob/master/Documentation/project-docs/contributing.md)
* [.NET Compiler Platform ("Roslyn")](https://github.com/dotnet/roslyn/wiki/Contributing-Code)
* [ASP.NET Contributing Guide](https://github.com/aspnet/Home/blob/master/CONTRIBUTING.md)

You are also encouraged to start a discussion by posting on the
[.NET Foundation Forums](http://forums.dotnetfoundation.org/) or filing an
issue in the corresponding GitHub project. See the contributing guides for more
details.

## .NET Foundation

The .NET Core platform is part of the [.NET Foundation](http://www.dotnetfoundation.org/projects).

* [.NET Core Project](http://www.dotnetfoundation.org/net-core)
* [.NET Compiler Platform ("Roslyn" Project)](http://www.dotnetfoundation.org/net-compiler-platform-roslyn)
* [ASP.NET Core Project](http://www.dotnetfoundation.org/asp-net-core)

## Licenses

.NET Core platform projects typically use either the [MIT](LICENSE.TXT) or
[Apache 2](http://www.apache.org/licenses/LICENSE-2.0) licenses for code.
Some projects license documentation and other forms of content under
[Creative Commons Attribution 4.0](http://creativecommons.org/licenses/by/4.0/).

See specific projects to understand the license used.

## Understanding the relationship between .NET Core and the .NET Framework

.NET Core and the .NET Framework have (for the most part) a subset-superset
relationship. .NET Core is named "Core" since it contains the core features from
the .NET Framework, for both the runtime and framework libraries. For example,
.NET Core and the .NET Framework share the GC, the JIT and types such as
`String` and `List<T>`.

.NET Core was created so that .NET could be open source, cross platform and be
used in more resource-constrained environments. We have also published a subset
of the [.NET Reference Source](https://github.com/Microsoft/referencesource)
under the MIT license, so that you and the community can port additional .NET
Framework features to .NET Core.

## Understanding the relationship between .NET Core and Mono

Mono is an important part of the .NET ecosystem, particularly for client
scenarios (for example, Xamarin). We will look for ways to collaborate with Mono
developers and encourage them to take our code to improve Mono. We will also
look for opportunities to improve .NET Core with MIT-licensed Mono code.

An important collaboration opportunity is making .NET Core NuGet packages
(produced from this code) work on Mono. The SIMD NuGet package is a perfect
example.

## Learning about ASP.NET and .NET Core

[ASP.NET Core](https://github.com/aspnet/home) is a new cross-platform version of
ASP.NET that is designed for the cloud, and runs on Windows, Linux and Mac. It
targets .NET Core by default, but you may choose to target the .NET Framework on
Windows.
>>>>>>> upstream/master
