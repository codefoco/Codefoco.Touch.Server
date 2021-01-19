[![Logo](https://raw.githubusercontent.com/codefoco/Codefoco.Touch.Server/main/Codefoco.Touch.Server.png)]()

 
 Codefoco.Touch.Server
 =====================



 
| NuGet | Build status |
| ------|------|
|[![nuget](https://badgen.net/nuget/v/Codefoco.Touch.Server?icon=nuget)](https://www.nuget.org/packages/Codefoco.Touch.Server)|[![Build Status](https://dev.azure.com/codefoco/NuGets/_apis/build/status/Codefoco.Touch.Server/Codefoco.Touch.Server?branchName=main)](https://dev.azure.com/codefoco/NuGets/_build/latest?definitionId=6&branchName=main)|

 This NuGet wraps the [Touch.Server](https://github.com/spouliot/Touch.Unit/tree/main/Touch.Server) from [Sebastien Pouliot](https://github.com/spouliot/), to make easier to Run [NUnitLite](https://docs.microsoft.com/en-us/xamarin/ios/deploy-test/touch.unit) from command line using MSBuild


Dependencies
---------
Before building fetch the submodules:

    git submodule update --init --recursive

Building
---------
    msbuild

Testing
---------
Use msbuild to run the `iOS` or `tvOS` tests

    msbuild /t:RunSimulatorTests MyiOSTest.csproj /p:Configuration=Release /p:Platform=iPhoneSimulator
