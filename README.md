# Exporting-F-functions-to-DLL

Basic code for F# library which exports two functions "add" and "write_line".
Based on the idea of https://secanablog.wordpress.com/2020/02/01/writing-a-native-library-in-f-which-can-be-called-from-c/ but updated to NativeAOT.


Compile with

dotnet publish /p:NativeLib=Shared /p:SelfContained=true -r win-x64 -c release

to export dlls to bin/../....../native directory
