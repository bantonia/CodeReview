!PollIdle
I've added a few lines to test CathLibCPP to main introducing vector components, they do nothing for the program themselves. Removing or commenting out the the lines between the //********** will produce a runnable application.
Link object files with the following if not using anything from CathLibCPP:
o.ToolboxC++Lib (from MyC++Lib)
o.RiscOSC++Lib (from MyC++Lib)
o.CommonC++Lib (from MyC++Lib)
o.wimplib (from the toolbox library)
o.c++lib (from c++lib)
o.stubs (from CLib)
Add the following if the extra lines are present therefore requiring CathLibCPP and OSLib:
o.CathLibCPP (from CathLib)
o.stubs (from CathLib)
o.OSLib32 (from OSLib)

The test directory has a source from one of the test programs for CathLibCPP, this compiles and links fine.
Link with:
o.CathLibCPP (from CathLib)
o.stubs (from CathLib)
o.OSLib32 (from OSLib)
o.c++lib (from c++lib)
o.stubs (from CLib)
