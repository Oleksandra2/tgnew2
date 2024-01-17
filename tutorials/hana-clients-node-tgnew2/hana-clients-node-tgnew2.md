---
title: Connect Using the SAP HANA Node.js Interface tgnew2
description: Create and debug a Node.js application that connects to SAP HANA using the SAP HANA client.
auto_validation: true

>```    

> ![debug output](debug-flag.png)

> The value of the environment variable DEBUG can be seen and removed with the commands below.

>```Shell (Microsoft Windows)
>set DEBUG
>set DEBUG=
>set DEBUG
>```  

>```Shell (Linux or Mac)
>printenv | grep DEBUG
>unset DEBUG
>printenv | grep DEBUG
>```


[DONE]
[ACCORDION-END]

[ACCORDION-BEGIN [Step 4: ](Debug the application)]

Visual Studio Code can run and debug a Node.js application.  It is a lightweight but powerful source code editor which is available on Windows, macOS and Linux.

1. If required, download [Visual Studio Code.](https://code.visualstudio.com/Download).

2. In Visual Studio Code, choose **File | Add Folder to Workspace** and then add the `HANAClientsTutorial` folder.

    ![Workspace](workspace.png)

3. Open the file `nodeQuery.js`.

4. Place a breakpoint inside the `connection.exec` callback.  Select **Run | Start Debugging | Node.js**.  

    Notice that the debug view becomes active.  

    Notice that the program stops running at the breakpoint that was set. Observe the variable values in the leftmost pane.  Step through code.

    ![VS Code Debugging](debugging.png)


Congratulations! You have created and debugged a Node.js application that connects to and queries an SAP HANA database.

[VALIDATE_1]
[ACCORDION-END]


---
