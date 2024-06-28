# Suppe
![c06bfd80-25b4-4f2a-95f0-1ef84f1b9372](https://github.com/chaoscalm/Suppe/assets/7214961/30162b95-2836-4b2d-bd40-fd8d7969556c)


Suppe is an Xposed module to disable SSL verification and pinning on Android using the excellent technique provided by [Mattia Vinci](https://codeshare.frida.re/@sowdust/universal-android-ssl-pinning-bypass-2/). The effect is specified by the scope.

---

## Requirements
* An Xposed-compatible hooking system. 
    * [LSPosed Mod](https://github.com/mywalkb/LSPosed_mod) 

## Tested
* Android 14 QPR3, ARM64, LSPosed Mod 1.9.3

## Troubleshooting
* Some apps implement custom certificate checking, bypassing this hook. Try sniffing Chromium traffic, if you don't get an invalid certificate error then this module is working as it should.

* Check your LSPosed logs, chances are this module couldn't hook the correct method.

## Credits
* [ViRb3](https://github.com/ViRb3/TrustMeAlready) Original project
  
* [jpacg](https://github.com/jpacg/TrustMeAlready) Updated dependencies and Main.java
  
* [D3fau4](https://github.com/D3fau4/TrustMeAlready) Updated dependencies and refactor
