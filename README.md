# Fullstack-Academy-Penetration-Testing-Report

During our cohort I was tasked with a Red Team Penetration test scenario. I have attached the report for your review. Below describes the parameters of the pentration test. 

------------------------------------------------------------
Scenario
Fullstack Academy has reviewed your team’s report and is satisfied with the results. Because your team did such a great job, they would like a follow-up penetration test with an isolated portion of the network that was not part of the original engagement. However, this isolated portion of the network has a small number of systems, so it does not make sense for your entire team to be involved with this follow-up engagement. Instead, your team has assigned you to complete the penetration test for this isolated network on your own, as you have proven yourself ready to handle this kind of engagement.

Rules of Engagement
You are authorized only to scan and attack systems that reside on the same /20 subnet on which your Kali instance resides (e.g., if the IP of your Kali instance is 172.31.6.161, you are only authorized to scan and attack systems on the 172.31.6.0/20 subnet).

No social engineering or client-side exploits are needed or permitted on this penetration test.

You are allowed to work with your classmates on this penetration test.
Everything you need to complete this test should be available to you on the systems already; there should be no need to download outside tools for this penetration test.

Problem
Capture the Flag machine to complete these challenges. Take notes and screenshots of your findings to use as you develop a report in the following section.

---------------------------------------------------------------
Challenge 1: Network Scanning
The first step is always reconnaissance. We need to identify all of the relevant targets in our network and find out what they're running. 

Challenge 2: Initial Compromise
Next, we need to find our initial compromise vector. Servers hosting openly accessible services, like websites and unsecured databases, are great places to start. 

Challenge 3: Pivoting
Now that you can run commands on the web server, we want to find a way to pivot into the other Linux machine on the network. 

Challenge 4: System Reconnaissance
With SSH access to the second Linux machine, our new goal is to find our way into the remaining Windows hosts.

Challenge 5: Password Cracking
With a password hash in our hands, we need to crack it to discover the actual password. 

Challenge 6: Metasploit
Start up the Metasploit framework on Kali, and load the windows/smb/psexec exploit module. 

Challenge 7: Passing the Hash
From your established Meterpreter session, perform a hash dump and save the results.

Challenge 8: Finding Sensitive Files
Using your Meterpreter shell, search the target server for a file named secrets.txt .

----------------------------------------------------------------
REPORT
Your manager, Jamar, would like you to write a report that will be shared with Fullstack Academy describing:

Objective of the penetration test
Tools used
Findings (including what is contained within the secrets.txt file).
