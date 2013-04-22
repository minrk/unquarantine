# Unquarantine service

This adds a right-click action to unset the quarantine flag,
which causes the "Untrusted developer" dialog when you try to run an installer that hasn't been properly signed.

The command that runs:

    xattr -r -d com.apple.quarantine "FILENAME"

To install, just copy `unquarantine.wflow` to `~/Library/Services/`.