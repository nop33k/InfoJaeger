# InfoJaeger
usage: InfoJaeger.py [-h] [-s | -f] [UserInput]

Run security check against single IP addresses or list of IPs

positional arguments:
  UserInput     Enter single IP or Filename

optional arguments:
  -h, --help    show this help message and exit
  -s, --single  Check single IP
  -f, --file    Check list of IPs


## Find details from a single IP or from a file listing of IP addresses.

# SINGLE IP ADDRESS EXAMPLE:
  -% InfoJaeger.py - s <ip-address>
  
This command will print the ARIN details for 

  ASN: <details-here>
  CIDR: <details-here>
  Country: <details-here>

For Instance:
  -% InfoJaeger.py -s 8.8.8.8

Results:

  ASN: 15169
  CIDR: 8.8.8.0/24
  Country: US

# LIST OF IP ADDRESSES EXAMPLE:
  -% InfoJaeger.py -f hostslist.txt
  
  This command will get the ARIN details for all IP addresses in the list, return the details, and store them in a file called Outfile.txt
