Unity Reference Assemblies

These are the reference assemblies used for the .NET Framework API Compatibility Level option in Unity.

They consist of the union of the .NET Framework 4.8 API and the .NET Standard 2.1 API.

To create them:

1. Clone the IL2CPP repository
2. Run perl build.pl in the repository root
3. Run build\tools\net5.0\ProfileTools.exe --generate=unity48api

The output should be something like:
Profile written to : C:\Unity\dev\il2cpp-alt\il2cpp-alt-1\build\profiles\unity-4.8-api

Unity Engine Reference Assemblies

These are the reference assemblies used to compile the Unity Engine assemblies.

They consist of the intersection of the .NET Framework 4.8 API and the .NET Standard 2.1 API, using a 
.NET Framework-based ecosystem (mscorlib.dll and friends).

To create them:

1. Clone the IL2CPP repository
2. Run perl build.pl in the repository root
3. Run build\tools\net5.0\ProfileTools.exe --generate=UnityEngineApi

The output should be something like:
Profile written to : C:\Unity\dev\il2cpp-alt\il2cpp-alt-1\build\profiles\unity-engine-api