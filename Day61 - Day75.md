# DAY 61

Did you know about the MITRE Navigator?

https://lnkd.in/eZaHhe3h

- ✅ Spent time exploring MITRE ATT&CK using the Attack Navigator, this helped me to connect attacker behaviour with where security controls should detect or respond.
- ✅ Completed the Cyber Kill Chain room on TryHackMe
- ✅ Started learning about planning and executing offensive operations, focusing on red team objectives align with real-world attack paths and outcomes.

# DAY 62

Glad to share that I’ve completed the Certified Red Team Operations Management (CRTOM) certification from Red Team Leaders .

Thanks for the amazing course 🫡 Joas A Santos

Modules Covered in this Course are:
- ✅Strategic Red Team Governance
- ✅Planning and Executing Offensive Operations
- ✅Post-Engagement Coordination
- ✅Operational Integration and Forward Strategy
- ✅Capstone, Assessment, and Operationalization

Key Takeaway:
- Shifting into offensive security isn’t easy, especially when you need to understand the operations, strategy, business and management, before exploring the technical side. Processing non-technical content took effort and a lot of note-taking, but completing the course and exam within a week made it a very rewarding experience. 

- I’m actively exploring full-time opportunities in Offensive Security, Red Teaming, and Application Security. Please check my profile and reach out if there are any relevant roles in your organisation.

Onto the next one 🚀

# DAY 63

Deeper you do the reconnaissance, more attack surface you uncover - Leads to finding more vulnerabilities 🐞 

- ✅ Completed the Information Gathering – Web Edition module on Hack The Box

Key takeaways:
- ✅ Whois, DNS and Subdomain Enumeration.
- ✅ Subdomain Bruteforcing and Virtual Hosts.
- ✅ Fingerprinting, Crawling and Discovery.
- ✅ Search Engine, Google Dorks and Web Archive Discovery.

# DAY 64

Do you know what LOLBins are? - Save this for your interview Prep!

LOLBins (Living off the Land binaries) are legitimate system tools that attackers abuse to perform actions beyond their original purpose. 

There are currently two websites that aggregate information on Living off the Land binaries(Check Pinned Comment). 

What Attackers do?
- 👉 Use legitimate tools and features already present in the target's environment. 
- 👉Leverage Trusted utilities to avoid detection, they are considered safe and commonly used within the network.
- 👉LOTL risks are more successful than virus attacks and are growing increasingly widespread. 
- 👉WMI, PowerShell, Mimikatz are frequent LOTL attack vectors.

- ✅Learnt how LOLBins are abused across different attack stages
- ✅Explored common tools and techniques attackers rely on

Have you heard of this attack? How do you detect and prevent this attack?

# DAY 65

Did you know? 

File transfer during an attack often relies on legitimate built-in tools rather than obvious malware!🔺 

- ✅Completed File Transfers module on Hack The Box
- ✅Completed Red Team Recon Room in TryHackMe
- ✅Applied for a few cybersecurity roles today.

Key takeaways:
- 👉Windows, Linux and Miscellaneous File Transfer Methods
- 👉Transferring Files with Code and Living off the Land (LOTL)
- 👉Protected File Transfers and Catching Files over HTTP/S
- 👉Active and Passive reconnaissance using various methods.

I am open to work and exploring opportunities in Offensive Security, Penetration Testing, or Application Security.

I’d appreciate any consideration or referrals


# DAY 66

Did you know SQLMap can do much more than just automate SQL injection💉 

Today, I explored how SQLMap can be used to bypass common web application protections and WAF mechanisms 🥷 

Learnt different techniques, and the switches to use along with the payload in the target
- --csrf-token to handle anti-CSRF protected requests
- --randomize to bypass unique value validation
- --eval to bypass calculated parameters
- --proxy for IP concealment
- --random-agent to evade User-Agent Blacklisting
- --tamper scripts to bypass WAF/IPS protections

For WAF bypass, SQLMap  uses a third-party library identYwaf, containing the signatures of 80 different WAF solutions - https://lnkd.in/eH_75gk4

Interesting how much we can play around with SQLMap.

Save this for your next SQL injection finding! Source: Hack The Box

# DAY 67

This kind of pattern is common in CTF challenges, but perfectly demonstrates why parameterized queries matter 🤯 

- ✅Completed SQLMAP Essentials module on Hack The Box
- ✅Completed the SQLMAP Room on TryHackMe
- ✅Also revisited the concepts of SQL injection - its types and prevention strategies.

Key takeaways:
- 👉 SQLMap tool Overview and advanced usage
- 👉Attack Tuning and Database Enumeration
- 👉Advanced Enumeration techniques
- 👉Bypassing Web Application Protections and OS Exploitation


# DAY 68

Can’t wait to get back to doing what I love 😄 

A Little Late posting this! 

I was invited to take part in a 24-hour CTF challenge conducted by the London Stock Exchange Group as part of their hiring process, along with submitting a pentest report documenting the findings.

It's been a while since i played CTF, hacking the web applications ethically. After applying for the role and receiving the invite, I decided to do my best.

Managed to capture all 10 flags. One of the challenges was very insane. It was a global competition, and I finished 12th Globally ✅ 

But beyond rankings, what felt special was putting my pentesting skills back into practice. Writing a full pentest report after years felt surreal 💯 

I spent a lot of time making sure the report was clear, structured, and readable, not just technically accurate. Added the first page of my report. That part reminded me why I enjoy this field. 

Now waiting for the next update. Whatever the result, this was a solid checkpoint in the journey. 

I’m actively looking for opportunities in Offensive Security, Penetration Testing, and Application Security in the UK. If you’re hiring or know of a suitable role, I’d be happy to connect and share more about my experience. 


