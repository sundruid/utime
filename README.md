# utime
Simple UTC to local time app for quick reference.

Drop both utime and epoch into your /usr/local/bin directory. No extension needed as interpreter is specified in file.

When scouring logs and various WW linux systems, its easy to get confused as to what TZ the system is in and what that is in UTC. So I made a simple python script that will give me this information quickly. I run it on my Mac laptop as well as systems in the cloud.

Drop the utime.py file into your /usr/local/bin directory and take off the '.py' to make it short to call. Because the interpreter is specified in the #! you don't need to call python or have the .py extension. If your interpreter is somewhere else, or if you get errors, check that you have python env setup right and ensure you have the required mods installed via pip.

Be sure to add the following to your pip env:

pip install pytz tzlocal



Example:

    utime 
    Current Time Information:  
    ==============================. 
    UTC Time     : 2024-08-17 19:40:46 UTC  
    Local Time   : 2024-08-17 12:40:46 PDT  
    Time Zone    : America/Los_Angeles  
    DST Active   : Yes  
    ==============================  



