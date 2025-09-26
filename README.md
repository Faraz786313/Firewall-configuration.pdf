Firewall Configuration Task Report
Steps Performed:
1 Opened firewall configuration tool:-On Windows:Control Panel →System and Security →
Windows Defender Firewall →Advanced Settings.-On Linux:Used UFW in terminal (requires
sudo).
2 Listed current firewall rules:-Windows:Checked 'Inbound Rules'and 'Outbound Rules'
sections.-Linux:Command →sudo ufw status verbose
3 Added a rule to block inbound traffic on port 23 (Telnet):-Windows:New Rule →Port →
TCP/UDP→Port 23 →Block Connection.-Linux:sudo ufw deny 23
4 Tested the rule by attempting to connect to port 23 locally/remotely (using telnet or netcat).
Connection was blocked.
5Added rule to allow SSH (port 22)on Linux:sudo ufw allow 22
6 Removed the test block rule to restore original state:-Windows:Deleted the custom Telnet
blocking rule.-Linux:sudo ufw delete deny 23
7 Documented commands/GUI steps used for both Windows and Linux environments.
8 Summary:A firewall filters traffic based on rules.It examines packets and decides whether to
allow,block,or restrict traffic depending on defined policies,helping to protect the system from
unauthorized access.
This report documents the firewall configuration task,demonstrating how to block and allow specific
ports,test rules,and restore firewall settings.
