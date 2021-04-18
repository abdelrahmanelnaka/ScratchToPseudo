# ScratchToPseudo
The aim of this project is to translate a JSON file produced from Scratch Programming Language to a pseudo code equivalent in the English language. The project is implemented using the Python programming language, and it is implemented natively with importing any libraries other than "JSON".

The code is divided into e main blocks:
1. Input JSON
2. Logic
4. Output Text

The logic component is mainly based on recursive calls of multiple helper functions within a main function "Run Translation", here are the used functions and their briefs:
-Run Translation
  -Takes a list of block IDs and initially an empty String.
  -Returns output pseudo code
  -recursively calls decodeBlock(BlockId, ListOfBlockNames)
-decodeBlock(blockId, blockNames):
  -Takes a block ID and a list of block IDS
  -Returns input block pseudo code
  -calls specific block methods "Motion, Event, Sensing, Control, Looks" 
-controlBlock(blockObject,opcodeOperation, blockNames):
  -Handles control blocks, recursively calls decodeBlock()
-eventBlock(blockObject,opcodeOperation, blockNames):
  -Handles event blocks, recursively calls decodeBlock()
-looksBlock(blockObject,opcodeOperation, blockNames):
  -Handles looks blocks, recursively calls decodeBlock()
-moveBlock(blockObject,opcodeOperation, blockNames):
  -Handles motion blocks, recursively calls decodeBlock()
-operatorBlock(blockObject, opcodeOperation, blockNames):
  -Handles operators blocks, recursively calls decodeBlock()
-sensingBlock(blockObject, opcodeOperation, blockNames):
  -Handles sensing blocks, recursively calls decodeBlock()
  
You will be able to find the input json file labelled:
-Project1.json

And the output text file labelled:
-Output.txt


