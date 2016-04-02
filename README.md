How to use it
-------------

For using this you should:
  * Import the module
  * Having CygWin into the default directory "C:\cygwin\"
  * Creating a function for every command that you want to export to powershell
```powershell
function ssh { Invoke-Cygwin "ssh" $args }
```
  * Using like the command was part of Powershell


The function will execute the command that you have typed (first parameters, in my case "ssh") into your current directory with the parameters that you haved pass in second arguments (in the example $args, is the argument of the function).

This example above allow you to do that:
```bash
ssh root@127.0.0.1
```

This is not realy impressive but you can totaly execute some none available windows command like ansible.
```bash
ansible help
```

That will work if ansible is install into cygwin
