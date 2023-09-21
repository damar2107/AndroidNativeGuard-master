# What is it?
Android Native Guard is a proof of concepts on how to detect various threat that might harm your application's integrity.

# How secure is it?
Android Native Guard used what's called `Secure API` and low-level function call through inline `syscall` to prevent any bypass that could potentially break the security system.
Android Native Guard used various open-source projects to implement a true-secure android application system.


# Modules
- Debugger Detection
- Frida Detection
- Riru & Zygisk Detection
- Root Detection
- Memory Access & Dump Detection
- Library Patch & Hook Detection

# TODO
- Better documentation (codes & README)
- App Tamper Detection (signature, checksum, etc)
- Magisk-Hide Detection Module (e.g. Shamiko)
- Blacklist for AntiLibPatch module

# Notes
- Don't forget to add `android:extractNativeLibs="true"` to your `AndroidManifest.xml` so that module _AntiLibPatch_ can work properly.

- to use string obfuscator, use AY_OBFUSCATE("string");
  example: const char* obfuscatedUrl = AY_OBFUSCATE("https://myapiurl.net/auth/login");

# Credits
https://github.com/darvincisec/AntiDebugandMemoryDump

https://github.com/darvincisec/DetectFrida

https://github.com/aimardcr/NativeDetector
