# File and Stream I/O

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

The example creates a data file called Test.data in the current directory, creates the associated BinaryWriter and BinaryReader objects, and uses the BinaryWriter object to write the integers 0 through 10 to Test.data, which leaves the file pointer at the end of the file. The BinaryReader object then sets the file pointer back to the origin and reads out the specified content.