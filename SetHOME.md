**For Windows**  
If your "HOME" environment variable is not set (or you don't know what this is):  
Open command prompt (Open Start Menu then type `cmd` and press [Enter])  
Type the following line into the command prompt window exactly as shown:  
`setx HOME "%USERPROFILE%"`  

Press [Enter], you should see SUCCESS: Specified value was saved.  
Quit command prompt by typing exit then pressing [Enter]  

`REG delete HKCU\Environment /F /V HOME` 

You can set OneDrive folder as your home directory in gitbash:  
Open .bash_profile and add:
`export HOME="HOME=/c/Users/<yourUsername>/OneDrive`  
New gitbash window will open in the same folder as before (in home director set by Windows ("%USERPROFILE%")), but when you type `cd` it will take you to HOME set in gitbash. 
