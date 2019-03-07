# Hearthstone Chat
Instantly chat with Hearthstone opponents that also have this application. *Only one file needs to be downloaded, no installation is required, no registration is required, no setup is required, no chat logs are stored, automatic updates.*

*On Windows Only.*

**Getting Started**

* Download the Hearthstone Chat application (only one .hta file). The icon is optional as your application's local shortcut icon.
* Open Hearthstone and the Hearthstone Chat application, in any order.
* The application will configure a Hearthstone log file if one doesn't already exist.
* Whenever you enter a new game, the application will automatically place you in a unique chat room with your opponent. If you don't see your opponent also enter the chat room, that means they don't have this application running.

**How It Works**

The application continously scans the Power.log file generated by Hearthstone. From this information, it finds you and your opponent's BattleTags and creates a unique chatID based on them. It sends this chatID to the web handler that puts you in a chatroom where only messages sent by your application with that matching chatID can be seen.

**Interface**

The window is resizable.

* Header
  * The header contains the name of your current opponent. Clicking on it copies their BattleTag to your clipboard.
  * Next to your opponent's name is a red 'ban' icon. Clicking the icon will temporarily block your opponent's messages (for only this session). When you click the icon, your opponent's status icon and name will become red. You'll also see a system message in the chat room. Clicking on the now white 'ban' icon again unblocks your opponent's messages and restores their status to normal.
  * Whenever you get a new message, a sound will play by default. If you don't want this sound, click on the 'speaker' icon to toggle this sound on/off. *If you don't see a sound icon, it means the application was unable to locate your log.config directory (see **Troubleshooting** below).*

* Chat Room
  * Your messages are gold and remain in the chat room for 5 minutes.
  * Your opponent's message are white and remain in the chat room for 5 minutes.
  * System messages are in blue (only seen by you) and only stays in the chat room for 30 seconds.

![Interface](https://i.imgur.com/yVrs8g9.png)

**Troubleshooting**

"The game started but my opponent didn't enter chat."
* This just means your opponent is not running the application.

"My chat window is blank, even when I'm playing games."

This stems from two issues:
* The application couldn't find the location of your hearthstone log.config file normally in your %localappdata%\Blizzard\Hearthstone directory. If your directory is different than above, please send me full path to add to the white list.
* The application couldn't find the location of your hearthstone Power.log file normally in %PROGRAM FILES%\Hearthstone\Logs or %PROGRAM FILES (x86)%\Hearthstone\Logs. If your directory is different than above, please send me full path to add to the white list.

**Author**

Gregg Jewell | Gatekeeper#1310 (NA Server)
