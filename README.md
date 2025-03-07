# <img src="https://i.imgur.com/cGllffv.png" width="75" height="75" /> CatalinaForensicsTool 
A GUI frontend for AppleScript (shell, etc) based forensic artifact retreival. 

See Wiki for detailed information. 

But what its really about is providing a building block so, so anyone can add in stuff, make it their own. Its not exactly simple to get Cocoa, and AppleScript talking to terminal, and using their own binaries. This app lays things out pretty understandably. Just be aware of how things are delegated and assigned, and you shouldnt have a problem adding on. The hardest part is getting familiar with Xcode. 

DOES NOT USE SANDBOX. 

Relies on AppleScriptObjC for operation. 

Requires various permissions.
* Full Disk Access
* System Events.app

If you are not prepared to debug any minor quirks / build failures from things in progress, stick with the releases tab. Those have actually been tested and are bookmarked for functionality. They're not actually "releases" as in full suites. 

This is not indended to be a standard consumer / production app, as its operation violates many core traits of normal macOS app operation. It is not malicious in any way, just not something the average Jill/Joe should be messing around with in general. 

#### Forensic Disclaimer:
This is a ongoing project, and should not be considered a completed product.  
<br><br>

## Future Functionality:
* There might be more stuff available in the protected volumes that can be mounted with SIP disabled. 
* See Issues


### Known Quirk(s)
* Dont open more than one instance. Doing so sometimes crashes things.  
* See Issues


## Two ways to run:
1. Compile it yourself! (BETTER, SAFER WAY. You should check what a program like this is doing)
2. Download the release .app and run the following command on the file:
xattr -cr CatalinaExporter.app
3. You must give CatalinaExporter.app full disk access for some functions to work. 

## Screenshot of Current (Release) State
<img src="https://i.imgur.com/vWfg3XB.png" width="500" />

## Credits:
* David Cowen's FSEventParser used for FSEvent Exporting: https://github.com/dlcowen/FSEventsParser <br>

