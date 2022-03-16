# Dead-by-Daylight-Unlocking-Utils
# DISCLAIMER
The files and instructions presented are for educational purposes only!! I assume no liability for your use of these. Likewise, I assume no liability for any resulting bans or other problems! Always compare the current GameVersion and the current version of the files before injecting/using them!

!!Before following any of these steps download and unpack the repository.!!
Currently the files are only for the Steam-Version of the Game!


## SSL-Bypass
You need it for everything  
Works for version 5.6.0+

WIN+R  
Enter "appdata"  
Go to "AppData\Local\DeadByDaylight\Saved\Config\WindowsNoEditor"  
Replace Engine.ini


## Fiddler Classic
https://www.telerik.com/download/fiddler

### Basic Setup
Download, Run Setup and Install  
Open Fiddler Classic  
On the top go to Tools -> Options and the Tab HTTPS  
Check the Boxes "Capture..." and "Decrypt..."  
Click OK  
Restart Fiddler and check if the boxes are still checked

### MarketFile Setup
(For every Character and every Cosmetic)  
Go to "AutoResponder"  
Check "Enable rules" and "Unmatched requests passthrough"  
Click on "Add Rule"  
Request URL (first line): api/v1/inventories  
Local file to return (second line): Click on the arrow and choose "Find a file..." at the Bottom  
                                    Choose the Market.json file  
                                    Click on Save  
           
Start the Game (Fiddler needs to run in the background, so you have to open it every time you want to play dbd with the market file)

### FullProfile Setup
(Setup the MarketFile first!)
(For Prestige 3, all Items and all Perks)  
Go to "FiddlerScript"  
Select "Go to: OnBeforeRequest"  
Copy and paste the code snippet from my FiddlerScript.txt under a closing bracket:  
![alt text](https://i.imgur.com/aE6ijKO.png)  

Download the FullProfile Injector (you need to make an mpgh account)  
https://www.mpgh.net/forum/showthread.php?t=1510097




