# OS
This is Windows-only stuff. Visual Studio 2019 will install and run on the following operating systems (64 bit recommended; ARM is not supported):

* Windows 10 version 1703 or higher: Home, Professional, Education, and Enterprise (LTSC and S are not supported);
* Windows Server 2019: Standard and Datacenter;
* Windows Server 2016: Standard and Datacenter;
* Windows 8.1 (with Update 2919355): Core, Professional, and Enterprise;
* Windows Server 2012 R2 (with Update 2919355): Essentials, Standard, Datacenter;
* Windows 7 SP1 (with latest Windows Updates): Home Premium, Professional, Enterprise, Ultimate.


# Visual studio building tools.

If you only want the command-line toolset, download the [Build Tools for Visual Studio](https://visualstudio.microsoft.com/downloads/#build-tools-for-visual-studio-2019). 
Yoy have to download <b>All downloads / Tools for Visual Studio 2019 / Build Tools for Visual Studio 2019</b>. Run <i>vs_BuildTools.exe</i> to install all necessary components.

## Off-line instalation.

First download all necesary packages using this command:

```
vs_buildtools-2019.exe --layout VS_BuildTools ^
--add Microsoft.VisualStudio.Workload.MSBuildTools ^
--add Microsoft.VisualStudio.Workload.UniversalBuildTools ^
--add Microsoft.VisualStudio.Component.VC.CoreBuildTools ^
--add Microsoft.VisualStudio.Component.VC.Redist.14.Latest ^
--add Microsoft.VisualStudio.Component.Windows10SDK ^
--add Microsoft.VisualStudio.Component.TestTools.BuildTools ^
--add Microsoft.VisualStudio.Component.VC.ASAN ^
--add Microsoft.VisualStudio.Component.VC.CMake.Project ^
--add Microsoft.VisualStudio.Component.VC.Tools.x86.x64 ^
--add Microsoft.VisualStudio.Component.Windows10SDK.18362 ^
--add Microsoft.Component.MSBuild ^
--add Microsoft.Component.VC.Runtime.UCRTSDK ^
--add Microsoft.Net.Component.4.6.1.TargetingPack ^
--add Microsoft.Net.Component.4.8.SDK ^
--add Microsoft.VisualStudio.Component.Roslyn.Compiler ^
--add Microsoft.VisualStudio.Component.TextTemplating ^
--add Microsoft.VisualStudio.Component.VC.140 ^
--add Microsoft.VisualStudio.Component.VC.ATL ^
--add Microsoft.VisualStudio.Component.VC.ATLMFC ^
--add Microsoft.VisualStudio.Component.VC.CLI.Support ^
--add Microsoft.VisualStudio.Component.VC.CoreIde ^
--add Microsoft.VisualStudio.Component.VC.Llvm.Clang ^
--add Microsoft.VisualStudio.Component.VC.Llvm.ClangToolset ^
--add Microsoft.VisualStudio.Component.VC.Modules.x86.x64 ^
--add Microsoft.VisualStudio.Component.VC.v141.x86.x64 ^
--add Microsoft.VisualStudio.Component.Windows10SDK.16299 ^
--add Microsoft.VisualStudio.Component.Windows10SDK.17134 ^
--add Microsoft.VisualStudio.Component.Windows10SDK.17763 ^
--add Microsoft.VisualStudio.ComponentGroup.NativeDesktop.Core ^
--add Microsoft.VisualStudio.ComponentGroup.NativeDesktop.Llvm.Clang ^
--add Microsoft.VisualStudio.ComponentGroup.UWP.VC.BuildTools ^
--add Microsoft.VisualStudio.ComponentGroup.UWP.VC.v141.BuildTools ^
--lang en-US
```
To run off-line instalation, you have to run it from the newly created directory (<i>VS_BuildTools</i> in my case. Run this command:

```
vs_buildtools.exe --noweb
```
## Be aware.

It takes more then 20Gb of the disk space :-(, if the SDK stuff is installed!

