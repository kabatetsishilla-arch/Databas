# Databas
HTTP
HTTPS = HyperText Transfer Protocol Secure
TLS = Transport Layer Security

(You asked about HTTP, so for completeness: HTTP = HyperText Transfer Protocol.)

HTTP is the protocol browsers and servers use to exchange web data. On its own, the data is sent as plain text, so anyone intercepting it can read it.
TLS is the security protocol that encrypts data travelling between two systems, so it can’t be read or altered on the way. It also verifies the server’s identity using a digital certificate. TLS is the modern successor to SSL (Secure Sockets Layer).
HTTPS is HTTP running over TLS. That’s the padlock you see in the browser.

Exam example (Case A): when an election official logs in to view their polling center assignment, HTTPS/TLS encrypts the username, password, and data, so an attacker on the network can’t read or change them.

Ready for Question Two when you are.

what are  some of the  security concerns for an online database explain in simple english

Here are the main security concerns for an online database, explained simply.

Unauthorized access: Someone who shouldn’t see or change the data gets in, like a stranger logging in to the election system. Fix: use strong passwords, add a second login step (like an SMS code), and give each person access only to what their job needs.
SQL injection: A hacker types harmful commands into a website form to trick the database into giving up or changing data. Fix: check everything users type before the database uses it.
Data interception: Data travelling over the internet can be spied on, like someone reading a letter in transit. Fix: use HTTPS/TLS, which scrambles the data so only the sender and receiver can read it.
Data theft from the server: If hackers break into the server, they can steal the stored data. Fix: encrypt the stored data and protect the server with a firewall.
Data tampering: Someone secretly changes records, for example marking a candidate as “cleared” when they weren’t. Fix: keep logs of who changed what and limit who can edit.
Denial of service (DoS): Attackers flood the system with so many requests that it crashes and real users can’t get in. Fix: use firewalls and tools that block or limit suspicious traffic.
Malware and ransomware: Harmful software damages the data or locks it until a ransom is paid. Fix: keep software updated, use antivirus, and keep backups.
Data loss: Data can disappear through attack, hardware failure, or mistakes. Fix: make regular backups and store them in a separate place.
Insider threats: A staff member misuses the access they legitimately have. Fix: give each person only the access they need and monitor their activity.
