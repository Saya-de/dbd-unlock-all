# Dead-by-Daylight-Unlocking-Utils

# DISCLAIMER
The files and instructions presented are for educational purposes only!! I assume no liability for your use of these. Likewise, I assume no liability for any resulting bans or other problems! Always compare the current GameVersion and the current version of the files before injecting/using them!

!!Before following any of these steps download and unpack the repository.!!
Currently the files are only for the Steam-Version of the Game!

## Table of Contents  
[SSL-Bypass](#SSL-Bypass)  
[Fiddler Classic](#Fiddler-Classic)  
[MarketFile Setup](#marketfile-setup-for-every-character-and-every-cosmetic)  
[FullProfile Setup](#fullprofile-setup-for-prestige-3-all-items-and-all-perks)
<a name="headers"/>


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

### MarketFile Setup (For every Character and every Cosmetic)
Go to "AutoResponder"  
Check "Enable rules" and "Unmatched requests passthrough"  
Click on "Add Rule"  
Request URL (first line): api/v1/inventories  
Local file to return (second line): Click on the arrow and choose "Find a file..." at the Bottom  
                                    Choose the Market.json file  
                                    Click on Save  
           
Start the Game (Fiddler needs to run in the background, so you have to open it every time you want to play dbd with the market file)

### FullProfile Setup (For Prestige 3, all Items and all Perks)  
(Setup the MarketFile first!)  
(You only need to do all of this once!)
Go to "FiddlerScript"  
Select "Go to: OnBeforeRequest"  
Copy and paste the code snippet from my FiddlerScript.txt under a closing bracket:  
![alt text](https://i.imgur.com/aE6ijKO.png)  
Click on Save Script  

Run the game with Fiddler open and go to the home Screen  
Go to Fiddler, find and click the URL "/api/v1/inventories" in the list on the left  
Select the Cookies Tab  
Copy the bhvrSession after the "="  
Save it to a file or something  

Run the Simple Injector.exe  
Paste the bhvrSession Cookie  
Click on Submit  
Click on Inject Profile and wait for the sound  
Click on Inject Profile again and wait for the sound  
Close the Injector

Restart the Game (Fiddler needs to stay open)


# Proof Images (Market and Fullprofile)  

Survivor:  
![alt text](https://i.imgur.com/SlvUAuj.png)  

Killer:  
![alt text](https://i.imgur.com/E8SBvgI.png)  



