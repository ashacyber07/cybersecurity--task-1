# cybersecurity--task-1 port scanning 

# Task Objective 
 To scan my local network for open ports using Nmap and understand the network exposure.

# Tools Used 
   -Nmap 
   -Wireshark (optional)
   
# Scan Command Used
  nmap -sS 192.168.56.1/24

  OPEN TCP PORTS  AND SERVICES 
  Port - 135 - msrps - Microsoft RPC - Used for DCOM, can be a vector for remote code execution
  Port - 139 - netbios-ssn -NetBIOS Session -Older Windowss file sharing.known for vulnerabilities 
  port - 445 - mmicrosoft-ds -SMB(Server Message Block ) - Windows sharing,targeted by ransomware.
  port - 7070 - realserver -RealNetworks streaming - uncommon today; can pose security risks if unused.

  SECURITY RISK ANALYSIS 
  port 135 - medium - Often targeted for lateral movement inside network
  port 139 - High - Desprecated; should be disabled unless absolutely needed.
  port 445 - Exploited by WannaCry ,NotPetya;block if not used.
  port 7070 - Legancy media service ;ensure it's up to date or consider disabling
  
# save this Report 
  scan_report.html

  
