
Welcome to the Tactics Ogre - The Knight of Lodis text editing guide. Here I'll 
explain how to edit text in this game.

If you are curious what the text replacements are, change totkol.tbl to 
totkol.txt and open it in notepad.

------

HOW TO EDIT TEXT

  1. BACK UP YOUR ROM! GIVE IT A RELEVANT NAME IF IT HELPS!
  
  2. Download and install ImHex, a hex editor which supports table (*.tbl) 
    files. It is here:
    https://github.com/WerWolv/ImHex
    
    Afterwards, start it up.
    
  3. Load your totkol rom in ImHex.
  
  4. OPTIONAL Go to the View drop-down menu and uncheck everything except the 
    box marked "Hex editor". This simplifies the view.
  
  5. Go to File -> Load custom encoding -> Browse, select totkol.tbl, and click 
    Okay.
    
    You may need to scroll up or down, or minimize then maximize ImHex for text 
    encoding changes to become visible.
    
  6. Navigate to the addresses below and edit the text you find. Be sure that 
    you are in Overwrite mode, not insert mode. And do not hit delete if you 
    mess up, instead arrow back to the error and redo it.
    
    Some bytes make produce two or more text characters. This is likely a 
    simple form of text compression, done to save space.
    
    Let me know on the discord what new discoveries you make.
    
------

TEXT ADDRESSES

  0x623E22 - Start address of character names.
  0x6254B8 - End address of character names.

  0x7843DC - Start address of characters speech.
  0x7BFC28 - End of characters speech.

  0x622A15 - Start address of item names, abilities, cities, emblems.
  0x623611 - End address of them all.

  0x15DA2B - Start address of something? It says TOG, and exists on the save 
            files as well.
  0x7D3A34 - Maybe the end address?

  0x74BACF - Start address of description: classes, items, emblems, etc.
  0x75EBF3 - End address of classes descriptions.

  0x75ECA4 - Start address of status effects and other in battle message boxes.
  0x75F1B6 - End address of status effects.

  0x75F22C - Start address of options text.
  0x75F43F - End address of options text.

  0x75F4B5 - Start address of options sub-text.
  0x75FE28 - End address of options subtext.

  0x75FE63 - Start address of help text and some shop text.
  0x7602C4 - End address of help text and some shop text.

  0x760375 - Start address of shopkeeper text?
  0x7611FA - End address of shopkeeper text.

  0x761270 - Start address of more help text on link cable and quest mode.
  0x761DBB - End address of more help text.

  0x761E6C - Start address of dying quotes and dismissal quotes?
  0x762CB6 - End address of quotes.

  0x762D67 - Start address of mission objectives text.
  0x763750 - End address of mission objectives text.

  0x76378B - Start address of game start questions.
  0x763B3B - End address of game start questions.

  0x763B3B - Start of more help text, maybe some bytes ahead of this position.
  0x7658BB - End of more help text.

  0x7658F6 - Start of even more help text.
  0x765A58 - End of more help text.

  0x765B09 - Start of descriptive help text?
  0x765D1C - End of descriptive help text?

