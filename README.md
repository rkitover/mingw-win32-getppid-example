The code for retrieving the parent process id on Windows using the Tool Help
library is based on the example from:

https://stackoverflow.com/a/558251/262458

, and the code for the WMI query to retrieve the commandline is from:

https://stackoverflow.com/a/20082113/262458

. Just run `make` in one of the MSYS2 native build shells or an MSYS shell.
Should also work on Cygwin with the relevant packages installed.

For MSVC run `make CC=cl`.

The resulting executables are `show-parent.exe` and `show-process.exe`, which
take an optional argument for the pid to look up, otherwise they will use their
own pid.
