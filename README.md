# game-ai
Mat Buckland: Programming Game AI by Example

I retargeted and fixed compilation for most of the projects under Visual Studio 2019.

Testing setup was Visual Studio v16.7.3, Debug Configuration, Win32 platform. Your mileage may vary.

DISCLAIMER: This repo is not meant for future support of any kind. Its only purpose is to be handy if like me, you're reading this book and would like to run the examples on a modern Windows.


Unfixed
=======

The "Buckland_Chapter6_Scripting_Source" folder is left widely unfixed as it was too hard to link Luabind, I gave up.

I first couldn't rebuild Luabind from source because the compile fails in complex Boost template code for some obscure reason.

I then managed to get precompiled Luabind binaries on the Web, stealing them from the zip at [this CodeProject blog](https://www.codeproject.com/Articles/22638/Using-Lua-and-luabind-with-Ogre-3d), but had to introduce some kind of weird double linking of the Lua dll under two different names, as the Luabind DLL depended on a Lua DLL that was named differently (lua-5.1.dll vs Lua51.dll).
Sadly, it made projects compile but crash instantly at runtime for an unknown reason.



- 원본 소스 추가함 (Original source added).
