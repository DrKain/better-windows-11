
<!--   
<details> 
<summary>Text</summary>  

Content

</details>
-->

--------------------------------------------------------------------

<details> 
<summary>Unable to unpin one-drive from file view</summary>  

1. Click on Start, search for command prompter
2. Right-click on and select "Run as Administrator"
3. Paste the following command:  
```
del "%AppData%\Microsoft\Windows\Recent\AutomaticDestinations\f01b4d95cf55d32a.automaticDestinations-ms"
```  

</details>

--------------------------------------------------------------------

<details> 
<summary>Disable "Group By" for all folders</summary>  

1. Download [WinSetView](https://github.com/LesFerch/WinSetView)  
2. Extract, run and hit "Submit"  

</details>

--------------------------------------------------------------------

<details> 
<summary>Always show "more options" in file view</summary>  

1. Click on Start, search for command prompter
2. Right-click on and select "Run as Administrator"
3. Paste the following command:  
```
@echo off
reg.exe add "HKCU\Software\Classes\CLSID\{86ca1aa0-34aa-4e8b-a509-50c905bae2a2}\InprocServer32" /f
EXIT
``` 
4. Open task manager (Ctrl + Alt + Esc)  
5. Open "details" view and close `explorer.exe`  
6. Click "run new task" and type `explorer.exe` 

</details>

--------------------------------------------------------------------






