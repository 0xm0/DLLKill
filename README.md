# DLLKill

### Check if your device has any suspicious DLLs

## Usage:
(Please run a cmd prompt as administrator, else it wont work (in the same directory))
```
Usage: DLLKILL.exe
-d [mandatory] Find DLL hijacking in all running processes and services.
-s [optional] Search for DLL references in the binary files of current running processes and services.
-r n [optional] Recursion search for DLL references in found DLL files privous scan.
   n is the number is the level of the recursion
-o [optional] Output path for the results in csv format of
               By ommiting this option, a defulat result file would be created on the desktop of the current user.
               Named after the name of the computer .csv
-X ['/specfic/path'] [high/medium/low] Find and kill all bad DLLs immediatly.
                                       Please note you should only run this if you are comfortable and have no worries if it breaks any applications.
                                       This can damage lots of software or applications it thinks is dangerous/medium or low.
               Please note: This does hunt any bad applications and deletes the root of their cause, ensuring you have not been a DLL Ratted or Hijacked enitely.

```

## RELEASE
https://github.com/0xm0/DLLKill/releases/tag/0.0.1

## NOTE
I can't stress this enough; this application scans windows' C: Drive. don't try to emulate the exe on linux to check for dlls it's not gonna help you.
Also don't run the -X module if you aren't aware of the risks this poses. Will add application and custom DLL Ignorance soon so there is no confusion.

### DISCLAIMER 1/2:
- This application is still in development and some things might not function as they should. it's your responsibility if this has any bad effects on your pc. I'd highly recommend you run a scan rather than letting it take action as some applications such as discord or spotify's DLLs it considers as critical. still working on better and more efficent string extraction and checking modules..etc
### DISCLAIMER 2/2:
- Base application was from DLLSpy (https://github.com/cyberark/DLLSpy) I just added a little sprinkles and some unicorn icecream to it. Use at your own risk, I'm not responsible for what you do with it.
