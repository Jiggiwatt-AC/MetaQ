**General Updates**

- Reworked the ChaosHelper UI to better group various functions. Current tabs are:

1. MetaQ – Basic load/start/stop functions
2. Options – Settings that apply specifically to MetaQ
3. Queue – Settings for managing your “meta queue”
4. Controls – Controls that can be used during the execution of any meta
5. MetaOpts -  Options for specific metas

- Modified the ‘Recover’ state in the various metas to launch MetaQ and let it handle rejoining the group, instead of doing so within the meta itself.
- Also made a change to stop error spamming while waiting for the group leader to show up while in the Recover state.
- Modified the provided ReComp nav route to improve reliability. Now uses the Aphus recall.

**New Features**

- Added the ability to define a turn-in trinket (imbued with pyreal for XP/lum bonus) which will automatically be equipped during quest turn-ins. You must also set a ‘default trinket’ which will be assumed to be your normally equipped trinket, and re-equipped after turn-in is complete. 
- Added a check to see if a character is close to max luminance (1.49 million), and skipping the turn-in step if that’s the case. The character will think to themselves so there’s a record of why they skipped the turn-in to help differentiate between this scenario and a problem with the meta
- Added a ‘Log Off on Complete’ option which can be toggled on/off (off by default). This setting is retained and does not reset automatically. If enabled, this will give a 3-minute warning after the completion of the final meta in the queue and then log off all characters.


**Bug Fixes**

- Resolved an issue with Bloodstone Investigation Flagging where the fellowship leader wasn’t using the key to unlock the door.
- Resolved an issue where after clicking ‘Set Group’ an error message would be thrown in spite of everything working properly.
- Resolved an issue where an empty queue was causing a premature triggering of the group shutdown process in MetaQ. This caused a problem where first-time users would have VirindiTank shut down right after starting up.
- Moved the enabling of UB Expressions up to one of the first commands to avoid errors on first launch if the user has not already enabled them.
