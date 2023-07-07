# DHCP Server Issue
 * No DHCP server is available and is automatically connected to the APIPA server

1. Check to see if the DHCP server is up and running.
2. Check the network cable connections to make sure they are secure.
3. Restart the DHCP server.
4. Restart the devices on your network.
5. Reset DHCP and flush DNS cache
6. If you are still having problems after following these steps, you may need to contact your network administrator for help.

## Reset DHCP and flush DNS cache
Here are the detailed steps on how to do it:

Open the Start menu and search for "Command Prompt".
Right-click on the Command Prompt app and select "Run as administrator".
In the Command Prompt window, type the following command and press Enter:

ipconfig /release

This command will release your current DHCP lease.

Type the following command and press Enter:

ipconfig /renew

This command will renew a new DHCP lease.

Type the following command and press Enter:

ipconfig /flushdns

This command will flush the DNS cache.

Close the Command Prompt window.
Your laptop should now have a new DHCP IP address and the cache of the old DHCP IP address should be cleared.


### DHCP
Link [DHCP] (https://github.com/CYBERPROJECT-WALLMARIA/Networking-Knowledge/tree/main/Common%20Protocols)

### APIPA
APIPA stands for Automatic Private IP Addressing. It is a feature in computer networking that allows devices to assign themselves a private IP address automatically when they are unable to obtain an IP address from a DHCP (Dynamic Host Configuration Protocol) server.

In a typical network environment, devices such as computers, smartphones, and printers rely on DHCP servers to provide them with unique IP addresses. However, in certain situations where a DHCP server is unavailable or misconfigured, devices may fail to obtain an IP address.

When this occurs, devices with APIPA enabled will assign themselves an IP address from a specific range reserved for APIPA. The APIPA range is defined as 169.254.0.0 to 169.254.255.255, with a subnet mask of 255.255.0.0. This range is designated for local communication within a network segment and is not routable on the internet.

APIPA allows devices to communicate with each other within the same network segment, even without a DHCP server. However, devices using APIPA addresses cannot communicate with devices outside their local network segment or access the internet.

APIPA addresses are temporary and are meant to be used as a fallback option until a valid IP address can be obtained from a DHCP server. Once a DHCP server becomes available, devices using APIPA will automatically switch to a dynamically assigned IP address from the DHCP server.

