# unfinished forensics tools

just dumping some anti-forensics and privacy tools i'm working on. executables only right now, no source code. everything is super early stage so expect bugs, crashes, and half-baked features.

**ram dump analyzer notes:**
it's a fast memory scanner to hunt down obfuscated commands and malware strings, but the built-in detections are still a heavy WIP. you can build your own custom keyword rules using a layered format (`output.txt:::primary_keys:::depth_keys:::regex`). just remember to use a semicolon (`;`) to separate multiple words inside those keys (like `iex;invoke-webrequest`). the tool encrypts and loads these directly. if someone wants to contribute better keyword lists, you can either make them inside the program and share the encrypted blob, or just open an issue.

if someone finds bugs, has suggestions, or wants to contribute, just open an issue here on github.
