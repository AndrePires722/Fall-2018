
To fix "no-pie" issue:

Check this link: https://stackoverflow.com/questions/50386787/cabal-install-gcc-failed-in-phase-c-compiler

Navigate to the directory (might be somewhat different depending on version of Haskell, etc): /Library/Frameworks/GHC.framework/Versions/8.4.2-x86_64/usr/lib/ghc-8.4.2/settings

Change permissions of "settings" file to Read&Write

Edit parameter "C compiler supports -no-pie" to "NO"

To fix "--enable-tests" issue:

Navigate to lab1 directory

Install necessary packages (see README)

Type "cabal configure --enable-tests"
