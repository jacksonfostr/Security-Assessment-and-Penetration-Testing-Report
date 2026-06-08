# Security-Assessment-and-Penetration-Testing-Report
This project was completed as part of cybersecurity coursework in a controlled lab environment. The organization and findings are part of a simulated assessment for educational purposes.

Executive Summary
Protego Security Solutions was employed by Pixel Paradise Inc. to do a black-box penetration test of their web, network, and employee security. The main goal of this test was to find any vulnerabilities that could be used by an attacker and to check the organization’s overall security. Most of the testing was done using a black-box approach, with no knowledge of the internal systems. However, limited access was given for better testing of vulnerabilities, and certain workers were informed of the testing to avoid disruption of normal operations. This penetration test found multiple vulnerabilities across web applications, internal systems, and employee awareness. Issues included employees falling for phishing, injection flaws, weak access controls, exposed internal systems, and insecure IoT devices. These findings could allow unauthorized access, data loss, and lateral movement.

Scope
The test focused on the following areas:
	1	Internet-facing web applications like the community forum and digital store
	2	Internal network infrastructure and the file sharing systems
	3	Employee security awareness and social engineering attacks
	4	Internet-facing devices and IoT systems
	5	Active Directory and Windows domain security controls
The testing was done as a black-box test with a small amount of internal access and limited awareness was given to employees.

Methodology
Both automated and manual testing tools and techniques were used to assess security.
	1	Social engineering tests used phishing emails and fake login pages to assess employee awareness. 
	2	Network reconnaissance was performed using tools like Nmap, GVM/OpenVAS, Nikto, and OWASP ZAP to find exposed services and vulnerabilities.
	3	Internal testing focused on Active Directory and SMB using BloodHound, enum4linux, and smbclient. 
	4	Web application testing focused on input validation, injection flaws, and access controls.
	5	IoT device vulnerabilities were tested using Shodan to find publicly accessible IoT and camera systems.

Found Vulnerabilities
The assessment found several important vulnerabilities:

	1	Employees fell for phishing, with employees clicking on malicious links and entering their credentials on fake websites
	2	A rogue internal server was found with weak credentials and the wrong firewall configuration
	3	Unauthorized firewall rule changes allowed outside access to internal systems
	4	Weak SMB configurations could lead to lateral movement across the network
	5	Web applications were vulnerable to SQL injection, command injection, and had poor input validation
	6	The community forum contained vulnerabilities due to exposed user IDs
	7	Default credentials were found on multiple systems, including IoT surveillance devices
	8	Surveillance devices exposed sensitive banner information and lacked update support
	9	Windows domain password policies and access controls were weak

Risk Analysis
The found vulnerabilities show a high level of risk to the organization.
Successful exploitation could lead to:
	1	Unauthorized access to internal systems
	2	Loss of user and organization data
	3	Compromise of web applications and backend databases
	4	Lateral movement across the internal network
	5	Exposure of surveillance systems and physical security risks
	6	Credential harvesting through phishing and social engineering attacks

Overall, the combination of weak access controls and low user awareness increases the likelihood of a successful attack.

Recommendations
Improvements should include:
	1	Hiring a dedicated cybersecurity manager to oversee security
	2	Including mandatory security awareness training for all employees
	3	Do regular phishing assessments and social engineering tests
	4	Get rid of rogue servers and investigate the unauthorized firewall changes
	5	Enforce stronger password policies for Windows domains
	6	Restrict SMB file sharing
	7	Implement more secure coding practices
	8	Improve input validation to prevent injection attacks
	9	Replace exposed user IDs with randomized IDs such as GUIDs
	10	Remove the default credentials and secure all access points
	11	Replace the outdated IoT and surveillance devices with secure, updatable models

Conclusion
The organization has multiple security weaknesses that place systems and data at a high risk. These vulnerabilities are a combination of technical misconfigurations, insecure application design, and low user security awareness. 
Without any changes, the organization is vulnerable to external attacks, internal compromise, and data loss. Implementing the recommended controls, improving security policies, and mandatory employee training will all be important for improving the overall security and helping business growth.
should i add this pen testing report to my repo and projects 