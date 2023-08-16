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

## Creating your first 'Hello, world!' dotnet program...(without needed to type in any code)
  
-(**NOTE:** You don't need to actually type in any code here...; instead, the DotNet program itself will write the template: 'Hello, world!' file for you.)-  
  
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

-----

## Running your first 'Hello, world!' dotnet program...
  
After the DOS Command Prompt symbol: > type in...

C:\\desktop\test> dotnet run

...and, the following output should appear...
  
  Hello, world!

...warmest congratulations; and, very welcome to the wonderful world of DotNet programming.

-----
  
## Changing/editing the 'Hello, world!' code; then, re-running it...
  
Now, if you find the file called: [Program.cs]...by opening it inside of Windows Notepad text editor...;  
then, you will be able too change the code to do anything you please...
  
Currently, the code says this...

// See https://aka.ms/new-console-template for more information    
Console.WriteLine("Hello, World!");
 
Change the bottom line to say, instead...   
Console.WriteLine("Goodbye, World!");

...next, use Windows Notepad to save the changes you made.

Now, open the DOS Prompt within the same folder directory; and, type...

C:\\desktop\test>dotnet run

...the output should appear as...
  
Goodbye, world!
  
...at this point, you've learned to change the code to say whatever it is you please.

**NOTE:** The code we are 'writing/running' here...is, in fact, C#/C sharp...hence the 'Program' file name extension is: [.cs].  
  
-----

Example program 1: Greeting...(shows: input/output)  
  
string name;    
Console.Clear();  
Console.WriteLine("Type your name: ");  
name = Console.ReadLine();  
Console.WriteLine("Welcome, {0}",name);  
  
...use Windows Notepad to save the above program as being called: [Program.cs]  

...then, run it as follows...  

C:\\desktop\test>dotnet run  

Type you name:  
Paul  
Welcome, Paul  

C:\Desktop\test>  

-----

Example program 2: For loop...enumeration loop  

Console.Clear();  
int tablesNo=0;  
Console.Write("What number times tables: ");  
tablesNo = Int32.Parse(Console.ReadLine());  
Console.WriteLine();  
for (int timesNo = 1; timesNo<13; timesNo++){    
 Console.WriteLine("{0} X {1} = {2}",timesNo,tablesNo,(timesNo*tablesNo));  
}  

...use Windows Notepad to save the above program as being called: [Program.cs]  

...then, run it as follows...  

C:\\desktop\test>dotnet run  
  
What number times tables: 7 (Press ENTER key...)  

1 X 7 = 7  
2 X 7 = 14  
3 X 7 = 21  
4 X 7 = 28  
5 X 7 = 35  
6 X 7 = 42  
7 X 7 = 49  
8 X 7 = 56  
9 X 7 = 63  
10 X 7 = 70  
11 X 7 = 77  
12 X 7 = 84  

-----

## While loop(1)...entry controlled loop    

>int x=0;  
>while(x<10){  
> Console.Write("{0} ",x);  
> x++;  
>}  
>//output: 0 1 2 3 4 5 6 7 8 9  

## While loop(2)...exit controlled loop    
  
>int y=0;  
>do{  
> Console.Write("{0} ",y);  
> y++;  
>} while(y<10);    
>//output: 0 1 2 3 4 5 6 7 8 9  

-----
  
## CONCLUSION
  
I am not myself an experienced C# programmer...; so, I'm just still in the process of learning it...; thus, my programs are very simple, indeed.  Hopefully, this situation might improve over time.  
  
I am also not familiar with learning to use Microsoft DotNet technologies before; therefore, I'm pretty damned sure...there must be loads of things I'm totally missing out on knowing altogether. Again, there is much I still have to learn...; as I understand it...they say DotNet can be used to create all sorts of programs: desktop/backend/frontend/web/database/-etc.; and, using all different sorts of programming languages: C#, C++, Visual BASIC, Python, Javascript, NodeJS, -etc. Frankly, at this moment, I've really no idea how to do any of that...???
  
-----
  
## LINKS

### Microsoft...
  
https://dotnet.microsoft.com/en-us/learn/dotnet/hello-world-tutorial/intro  

In-browser tutorial (don't need to download anything)    
  
https://dotnet.microsoft.com/en-us/learn/dotnet/in-browser-tutorial/1  
  
Learn C# Tutorials

https://docs.microsoft.com/en-gb/users/dotnet/collections/yz26f8y64n7k07?WT.mc_id=dotnet-35129-website  

### DOCS  

https://aka.ms/dotnet-docs  

  
### YouTube...

What is .NET? What's C# and F#? What's the .NET Ecosystem? .NET Core Explained, what can .NET build?  
https://www.youtube.com/watch?v=bEfBfBQq7EE   
  
### Package Manager
  
https://www.nuget.org/    
                     
                        
     
  

  
  

  


