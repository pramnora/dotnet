# dotnet

-----

# DotNet, Introduction

Microsoft DotNet, is a technology I haven't really used that much before...; but, am still in the process of learning 'how to' use, right now.

-----

## Where to download...

Microsoft Dotnet can be downloaded for FREE from...

- https://dotnet.microsoft.com

-----

## Checking if DotNet is correctly installed on your system...

The first thing one needs to do is check...after already downloading/and, installing the program...to test seeing if DotNet has been installed, correctly, on your computer system...; which, in my own case, as of the date/time: 20th June 2022 15:57 PM GMT, happens to be Windows 10 Professional operating system.    

Open up a DOS command line prompt window...; and, type in after the command line prompt...  

C:\\>dotnet  

Usage: dotnet [options]  
Usage: dotnet [path-to-application]  

Options:  
  -h|--help         Display help.  
  --info            Display .NET information.  
  --list-sdks       Display the installed SDKs.  
  --list-runtimes   Display the installed runtimes.  

path-to-application:  
  The path to an application .dll file to execute.  

...if you get returned back the above list of results; then, that should mean, yes, you have successfully installed DotNet. Very well done! ;-)

-----

## How to get help...

The next thing I would check for is how to display DotNet help...

After the command line prompt type in the following...

C:\\>dotnet -h

Usage: dotnet [runtime-options] [path-to-application] [arguments]  

Execute a .NET application.  

runtime-options:  
  --additionalprobingpath <path>   Path containing probing policy and assemblies to probe for.  
  --additional-deps <path>         Path to additional deps.json file.  
  --depsfile                       Path to <application>.deps.json file.  
  --fx-version <version>           Version of the installed Shared Framework to use to run the application.  
  --roll-forward <setting>         Roll forward to framework version  (LatestPatch, Minor, LatestMinor, Major, LatestMajor, Disable).  
  --runtimeconfig                  Path to <application>.runtimeconfig.json file.  

path-to-application:  
  The path to an application .dll file to execute.  

Usage: dotnet [sdk-options] [command] [command-options] [arguments]  

Execute a .NET SDK command.  

sdk-options:  
  -d|--diagnostics  Enable diagnostic output.  
  -h|--help         Show command line help.  
  --info            Display .NET information.  
  --list-runtimes   Display the installed runtimes.  
  --list-sdks       Display the installed SDKs.  
  --version         Display .NET SDK version in use.  

SDK commands:  
  add               Add a package or reference to a .NET project.  
  build             Build a .NET project.  
  build-server      Interact with servers started by a build.  
  clean             Clean build outputs of a .NET project.  
  format            Apply style preferences to a project or solution.  
  help              Show command line help.  
  list              List project references of a .NET project.  
  msbuild           Run Microsoft Build Engine (MSBuild) commands.  
  new               Create a new .NET project or file.  
  nuget             Provides additional NuGet commands.  
  pack              Create a NuGet package.  
  publish           Publish a .NET project for deployment.  
  remove            Remove a package or reference from a .NET project.  
  restore           Restore dependencies specified in a .NET project.  
  run               Build and run a .NET project output.  
  sdk               Manage .NET SDK installation.  
  sln               Modify Visual Studio solution files.  
  store             Store the specified assemblies in the runtime package store.  
  test              Run unit tests using the test runner specified in a .NET project.  
  tool              Install or manage tools that extend the .NET experience.  
  vstest            Run Microsoft Test Engine (VSTest) commands.  
  workload          Manage optional workloads.  

Additional commands from bundled tools:  
  dev-certs         Create and manage development certificates.  
  fsi               Start F# Interactive / execute F# scripts.  
  sql-cache         SQL Server cache command-line tools.  
  user-secrets      Manage development user secrets.  
  watch             Start a file watcher that runs a command when files change.  

Run 'dotnet [command] --help' for more information on a command.  

...if you get back the above results...; then, all's good. ;-)
  
-----

## Creating your first 'Hello, world!' dotnet program...
  
-(**NOTE:** You don't need to actually type in any code here...; instead, the DotNet program itself will write the template: 'Hello, world!' code file for you.)-  
  
1> First, go to your desktop; and, there create a folder called: test...; this is being done so that you can...  
  a> very quickly and easily find where the folder is whenever you want it  
  b> so that all output files can be stored tidily inside of 'one' same folder  
  
2> Next, open up a DOS Command Prompt...and, use this to CD-Change Directory...into the 'test' folder.
  
3> When inside of the 'test' folder...after the Command Prompt symbol: > type in...
  
C:\\desktop\test> dotnet new console  (then, press ENTER key)

...this should create a number of folders/files...inside of your 'test/ folder...one of which file name is: [Program.cs]...it is inside of the [Program.cs] that your program code will be stored.   

If you open up Windows Notepad text editor application...and, drag the file [Program.cs] onto the Notepad window...it will display the following 'template' code...

// See https://aka.ms/new-console-template for more information  
Console.WriteLine("Hello, World!");


  


