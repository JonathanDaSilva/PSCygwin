How to use it
-------------

For using this you should:
  * Import the module
  * Having CygWin into the default directory "C:\cygwin\"
  * Creating a function for every command that you want to export
```powershell
function ssh { Invoke-Cygwin "ssh" }
```
  * Using like the command was part of Powershell


What the function will execute the command that you have typed into your current directory with the parameters that you haved pass.

For exemple:
```bash
ssh root@127.0.0.1
```
will work
