<<<<<<< HEAD
﻿# File and Stream I/O
=======
# File and Stream I/O
>>>>>>> 44afef69c804e45a453d15eb3b021ec5c0f85aab

## Defintion
-- File and stream I/O (input/output) refers to the transfer of data either to or from a storage medium.
-- In the .NET Framework, the System.IO namespaces contain types that enable reading and writing, both synchronously and asynchronously, on data streams and files.
-- These namespaces also contain types that perform compression and decompression on files, and types that enable communication through pipes and serial ports.

### Here are some commonly used file and directory classes:

 1. File - provides static methods for creating, copying, deleting, moving, and opening files, and helps create a FileStream object.

 1. FileInfo - provides instance methods for creating, copying, deleting, moving, and opening files, and helps create a FileStream object.

 1. Directory - provides static methods for creating, moving, and enumerating through directories and subdirectories.

 1. DirectoryInfo - provides instance methods for creating, moving, and enumerating through directories and subdirectories.

 1. Path - provides methods and properties for processing directory strings in a cross-platform manner.

#### Streams involve three fundamental operations:

1. Reading - transferring data from a stream into a data structure, such as an array of bytes.

1. Writing - transferring data to a stream from a data source.

1. Seeking - querying and modifying the current position within a stream.

#### How to: Write text to a file

1. This topic shows different ways to write text to a file for a .NET app.

1. The following classes and methods are typically used to write text to a file:

1. StreamWriter contains methods to write to a file synchronously (Write and WriteLine) or asynchronously (WriteAsync and WriteLineAsync).

1. File provides static methods to write text to a file, such as WriteAllLines and WriteAllText, or to append text to a file, such as AppendAllLines, AppendAllText, and AppendText.

1. Path is for strings that have file or directory path information. It contains the Combine method and, in .NET Core 2.1 and later, the Join and TryJoin methods, which allow concatenation of strings to build a file or directory path.

##### How to: Read and write to a newly created data file

The System.IO.BinaryWriter and System.IO.BinaryReader classes are used for writing and reading data other than character strings. The following example shows how to create an empty file stream, write data to it, and read data from it.

<<<<<<< HEAD
The example creates a data file called Test.data in the current directory, creates the associated BinaryWriter and BinaryReader objects, and uses the BinaryWriter object to write the integers 0 through 10 to Test.data, which leaves the file pointer at the end of the file. The BinaryReader object then sets the file pointer back to the origin and reads out the specified content.
=======
The example creates a data file called Test.data in the current directory, creates the associated BinaryWriter and BinaryReader objects, and uses the BinaryWriter object to write the integers 0 through 10 to Test.data, which leaves the file pointer at the end of the file. The BinaryReader object then sets the file pointer back to the origin and reads out the specified content.
=======
3 Unit Testing

## Unit Testing
First, let’s clear up any misconceptions by talking about what doesn’t count.  Not every test you could conceivably write qualifies as a unit test.

If you write code that stuffs things into a database or that reads a file from disk, you have not written a unit test.  Unit tests don’t deal with their environment and with external systems to the codebase.  If it you’ve written something that can fail when run on a machine without the “proper setup,” you haven’t written a unit test.

### Dowload .NERT
Download the .NET SDK
As of this writing, the .NET SDK is available for download for Windows, Linux, and macOS. Once you've downloaded and installed the SDK, open a fresh command prompt of your choice (CMD, PowerShell, Bash, etc.) and make sure that you can access the CLI by typing dotnet --version. You should be rewarded with a single line, describing the version of the .NET Core SDK you have installed:

$ dotnet --version
2.2.103
Note: the first time you run the dotnet command, it may perform some post-installation steps. Once these one-time actions are done, it will execute your command.

Create the unit test project
An xUnit.net test project for .NET Core, just like other xUni
t.net test projects for .NET, starts with a class library. From the command line, create a folder for your test project, change into it, and then create the project:

$ mkdir MyFirstUnitTests
$ cd MyFirstUnitTests
$ dotnet new classlib
The template "Class library" was created successfully.
>>>>>>> 44afef69c804e45a453d15eb3b021ec5c0f85aab
