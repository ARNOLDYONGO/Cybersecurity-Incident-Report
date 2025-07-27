# Cybersecurity incident report

## Summary of the problem found in the DNS and ICMP traffic log

The network protocol analyzer logs indicate that port 53 is unreachable when attempting to access the yummyrecipesforme website. Port 53 is normally used for
HTTPS traffic. This may indicate a problem with the web server or the firewall configuration. This may be an indication of a malicious attack on the web server.

## Analysis of the data and cause of the incident
The incident occurred earlier this afternoon. Clients reported that they were not able to access the client company website www.yummyrecipesforme.com, and saw the error “destination port unreachable” after waiting for the page to load. I responded by attempting to visit the website and also received the error “destination port unreachable.” Then began to run tests with the network protocol analyzer tool tcpdump. The resulting logs revealed that port 53, which is used for HTTPS traffic, is not reachable. We are continuing to investigate the root cause of the issue to determine how we can restore access to the secure web portal. Our next steps include checking the firewall configuration to see if port 53 is blocked and contacting the system administrator for the web server to have them check the system for signs of an attack. The team believes it might be a DoS attack that is flooding the network and, therefore, blocking access. This might be the reason that led to the crash of the yummyrecipeforme website.

