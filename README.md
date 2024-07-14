Process Hider uses Windows API Hooking to Hide a Process from TaskManager. It utilises Minhook Library to hook NtQuerySystemInformation function so whenever NtQuerySystemInformation 
is called our function executes which removes the chosen process from Process List returned by the original function.
There are 2 projects inside the repo, the main one is ProcessHider which produces the DLL that is injected inside 
Task Manager. The second one is the DLL injector whose main job is to inject the DLL and pass the name of the process to hide.

To Build Or Combile:
Downlaod Extention MSVC V140 - VS2015 - C++ Build Tools
And Change Settings Project To (Release - 64) And Rebuild Soultion

This Method Developer: kernelm0de
Solve Software Bug Problems: mekky0x0
