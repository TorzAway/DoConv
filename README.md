-------------------------------------------------------------------
This utility will automate key features on Project Lazarus (EverQuest EMU) server:
-------------------------------------------------------------------
1) Automate the conversion of all your group's AA [Alternaet Advancement] to DC [Diamond Coin]
2) Automate the conversion of all your group's DC [Diamond Coin] to AA [Alternaet Advancement]
3) Collect all your group's [Diamond Coin] (issuesd from one character who MUST be in group).
4) Collect all your group's coin [Platinum | Gold | Silver | Copper] (issuesd from one character who MUST be in group).
-------------------------------------------------------------------
Run this in Plane of Knowledge of Temple of Marr:
-------------------------------------------------------------------
Setup (4) separate EQ Social Hotkeys, one for each of the following functions:
(We will assume your using native E3BC in the E3 mono package for group communiucation)
-------------------------------------------------------------------
1) Convert Group AA to DC (GROUP COMMAND): 
      /e3bcga /macro DoConv ALL-AA
2) Convert Group DC to AA (GROUP COMMAND): 
      /e3bcga /macro DoConv ALL-DC
3) Collect ALL the group's [Diamond Coin] (SINGLE COMMAND): 
      /macro DoConv GIMME
4) Collect ALL the group's coin [Platinum | Gold | Silver | Copper] (SINGLE COMMAND): 
      /macro DoConv STICKEMUP
-------------------------------------------------------------------
NOTE: 
NEVER ISSUE THE COLLECTION COMMANDS AS GROUP COMMANDS !
-------------------------------------------------------------------
NOTE: 
The macro relies on having MQ2AutoAccept plugin setup for free trade with your own group members.
-------------------------------------------------------------------
NOTE: 
If your trying to setup the buttons for GIMME DC and GIMME $$$ in boxhud
You need to issue the command to the toon via boxhud's toons name variable ... the button example would be:
-------------------------------------------------------------------
Conv AA = /e3bcga /macro DoConv ALL-AA

Conv DC = /e3bcga /macro DoConv ALL-DC

Gimme $$$ = /dex #botName# /macro DoConv STICKEMUP

Gimme DC = /dex #botName# /macro DoConv GIMME 

-------------------------------------------------------------------
