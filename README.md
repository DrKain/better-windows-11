*I recently bought a laptop that runs Windows 11, it was the only option at the time or I would have stuck with 10. I had a feeling it would be bad, but it was much worse than I expected. If Windows 7 was still supported by modern apps I'd still be using that.*  

*This readme/repo is a personal collection of tools and guides I've used to optimize and un-fuck Windows 11. Includes privacy tweaks and other QOL improvements.*

<!--   
<details> 
<summary>Text</summary><br>    

Content

</details>
-->

--------------------------------------------------------------------

<details> 
<summary>Disable telemetry/tracking/spyware/cortana ect</summary><br>  
  
1. Download [ShutUp10++](https://www.oo-software.com/en/shutup10)  
2. Run the file  
3. Click "Actions" -> "Apply only recommended settings"  
4. Wait 5 seconds then close the app

</details>

--------------------------------------------------------------------

<details> 
<summary>Unable to unpin one-drive from file view</summary><br>  

1. Click on Start, search for command prompt  
2. Right-click and select "Run as Administrator"
3. Paste the following command:  
```
del "%AppData%\Microsoft\Windows\Recent\AutomaticDestinations\f01b4d95cf55d32a.automaticDestinations-ms"
```  

</details>

--------------------------------------------------------------------

<details> 
<summary>Disable "Group By" for all folders</summary><br>  

1. Download [WinSetView](https://github.com/LesFerch/WinSetView)  
2. Extract, run and hit "Submit"  

</details>

--------------------------------------------------------------------

<details> 
<summary>Always show "more options" in file view</summary><br>  

1. Click on Start, search for command prompter
2. Right-click on and select "Run as Administrator"
3. Paste the following command:  
```
reg.exe add "HKCU\Software\Classes\CLSID\{86ca1aa0-34aa-4e8b-a509-50c905bae2a2}\InprocServer32" /f
``` 
4. Open task manager (Ctrl + Alt + Esc)  
5. Open "details" view and close `explorer.exe`  
6. Click "run new task" and type `explorer.exe` 
   
<details> 
<summary>If you want to undo this change:</summary><br>    

```
reg.exe delete "HKCU\Software\Classes\CLSID\{86ca1aa0-34aa-4e8b-a509-50c905bae2a2}" /f
```

</details>
</details>

--------------------------------------------------------------------

<details> 
<summary>Disable snap layouts on hover</summary><br>   

Some people find this feature useful, some may not. I found the popups to be annoying so here's how to disable it:  

![snap-windows.png](images/snap-windows.png)  

1. Open start menu
2. Search for `multitasking settings`  
3. Expand "Snap Windows" to show all options  
4. Uncheck "Show snap layouts when I hover over a window's maximize button"

Optional: You may also want to uncheck "Show snap layouts when I drag a window to the top of the screen"


</details>

--------------------------------------------------------------------



