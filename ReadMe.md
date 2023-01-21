# C# Hello World with Visual Studio Code

This is a very basic C# Hello World app written in Visual Studio Code. Yes 'Code', not VS. I followed the tutorial from [Visual Studio Code for C# Developers | .NET Conf 2022](https://www.youtube.com/watch?v=fuBi4d7k1-M). 

.NET is an open source developer platform, created by Microsoft, for building many different types of applications.

C# is a simple, modern, object-oriented, and type-safe programming language.

## How To

Instructions: 

1. Download and install Visual Studio Code from https://code.visualstudio.com/Download
2. Download and install the .Net SDK from https://dotnet.microsoft.com/en-us/download
3. Follow Tim's instructions from the Video

Commands I used: 

```console
dotnet new sln --name "HelloWorld"
dotnet new gitignore
dotnet new console --name "HelloWorld"
dotnet new classlib --name "Core"
dotnet sln add '.\HelloWorld\CSharp Hello World.csproj'
dotnet sln add '.\Core\Core.csproj'
dotnet add '.\HelloWorld\CSharp Hello World.csproj' reference '.\Core\Core.csproj'
cd .\Core
dotnet add package 'Dapper'
```

## Remark

Another great beginner tutorial is the one from the Microsoft Learning center: [.NET Tutorial - Hello World in 5 minutes](https://dotnet.microsoft.com/en-us/learn/dotnet/hello-world-tutorial/intro)