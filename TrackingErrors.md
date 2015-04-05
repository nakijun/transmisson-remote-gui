Often it is not possible to find and fix a error, if a user just reports: "I have the error X, when I try to do Y".

It is needed to provide more details, like call stack information with line numbers.


To do that:
  * Download and install FPC and Lazarus, download the transgui source code. See the [Building](Building.md) wiki page to learn how to build the program.
  * Build the program using the following command: `make clean debug`
  * Run transgui and reproduce the error.
  * You should see a call stack information in the error message box. The call stack information has been copied to the clipboard.
  * Paste this call stack information to your bug report.