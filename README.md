# unfinished forensics tools

just dumping some anti-forensics and privacy tools i'm working on. executables only right now, no source code. everything is super early stage so expect bugs, crashes, and half-baked features.

**ram dump analyzer notes:**
analyzes kernel or ram dumps. ram dumps are recommended since they have way more chance to detect stuff. the format is filename.txt:::keyword1;keyword2;keyword3:::depth1:::depth2:::depth3:::depth4:!:regex
the regex must be at the end only of each file. and itll only run if the keyword previously has less than 5mb results as regex on bigger files will be deadly slow.
example would be :
powershellfileless.txt:::IEX:::https

have fun detecting fileless :3

also keywords can be encrypted so that cheaters can't patch your detection
if someone finds bugs, has suggestions, or wants to contribute, just open an issue here on github.
