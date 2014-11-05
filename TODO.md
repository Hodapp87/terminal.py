- serial.write() may block for reasons beyond our control.  For
  example, CDC-ACM devices may do flow control internally and block on
  USB transfers; the CDC-ACM interface does not expose flow control
  settings to the PC, and writes will hang indefinitely even if
  --flow is not used.  Since polling the keyboard is in the write loop,
  this kills us.

- Support some other escape character so ^C can be optionally used.
  Maybe even remove ^C as an option, use ^] exclusively?

- Support reconnection

- See patches from "Guyzmo"
