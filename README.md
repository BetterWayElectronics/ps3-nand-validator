# BwE PS3 NAND Validator

Created/Started by BwE on the 3rd March 2013 (Because I was pressured to).
Greetz/Credit: EussNL, Judges, No0bZiLLa, Rogero, Rebug, deank, 3absiso, AFP, SCE & PS3 Dev Wiki (+ Its Contributers).
This all in one validator/patcher will patch for 3.55 and will output the results of 2799+ validations via HTML.

How?
1 - Place your .bin/s in the same folder as the validator.
2 - Run the validator and press Start.
3 - A console will appear asking you to select your dump (if you have more than one in the folder).
4 - Make your selection and or select if you watch to patch it.
5 - Wait patiently.
6 - Press Enter at the end to launch the output.

Explanation
After selecting your dump and choosing which patch you want it will begin to process the validation. Once it is finished it will give you a brief
count of the results, after this you simply press enter to exit.
The program will then open a html output illustrating everything that has been validated. Scroll through or use the menu at the top and read
each section.

If a validation says 'warning' or 'danger' investigate it yourself manually using a hex editor, or contact somebody knowledgeable. Only corruption
messages will show you the exact offset to look at, everything else won't so this is where you have to read/learn about it on the psdevwiki.
Some validations will tell you that you need to patch it (e.g. ROS0 / ROS1 errors or warnings), if this is the case then do so (don't forget to rename
the patched dump) and re-validate the patched dump (you can move the original unpatched dump to make sure it is checking the patched one).
If your dump has any 'danger' messages in the per console sections (find them in the menu) then there is a good chance its completely ruined and
unfixable. Also, if your dump has a large amount of 'danger' messages then there is a serious issue - bad wiring can be discovered if you have any
repetition in the dump.

Areas Of Validation
1. Lv0ldr/Bootldr
2. Lv0ldr/Bootldr Corrupt Sequences
3. Lv0ldr/Bootldr Statistics/Entropy
4. First Region Header
5. Flash Format
6. Flash Region
7. Asecure_Loader/Metldr
8. Asecure_Loader/Metldr Corrupt Sequences
9. Asecure_Loader/Metldr Encrypted Statistics/Entropy
10. EID
11. EID0
12. EID1
13. EID2
14. EID3
15. EID4
16. EID5
17. IDPS
18. CISD
19. CISD0
20. CISD1
21. CISD2
22. CCSD
23. CCSD0
24. TRVK_PRG0
25. TRVK_PRG1
26. TRVK_PKG0
27. TRVK_PKG1
28. ROS0
29. ROS1
30. ROS0/1 AuthID's/MD5's
31. CoreOS MD5's
32. CVTRM/VTRM0
33. VTRM 1
34. CELL_EXT_OS_AREA
35. OtherOS
36. Lv0ldr/Bootldr
37. Lv0ldr/Bootldr Corrupt Sequences
38. Lv0ldr/Bootldr Statistics/Entropy
39. Minimum Version
40. File Digest Keys
41. PerConsole Nonce
42. Corrupt Sequences
43. Repetition
44. Authenticiation IDs

Changelog
1.02 - 09/06/2013 : bugfix for patcher (did not fix enough) + added some more MD5's (CFW)
1.01 - 28/05/2013 : bugfix for patcher (mistake from using old nor code)
1.00 - 27/05/2013 : first proper/public release (because I am lazy there will be no loader!)
