# Rayman from scratch

Rayman from scratch is yet another attempt at reverse engineer and reimplement Rayman 1 source code.

In 2016, UbiSoft re-released Rayman as “Rayman Classic” for iOS and Android.

The Android APK contains a `libSparkApp.so` library, for both x86 and ARM, that still contains all of the symbols for functions, and possibly global variables, of the entire source code.
Simple examination of the function name reveals that the source code of the MS-DOS version has been used.

The goal of this project is to do like Jeff Harris's Carmageddon reimplementation from scratch: rebuilt the source code, using SDL2, to have a fully working and faithful reimplementation of the MS-DOS binary that runs on modern hardware and operating systems.

Text files `1.txt` and `2.txt` contains the output of the command `objdump -TC libSparkApp.so` for two revisions of the x86 Android release of Rayman Classic.
