# CBT630
Converted to GitHub via [cbt2git](https://github.com/wizardofzos/cbt2git)

This is still a work in progress. 
Due to amazing work by Alison Zhang and Jake Choi repos are no longer deleted.

```
//***FILE 630 is from Bob Glover, and contains a REXX exec which    *   FILE 630
//*           uses DFDSS in the foreground to COPY or MOVE          *   FILE 630
//*           datasets from one disk pack to another.  All that     *   FILE 630
//*           is required is the REXX (called MC - "move copy")     *   FILE 630
//*           and one panel, which formats the input and controls   *   FILE 630
//*           the operation of the EXEC.                            *   FILE 630
//*                                                                 *   FILE 630
//*           There is one caveat, to get this thing to work.       *   FILE 630
//*           You have to APF authorize a TSO CALL to the           *   FILE 630
//*           ADRDSSU program.  That is accomplished either by      *   FILE 630
//*           adding the name ADRDSSU to the AUTHPGM list in the    *   FILE 630
//*           IKJTSOxx member of PARMLIB, or you can do it          *   FILE 630
//*           "personally" for yourself, if you have permission     *   FILE 630
//*           to make your own LOGON PROC with an authorized        *   FILE 630
//*           STEPLIB library.  See Files 185 and 186 of the CBT    *   FILE 630
//*           Tape collection about how to implement that.  You     *   FILE 630
//*           have to add the name ADRDSSU to the IKJEFTE8          *   FILE 630
//*           module of the IKJTABLS load module, and copy          *   FILE 630
//*           module IKJTABLS into your authorized STEPLIB          *   FILE 630
//*           library.  Then, the IKJTABLS entries will             *   FILE 630
//*           completely override the IKJTSOxx PARMLIB entries      *   FILE 630
//*           for your TSO session.  BUT the conditions for that    *   FILE 630
//*           are, that the library containing IKJTABLS must be     *   FILE 630
//*           running under your TSO session as an authorized       *   FILE 630
//*           library and a STEPLIB.  And the override of the       *   FILE 630
//*           IKJTSOxx PARMLIB member is complete.  That is, you    *   FILE 630
//*           lose authorization of all the IKJTSOxx names, not     *   FILE 630
//*           copied into your IKJTABLS module.  So be careful      *   FILE 630
//*           implementing this for yourself or your group.         *   FILE 630
//*                                                                 *   FILE 630
//*           email:  Bob.Glover@fnf.com                            *   FILE 630
//*                                                                 *   FILE 630
```
