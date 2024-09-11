# utime & epoch
Simple UTC to local time app for quick reference.

Drop both `utime` and `epoch` into your `/usr/local/bin` directory. No extension is needed as the interpreter is specified in the file.

When scouring logs across various Linux systems, it’s easy to get confused by the different time zones and how they relate to UTC. So, I made a couple of simple scripts (`utime` and `epoch`) to quickly convert and display the time information. I run them on my Mac laptop as well as systems in the cloud.

For `utime`, drop the `utime.py` file into your `/usr/local/bin` directory and remove the `.py` extension for easier execution. Because the interpreter is specified in the `#!` shebang, you don’t need to call Python or keep the `.py` extension. If your interpreter is located elsewhere, or if you encounter errors, make sure you have your Python environment set up correctly and that you’ve installed the necessary modules via pip.

Be sure to install the following via pip:

pip install pytz tzlocal

For `epoch`, you can use it to convert Unix epoch timestamps to local time or to get the current time in epoch format. Simply drop the `epoch` script into your `/usr/local/bin` directory, just like `utime`.

## Example Usage:

### utime

utime 

Output:

  Current Time Information:  
  ==============================  
  UTC Time     : 2024-08-17 19:40:46 UTC  
  Local Time   : 2024-08-17 12:40:46 PDT  
  Time Zone    : America/Los_Angeles  
  DST Active   : Yes  
  ==============================

### epoch

epoch

Output:
1692280846

This prints the current time in Unix epoch format.

epoch @1692280846

Output:
2024-08-17 12:40:46

This converts a given Unix epoch timestamp into a local time format.

By having these two tools (`utime` for detailed UTC to local time info and `epoch` for Unix timestamp conversions), you can quickly reference or convert times when working across different systems and time zones.
