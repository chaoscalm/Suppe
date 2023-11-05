# Suppe
Suppe is an Xposed module to disable SSL verification and pinning on Android using the excellent technique provided by [Mattia Vinci](https://techblog.mediaservice.net/2018/11/universal-android-ssl-check-bypass-2/). The effect is specified by the scope.

---

## Requirements
* An Xposed-compatible hooking system. 
    * [LSPosed](https://github.com/LSPosed/LSPosed) (Android 13)  

## Tested
* Android 13.0, ARM64, LSPosed 1.9.2

## Troubleshooting
* Some apps implement custom certificate checking, bypassing this hook. Try sniffing Chromium traffic, if you don't get an invalid certificate error then this module is working as it should.

* Check your LSPosed logs, chances are this module couldn't hook the correct method.

## Credits
* [ViRb3](https://github.com/ViRb3/TrustMeAlready) Original project
  
* [jpacg](https://github.com/jpacg/TrustMeAlready) Updated dependencies and Main.java
  
* [D3fau4](https://github.com/D3fau4/TrustMeAlready) Updated dependencies and refactor
