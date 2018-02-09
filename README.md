# VB-Hash-Updater
This one is mainly useful for people working in Russian banks, but can be used by others as a basis, too.

Central Bank of Russia requires that a set of files need to be validated before running clearing software (and thus operations in it). Recommended software to do that is hashfile.exe by Validata (provided along with their crypto-software). Unfortunately, it's not really convenient to use it to get file hashes for a hundreds of files. This HTA code will solve this issue.

First of all it requires a .cfg/.ini file like the sample provided.

When everything is setup you simply launch the file under designated user (recommended to have admin rights due to access restrictions to some system libraries). Script will be parse the filelists and write 2 sets of hashlists like in the sample provided.

These hashlists can then be used to validate the files later on (check my Hash Checker).

Example of "full" list (contains all the Windows' files recommended for checking by Central Bank) is in the sample provided.
"Short" one can also be found in the sample and it contains files of Central Bank Software, which are required to be validated on each software run.
Of course, each list can be modified according to production needs, but either way if a file is missing in the system it will be silently skipped.
