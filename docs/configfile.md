This is the default ConfigFile:

```YAML
Prefix: '&9SuperAuth»&r '
Language: 'en_US'
DialogCloseWord: 'close'
TranslationAutoDownload: true
Updater:
  Enabled: true
SQL:
  Enabled: false
AntiBot:
  Captcha: 0.9
  MaxAuthTime: 30
  PreventSameUserOnline: false
AntiThief:
  PreventLoginFromOtherIP: true
AutoLoginPremium: true
AfterAuth:
- 'msg:&6Welcome &5{Player}&7!'
- 'console:say Hello {DisplayName}!'
- 'player:kit noob'
- 'server:hub'
```

## Explanation
Here you can see an explanation of every setting of the System.cfg file.
<br>
### General Settings:<br>
• Prefix: This is the prefix of the plugin, used in some messages
• Language: This is the language of the plugin, you can contribute and see a list of available languages [Here](https://github.com/TheProgramSrc/PluginsResources/tree/master/superauth)<br>
• DialogCloseWord: The word to close a dialog (Won't work on register, login or captcha dialog.)<br>
• TranslationAutoDownload: If it's enabled automatically the plugin will fetch translations and download every time that it's possible.<br>
• Updater: This will notify you if there is a new update.<br>
• SQL: `STILL IN WORK`<br>
<br>
### AntiBot:<br>
• Captcha: Set it to `0` or `0.0` to disable the Captcha. This is the chance of show the captcha dialog, must be between 0.1 and 1.0<br>
• MaxAuthTime: If a user it's logging or registering more than the specified time will be kicked with a message. Set it to `0` to disable<br>
• AntiThief-PreventLoginFromOtherIP: When you enter for the first time your IP it's logged, if you enter again from another IP you'll be kicked from the server<br>
• AutoLoginPremium: If it's enabled Premium users will be auto-logged in<br>
• AfterAuth: A list of actions that Will be executed after the login-register form<br>
<br>
### AfterAuth Actions:<br>
• msg: Message with colors and PlaceholderAPI Support<br>
• console: Command that will be executed by the console<br>
• player: Command that will be executed by the player<br>
• server: Send a player to another server (Only for Networks, or servers linked to BungeeCord)<br>