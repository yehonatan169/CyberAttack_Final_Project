Made by:
Amit goffer 
Yehonatan Amosi 

commands:
apktool d {myapp}.apk -> disassemble exported file

apktool b {myapp} -> rebuild disassembled app to apk file output.
the output file will be in {myapp}/dist/{myapp}.afk

to download the signer:
https://github.com/patrickfav/uber-apk-signer -> go to releases -> download uber-apk-signer-1.2.1.jar
or download directly:
https://github.com/patrickfav/uber-apk-signer/releases/download/v1.2.1/uber-apk-signer-1.2.1.jar

to sign:
java -jar uber-apk-signer-1.2.1.jar --apks {myapp}.apk ->
the uber-apk-signer-1.2.1.jar and the output file from the build must be in the same folder.

adb:
1. go to "C:\Program Files (x86)\Android\android-sdk\platform-tools" in your computer, open cmd.

2.
adb -s emulator-5554 pull sdcard/Download/information.txt C:\my_desired_path
-> change C:\my_desired_path to any path in your computer.
make sure the information.txt exists in the emulator first.


enjoy :)
