# Demo Git Submodules

1. Clone the demo repositories

        git clone https://github.com/TheAutomaTom/DotNet-Dependencies.0.ExampleClassLibrary
        git clone https://github.com/TheAutomaTom/DotNet-Dependencies.1.NugetPackages
        git clone https://github.com/TheAutomaTom/DotNet-Dependencies.2.Projects
        git clone https://github.com/TheAutomaTom/DotNet-Dependencies.3.GitSubmodules
        
1. Set up the Dependents' relationship to the Provider.

- Nugets

```      
    - Creating and using a .Net 2.0 Class Library Nuget Package
        1. Open the Nuget project's solution in  VS22... 
            1. Set the build mode to `Release` from the select menu (to the left of the `Begin Debugging` button).  
            1. `Build Solution` 
                Create a DLL found within .\bin\Release` directory.
            1. Select the AppLogger project in Solution Explorer, then select Pack.
                Build the project and create the .nupkg file in `.\bin\Release`
        1. Send the .nupkg file to your nuget repository, then 

        1. Run `dotnet pack` from the directory containing the project file.
      
      1. In your dependent solution, add your nuget library to the list of nuget sources.
        1. Tools/ Nuget Package Manager/ Manage...
        1. Top right gear symbol button
        1. Nuget PAckage Manager/ Package Sources
        1. Add (plus sign in the top right)
        1. Source (specify the location of the .nupkg file)
        1. Install your new nuget library
    - 
```

- Submodules

```  
    1. Run `git submodule add https://github.com/TheAutomaTom/GitSubmodules.Library`
    1. Run `git submodule init`
    1. Run `git submodule update`
       A new folder has been created containing your gitsubmodel project.
    1. Reference the csproj file.

```

### Bibliography

- Quickstart: Create and publish a NuGet package using Visual Studio (Windows only)

    https://learn.microsoft.com/en-us/nuget/quickstart/create-and-publish-a-package-using-visual-studio?tabs=netcore-cli#create-a-class-library-project


### Pop culture references

#### Dependent-A

Big (1988)

> Q: Zoltar asks "Make your wish!"

> A: Not matter what, he says, "Your wish is granted!"

##### Dependent-B

Bob Dylan's "Blowing in the Wind" (1961)

> Q: How many times must one look up before they can see the sky?

> A: The answer, my friend, is blowing in the wind.

##### Dependent-C

Douglas Adams' The Hitchhiker's Guide to the Galaxy (1981)

> Q: What is the meaning to Life, The Universe, and Everything?

> A: 42.  







