# BLiP.API.Template [![Build Status](https://travis-ci.org/lfmundim/Blip.Api.Template.svg?branch=master)](https://travis-ci.org/lfmundim/Blip.Api.Template) [![Nuget](https://img.shields.io/nuget/v/Blip.Api.Template.svg)](https://www.nuget.org/packages/blip.api.template) [![GitHub stars](https://img.shields.io/github/stars/lfmundim/Blip.Api.Template.svg)](https://github.com/lfmundim/Blip.Api.Template/stargazers)


## This template aims to kickstart the development of an API to be used alongside BLiP's Builder feature

## Installation
If you already have `dotnet` installed, you can install this template with the command
```sh
dotnet new -i Blip.Api.Template
```

If you don't have `dotnet` installed, follow [these](https://www.microsoft.com/net/learn/get-started-with-dotnet-tutorial) instructions from _Microsoft_ to install it on GNU/Linux, Mac or Windows, and then use the command above.

## Usage
To create a new project using this template, after installing, type in the following command
```sh
dotnet new blip-api
```
Your new project should be created in the open folder.

### Renaming the `Services` project
By default, when you create a new solution using the template, all `.csproj` files will use the name of the folder you're in (along with any mentions of `Blip.Api.Template`. You can give the `Services` project a different name should you like it using the CLI param `--Services`. 

For example, if you run the command

```bash
dotnet new blip-api --Services DifferentName.Services
```

inside a folder named `Blip.Bot.Project`, it will create a `.sln` with two projects: `Blip.Bot.Project.csproj` and `DifferentName.Services.csproj`, instead of a `Blip.Bot.Project.Services.csproj`.

## File Structure
```cs
 📁Blip.Api.Template // assuming your folder is called Blip.Api.Template. Whatever name you choose will replace all occurrences of that string in the sln
 |__📁src
    |__📁Blip.Api.Template // The Web API project Folder
    |   |__📁Controllers
    |   |   |__📃{YourControllers.cs}
    |   |   |__📃{...}
    |   |__📁Models
    |   |   |__📃{YourModelClasses.cs}
    |   |   |__📃{...}
    |   |__📁Services
    |   |   |__📃{YourServicesAndInterfaces.cs}
    |   |__📃MySettings.cs
    |   |__📃Startup.cs
    |   |__📃appsettings.json
    |__📁Blip.Api.Template.Services // (If needed) The project to use for 3rd party APIs to be consumed
    |   |__{Recommended to follow similar structure from the above project}
    |__⚙️.editorconfig
```

## Uninstallation
To uninstall the template from your local machine, use the command
```sh
dotnet new -u Blip.Api.Template
```
Your current projects that already use the template **will not** be affected.

## Feature Roadmap
* Basic controller for external link tracking
