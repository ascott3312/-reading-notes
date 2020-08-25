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

Readme Best Practices
A place to copy-paste your README.md from

One of the most crucial things in your open source project is the README.md file. This repository has a ready-to-copy-paste template you can use for all your projects.

Getting started
Copy the README-default.md file for yourself and start editing! At the root of your project, run:

curl https://raw.githubusercontent.com/jehna/readme-best-practices/master/README-default.md > README.md
The code above fetches the README-default.md file from this repository and renames it to README.md.

Fill with your own text
The default template has some guiding text to get you started. However you'll need to edit the file with your own text to use it with your project.

atom README.md
If you're using Atom code editor, the code above opens the file for editing. If necessary, substitute with your preferred markdown editor.

Add to git and push
After you've filled your README.md file with your own project's text, you should push it to your GitHub project:

git add README.md
git commit -m "Added: README"
git push
This adds the README.md file to your git repository, creates a commit for it and pushes it to GitHub (or other preferred remote repository).

Features
This project makes it easy to:

Bootstrap your open source project properly
Make sure everyone gets what you're trying to achieve with your project
Follow simple instructions for a perfect README.md
Contributing
As I use this for my own projects, I know this might not be the perfect approach for all the projects out there. If you have any ideas, just open an issue and tell me what you think.

If you'd like to contribute, please fork the repository and make changes as you'd like. Pull requests are warmly welcome.

If your vision of a perfect README.md differs greatly from mine, it might be because your projects are for vastly different. In this case, you can create a new file README-yourplatform.md and create the perfect boilerplate for that.

E.g. if you have a perfect README.md for a Grunt project, just name it as README-grunt.md.

Related projects
Here's a list of other related projects where you can find inspiration for creating the best possible README for your own project:

Billie Thompson's README template
A list of awesome READMEs
Akash Nimare's kickass README guide
Dan Bader's README template
Licensing
This project is licensed under Unlicense license. This license does not require you to take the license with you to your project.

About
Best practices for writing a README 
