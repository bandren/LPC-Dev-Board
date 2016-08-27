#Welcome
---

This is a repository for a custom LPC1769 development board.

#Post assembly setup

###USB - TTL UART

The FT230XS-U (usb-uart) chip has an internal MPT memory which needs to be programmed with different values than its default. The table below shows the required values and the default values of the various parameters. 

| Paramter | Required  | Default |
|:---------|:----------|:--------|
| CBUS0  | TRI-STATE | TXDEN |
| CBUS1  | RXLED# | RXLED# |
| CBUS2  | TXLED# | TXLED# |
| CBUS3  | VBUS_SENSE | SLEEP# |
| power source | external power | bus power |

###uController

[LPC1343FBD48,151](http://www.digikey.ca/product-detail/en/nxp-semiconductors/LPC1343FBD48,151/568-4945-ND/2180456) with digikey part number: 568-4945-ND. [Design considerations](https://community.nxp.com/message/630601) when designing a board with debugging in mind.
