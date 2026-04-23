!PollIdle<br/>
I've added a few lines to test CathLibCPP to main introducing vector components, they do nothing for the program themselves. Removing or commenting out the the lines between the //********** pairs will produce a runnable application.<br/>
These extra lines have been taken from the test program below but removing the lines concerning output.<br/>
Link object files with the following if not using anything from CathLibCPP:<br/>
o.ToolboxC++Lib (from MyC++Lib)<br/>
o.RiscOSC++Lib (from MyC++Lib)<br/>
o.CommonC++Lib (from MyC++Lib)<br/>
o.wimplib (from the toolbox library)<br/>
o.c++lib (from c++lib)<br/>
o.stubs (from CLib)<br/>
Add the following if the extra lines are present therefore requiring CathLibCPP and OSLib:<br/>
o.CathLibCPP (from CathLib)<br/>
o.stubs (from CathLib)<br/>
o.OSLib32 (from OSLib)<br/>
<br/>
The test directory has a source from one of the test programs for CathLibCPP, this compiles and links fine.<br/>
Link with:<br/>
o.CathLibCPP (from CathLib)<br/>
o.stubs (from CathLib)<br/>
o.OSLib32 (from OSLib)<br/>
o.c++lib (from c++lib)<br/>
o.stubs (from CLib)<br/>
