# Suppe
![output](https://github.com/user-attachments/assets/c42e5704-0a83-427a-9ef8-35e8a29c0cea)



Suppe is an Xposed module to disable SSL certificate verification on Android using the excellent technique provided by [Mattia Vinci](https://codeshare.frida.re/@sowdust/universal-android-ssl-pinning-bypass-2/). The effect is specified by the [scope](https://github.com/LSPosed/LSPosed/wiki/Module-Scope)

---

## Requirements
* An Xposed-compatible hooking system. 
    * [LSPosed](https://github.com/JingMatrix/LSPosed) 

## Tested
* Android 14 QPR3, ARM64, LSPosed v1.10.1

## Troubleshooting
* Some apps implement custom certificate checking, bypassing this hook. Try sniffing Chromium traffic, if you don't get an invalid certificate error then this module is working as it should.

* Check your LSPosed logs, chances are this module couldn't hook the correct method.

## Credits
* [ViRb3](https://github.com/ViRb3/TrustMeAlready) Original project
  
* [jpacg](https://github.com/jpacg/TrustMeAlready) Updated dependencies and Main.java
  
* [D3fau4](https://github.com/D3fau4/TrustMeAlready) Updated dependencies and refactor
