# Hello World SSMS Extension
This is a simple SQL Server Management Studio 17 (SSMS) extension used to demonstrate how to get started with creating your own.

## QuickStart
Clone the repository to your computer and open it in Visual Studio.

**Important: Run Visual Studio as an administrator.**

_Note: This project was created in Visual Studio 2015. If you try to open it in Visual Studio 2017 it will probably show the one-way upgrade window when loading the solution. Just hit OK. The project will work just fine._

Build the solution and then open the project’s properties window by right-clicking the project in the Solution Explorer and selecting Properties. In the Debug tab put the location to your SSMS executable in the "Start external program" field. By default it should be:
```
C:\Program Files (x86)\Microsoft SQL Server\140\Tools\Binn\ManagementStudio\Ssms.exe
```
_Note: Optionally you can add the /log argument in the "Command line arguments" field to make SSMS log its activity which can help with troubleshooting down the line. The log file can be found at:_
```
C:\Users\Username\AppData\Roaming\Microsoft\AppEnv\14.0
```
Now, just hit Start in Visual Studio and you should see SQL Server Management Studio starting up.
On the first run, SSMS will complain that something is wrong with the extension and ask you if it should continue to show the error message.

**Important: Select No. If you don’t select No you won’t be able to load the extension.**

After this, just close SSMS, go back to Visual Studio and hit Start again. This time SSMS should start without any errors. After starting, close the Connect to Server window and open the Tools menu in the menu bar. You should see the extension’s command (Invoke HelloWorldCommand) listed as the first item indicating that it loaded correctly. 
