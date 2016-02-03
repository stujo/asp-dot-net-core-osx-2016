.NET Coire on OSX 2016 Notes
================

* 2016 - Notes on Setting up .NET Core on OSX x64

#Setting Up

* Visit [https://dotnet.github.io/getting-started/](https://dotnet.github.io/getting-started/) to get 
* [The OSX installation pkg](https://dotnetcli.blob.core.windows.net/dotnet/dev/Installers/Latest/dotnet-osx-x64.latest.pkg)
* The package was not signed correctly :( 
* [Domain Looks Legit](http://www.whois.com/whois/windows.net)
* Installer takes - 100MB
* Brew Install OpenSSL http://brewformulas.org/Openssl


# Hello World
* The installer adds ``/usr/local/share/dotnet/bin`` to the path, so you'll need to open a new terminal tab

##Create Project
```
$ mkdir hello_world
$ cd hello_world
$ dotnet new
Created new C# project in /work/dotnet/hello_world.
$ ls -la
total 24
drwxr-xr-x  5 stuart  staff  170 Feb  3 15:51 .
drwxr-xr-x  3 stuart  staff  102 Feb  3 15:45 ..
-rwx------  1 stuart  staff  383 Feb  3 15:51 NuGet.Config
-rwx------  1 stuart  staff  202 Feb  3 15:51 Program.cs
-rwx------  1 stuart  staff  227 Feb  3 15:51 project.json
```

##Install Dependencies
```
$ dotnet restore
```
