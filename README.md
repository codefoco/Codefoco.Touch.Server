[![Logo](https://raw.githubusercontent.com/codefoco/Codefoco.Touch.Server/master/Codefoco.Touch.Server.png)]()

 
 Codefoco.Touch.Server
 =====================



 
| NuGet | Build status |
| ------|------|
|[![nuget](https://badgen.net/nuget/v/Codefoco.Touch.Server?icon=nuget)](https://www.nuget.org/packages/Codefoco.Touch.Server)|[![Build Status](https://dev.azure.com/codefoco/NuGets/_apis/build/status/Codefoco.Touch.Server/Codefoco.Touch.Server?branchName=master)](https://dev.azure.com/codefoco/NuGets/_build/latest?definitionId=6&branchName=master)|

 This NuGet wraps the [Touch.Server](https://github.com/spouliot/Touch.Unit/tree/master/Touch.Server) from [Sebastien Pouliot](https://github.com/spouliot/), to make easier to Run [NUnitLite](https://docs.microsoft.com/en-us/xamarin/ios/deploy-test/touch.unit) from command line using MSBuild


Use msbuild to run the `iOS` or `tvOS` tests.


Running iOS/tvOS tests:

    msbuild /t:RunSimulatorTests MyiOSTest.csproj /p:Configuration=Release /p:Platform=iPhoneSimulator
