# Subflow for Asus DDNS
please note: you have to own an Asus router, as the registration is depending on MAC address and WPS PIN of physical router

## Setup

fill in the fields in the Asus DDNS subflow node:
 - Action: use "register" only once to register
           the desired <name>.asuscomm.com
           then use "update" to refresh the IP
 - Name:   enter the name without asuscomm.com
 - MAC:    enter the MAC address from the label 
           of your router
 - PIN:    enter the PIN from the label 
           of your router

## Usage

just send any msg to the node, 
content will be ignored

## Output
 - msg.statusCode - returned code (200 is OK)
 - msg.payload    - text message explaining
                    possible error