# DAY 69

Ever been inside a network but couldn’t reach anything else? 🤯 

That’s where pivoting comes in. Pivoting is all about using a compromised machine as a bridge to access internal systems that are not directly reachable from outside.

Today I explored different ways to pivot inside a network and got to use some of them in hands-on practice as well.

- 👉 Proxychains – Useful when you want your tools (like Nmap or Burp) to go through a compromised machine and reach internal systems.
- 👉SSH tunneling and port forwarding – Still one of the most reliable ways to move traffic around internally using local, remote, or dynamic forwarding.
- 👉Plink – Can be used on Windows targets when you need SSH-style pivoting without a full SSH client setup.
- 👉Chisel – Great when outbound traffic is restricted and you need to tunnel over HTTP.
- 👉Socat – Very flexible for relaying traffic between ports in custom pivot scenarios.
- 👉Sshuttle – Feels almost like creating a quick VPN into the internal network through SSH.
- 👉Ligolo-ng – Modern approach sets up a TUN interface and makes more easy.

Personally, I found SSH tunnelling and rpivot really interesting.


# DAY 70

Getting in is Easy. Command and control Keeps you there👀

Command and Control? 
A communication channel between the attacker and the compromised machine. Without C2, access is temporary. With C2, commands, file transfers, and lateral movement become possible.

How C2 blends in?
Instead of obvious traffic, C2 often uses normal protocols like HTTP, HTTPS, or DNS to avoid standing out.

Beaconing behaviour?
I didn’t realise how important beacon timing is until I looked into sleep intervals and jitter.

Why pivoting + C2 go together?
Pivoting expands access inside the network. C2 maintains and coordinates that access.

Explored a few common C2 platforms and frameworks.
- 👉Metasploit (Meterpreter) – Classic framework for session handling and post-exploitation.

- 👉Cobalt Strike – Popular in red team operations for beaconing and controlled engagements.

- 👉Sliver – A modern open-source alternative.

- 👉Mythic / Covenant – Modular C2 frameworks for structured operations

# DAY 71

I didn’t expect this to be part of my Master’s journey❤️ 

During my Master’s at the University of Warwick, WMG, University of Warwick 

Beyond lectures, assignments, project work and technical focus.
I made a conscious effort to invest time in developing my employability skills.

Through the Skills+ Development Programme. Completed over 100 hours of structured growth outside the classroom.

It wasn’t about ticking boxes.
It was about stepping outside comfort zones.

Working on how I communicate.
- How I collaborate.
- How I think critically.
- How I present ideas clearly.

Received the Warwick Award after developing skills across areas such as:
- Critical thinking and problem solving
- Communication and teamwork
- Professionalism and organisational awareness
- Digital literacy and ethical values
- Intercultural awareness and self-awareness

These aren’t just academic skills.
Capabilities UK employers genuinely look for when hiring graduates.

Special thanks to Claire Dixon for the support throughout the programme.

Now, I’m actively looking for full-time opportunities in Offensive Security, Penetration Testing, and Application Security in the UK.
 
If you’re hiring, I’d love to connect

# DAY 72

I had Domain Admin… and still got Access Denied ❗ 

When I was practising Active Directory Lab Exploitation today,

Compromised the child domain. Got Domain Admin.

Dumped krbtgt hash - Forged Golden Ticket - injected the SID. All good
klist showed the TGT. 

Then I tried accessing the parent Domain Controller. Access Denied:)

Curious why I couldn't access. After Sometime figured out that authorization failed.

Just because a child domain trusts the parent doesn't mean privileges automatically flow upward.

Domain Admin in a child domain? Yeah, that only works inside that domain.
Enterprise Admin? That's parent domain territory. Completely separate.

Here's the part I missed - trust just means you can authenticate. That's it. Authorization is a different conversation. And SID injection? Only works if the trust is actually configured to allow it.

Learned this the hard way today!

How did I fixed?
- To access the parent DC, I need to either:
- Compromise the parent domain directly - I was injecting the child domain
- Inject Enterprise Admin SID (519) or exploit the trust with Extra SID attacks - didn't know about this before

Takeaways:
- ✅Domain Enumeration, Compromise, and trust mapping
- ✅Mimikatz and Golden Ticket Execution
- ✅Tested Cross-Domain Boundaries & Analyzed Failure


# DAY 73

In the world of red teaming, Impacket feels less like a tool and more like an arsenal🗡️

What is Impacket?
It’s a collection of Python-based utilities that allow you to interact directly with network protocols, especially in Windows and Active Directory environments. 

And the more I understand it, the more I realise how powerful it really is 🥷 

Today, I went deeper into how Impacket enables Kerberos abuse!

Practised these scripts:
- GetNPUsers – for AS-REP Roasting when pre-authentication is disabled.
- GetUserSPNs – Identifying service accounts vulnerable to Kerberoasting.
- GetTGT – Requesting Kerberos tickets and using them for remote access.
- Ticketer – Crafting forged tickets (Golden Ticket scenarios).
- TicketConverter – Converting between ticket formats when switching toolsets.
- GetADUsers – Powerful enumeration of domain users.
- PsExec – Executing commands remotely using valid credentials over SMB.
- SMBExec – Leveraging SMB for RCE
- WMIExec – Using built-in Windows management features for RCE.

The interesting part?
None of these are exploits.

At first, these look like just scripts. But it goes beyond just running scripts. 

Still early in this journey, but it’s interesting how much red teaming revolves around tools.

Also, completed the Red Team Threat Intelligence room on TryHackMe — Learnt the fundamentals of threat intelligence, how to apply it in red team engagements, and how frameworks guide the planning of intel-driven campaigns.

What is your favourite script in Impacket?

# DAY 74




# DAY 75
