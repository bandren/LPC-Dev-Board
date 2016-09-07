#Welcome
---

This is a repository for a custom LPC1769 development board.

#Post assembly setup

###USB - TTL UART

The FT230XS-U (usb-uart) chip has an internal MPT memory which needs to be programmed with different values than its default. The table below shows the required values and the default values of the various parameters. 

| Paramter | Required  | Default |
|:---------|:----------|:--------|
| CBUS0  | RXLED# | TXDEN |
| CBUS1  | TXLED# | RXLED# |
| CBUS2  | Keep_Awake# | TXLED# |
| CBUS3  | PWREN# | SLEEP# |
| Max Bus Power Current | 500mA | 90mA |
| Uart pulldown in suspend | enabled | disabled |

###uController

 [Design considerations](https://community.nxp.com/message/630601) when designing a board with debugging in mind.
