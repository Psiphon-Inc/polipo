# Psiphon's Polipo fork

This Polipo code lives permanently and canonically at: 
https://github.com/Psiphon-Inc/polipo

This same code base must work for Android and Windows. (It's not important that
it compile under Cygwin, though.)

When you make changes to the code, you MUST wrap the changes in:

```
/* PSIPHON: maybe some text here */
...changes...
/* /PSIPHON */
```


## Building for Android

Use the NDK. Copy resulting `.so` files to appropriate subdirectories of 
`psiphon-circumvention-system/Android/PsiphonAndroidLibrary/libs`.


## Building for Windows

Use Microsoft Visual Studio 2013 for Windows Desktop (Express). Copy release
build of `polipo.exe` to `psiphon-circumvention-system/Client/psiclient/3rdParty`.
