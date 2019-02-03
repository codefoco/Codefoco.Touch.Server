[![Logo](https://raw.githubusercontent.com/codefoco/Codefoco.Touch.Server/master/Codefoco.Touch.Server.png)]()

 
 Codefoco.Touch.Server
 =====================

 
| NuGet | Build status |
| ------|------|
|[![nuget](https://img.shields.io/nuget/v/Codefoco.Touch.Server.svg)](https://www.nuget.org/packages/Codefoco.Touch.Server)|[![Build status](https://dev.azure.com/NLua/NLua/_apis/build/status/Codefoco.Touch.Server)](https://dev.azure.com/NLua/NLua/_build/latest?definitionId=8)|



NuGet package for Touch.Server

🐛 a manual edit is necessary in order to add the `.targets` file to `.csproj`.
Append the import element to `.csproj` to add the `RunSimulatorTests` target to the project.

    <Import Project="..\..\..\packages\Codefoco.Touch.Server.1.0.7\build\RunSimulatorTests.targets" Condition="Exists('..\..\..\packages\Codefoco.Touch.Server.1.0.7\build\RunSimulatorTests.targets')" />

Running iOS/tvOS tests:

    msbuild /t:RunSimulatorTests MyiOSTest.csproj /p:Configuration=Release /p:Platform=iPhoneSimulator
