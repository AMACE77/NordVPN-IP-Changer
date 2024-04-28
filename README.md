**NordVPN IP Changer Script**

Overview:

This Bash script automates the process of changing the IP address provided by NordVPN. It attempts to connect to a NordVPN server in the United States every three minutes and fetches the public IP address from ifconfig.me. If the connection fails, it automatically retries after disconnecting from NordVPN and waiting five seconds.

Requirements:

    Bash shell (sudo apt install bash)
    NordVPN client installed and configured (see https://github.com/NordSecurity/nordvpn-linux)
    curl (sudo apt install curl)

Usage:

   - Make sure you have the necessary permissions to execute the script (chmod +x ipchanger).
   - Run the script by executing the following command:

    ./ipchanger

   - The script will attempt to connect to a NordVPN server in the United States (changed to desired country) every three minutes, displaying the VPN number and the new public IP address associated with each successful connection.
   - If the connection fails, the script will automatically disconnect and retry after five seconds.

Notes:

   - Ensure that the NordVPN client is properly configured on your system before running the script.
   - The script currently sleeps for three minutes between connection attempts. You can adjust this interval as needed      by modifying the sleep command in the script.

Disclaimer:

This script is provided as-is without any warranty. Use it at your own risk.
