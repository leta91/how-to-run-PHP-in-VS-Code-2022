# How to run 🐘PHP on Visual Studio Code 2022 and how to fix some related bugs 🐛:

You need 3 things to run PHP on your local machine:
1. PHP
2. a web server
3. a database

The software that offers all 3 and that I found to be the best choice is **WAMP** 🥇

Open WAMP 
    🔽
go to *C:\wamp64\www\newfolder*
    🔽
:file_folder: *newfolder* is the folder's name I created within the *www* folder (it's important to keep all PHP files inside the *www* folder in order for them to be opened)
    🔽
select *newfolder*'s path and type `cmd` and click *Enter*
    🔽
within Command Prompt type `code .` 
this will set VS Code as the default text editor to open this specific folder with a PHP file
    🔽
to access this file, type in the browser *localhost* that will show the homepage of all the folders within the *www* folder of WAMP, select the one that says *newfolder* ▶️ *indexb.php* 
*indexb.php* will show the output of the PHP code that in this case corresponds to the word **Greetings**

About bugs 🐛 here are the solutions to the error messages that you might get on WAMP
when you left-click on your 🖱️ on the small WAMP icon that is located on the right side of the taskbar 

- #### default text editor does not exist
within the folder *wamp64* open with normal notepad the file named *wampmanager.conf* and swap the previous text editor .exe to VS Code. Type on your computer the **Windows key + R** and type *%appdata%\..\Local\Programs\Microsoft VS Code*

Add right after `editor =` in *wampmanager.conf* the path to VS Code that needs to have a similar syntax to the following `C:\..\..\AppData\Local\Programs\Microsoft VS Code\Code.exe"`

- #### default log viewer does not exist 
copy and paste the same .exe path after it says `logviewer =`

- #### warning C:\wamp64 or PHP in PATH
in Windows search bar type *environment variables* and click on *edit* when you see on *Path* `C:\wamp64\bin\php\php7.4.26` or something similar delete it and click ok. then right-click on 🖱️ and select *exit* on WAMP small icon. When you will re-open WAMP all 3 bugs will be fixed ✅



    
