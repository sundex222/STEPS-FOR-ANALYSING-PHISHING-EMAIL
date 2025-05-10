# STEPS-FOR-ANALYSING-PHISHING-EMAIL

STEPS FOR ANALYSING PHISHING EMAIL

Conducted by OGUNDOYIN SUNDAY MICHEAL; Cybersecurity Analyst, Ethical Hacker.

A suspicious email was captured via the company's email gateway and subjected to detailed analysis. The email was isolated in a sandboxed virtual environment to ensure secure handling.
Therefore :

* Performed email header inspection to trace the source and detect anomalies.
* Conducted URL reputation checks using threat intelligence platforms.
* Gathered relevant threat intelligence to assess indicators of compromise (IOCs).



1. <h2>STEP 1: Download the emil on a sandbox or virtual mchine</h2>

If you receive a phishing email in your inbox or spam folder, avoid clicking on any links, as doing so could expose your system to attackers. Instead, consider safely downloading the email and analyzing it within a secure virtual machine environment.

<img src="Folder/phishing 01.PNG">
2. <H2>STEP 2: Analyze the url with tools like symante.bluecoat.com, urlsan.io, virustotal, phishtank</H2>

You can download sample phishing emails from a repository called Phishing Pot, which is available on GitHub. Phishing Pot contains real phishing emails that have been reported and shared for educational and research purposes. To access it, simply search for 'Phishing Pot GitHub' on Google. Once you find the repository, select an email sample and use your virtual machine to download and analyze it safely.
<img src="Folder/phishing 001.PNG">

<img src="Folder/phishing 1.PNG">

3. <h2>STEP 3: Analyze the email headers</h2>

To analyze the sample email you downloaded from Phishing Pot, install Mozilla Thunderbird on your virtual machine. Thunderbird functions as an email client, allowing you to open and view the phishing email in an environment that closely resembles a real inbox. This helps simulate a realistic email interaction for safer analysis.
<img src="Folder/phishing 2.PNG">





4. <h2>STEP 4: Check the spf record, if it is equal to none or diabled, this may be a signal</h2>

It is also to check the email to know if it's pass or Fail

After opening the phishing email retrieved from Phishing Pot using Thunderbird, you can analyze the links it contains by submitting them to public scanning services. Use tools like Urlscan.io, Symantec, VirusTotal, and PhishTank to examine the URLs. These platforms help determine whether the links are associated with phishing activity or malicious content, providing a clearer assessment of the threat.
<img src="Folder/phishing 4.PNG">

<img src="Folder/phishing 5.PNG">

<img src="Folder/phishing 6.PNG">





5. <h2>STEP 5: Check return ip address</h2>
<img src="Folder/phishing 7 header.PNG">


6. <h2>STEP 6: Compare the return address to the from address, and if it doesn't match, this may be a signal too</h2>
<img src="Folder/phishing 7 header.PNG">





7. <h2>STEP 7: Check the address of the ip address of the sender on  abuseipdb</h2>

Check the IP adress on abuseipdb.com to know if it has been reported for any malicious activities or not
<img src="Folder/phishing 8.PNG">

<img src="Folder/phishing 9.PNG">




<h2>CONCLUSION</h2>

Following a thorough inspection of the email headers, identification of authentication failures, and analysis using third-party threat intelligence tools, I have determined that this email is a confirmed phishing attempt. It is designed to deceive recipients into clicking a potentially malicious link hosted on the 'devicetechie' domain. Both the domain and associated IP address display indicators commonly linked to phishing infrastructure, however there are no existing reports associated with this IP address in the AbuseIPDB database, perhaps, the absence of reports should not be interpreted as an indication of safety, particularly in light of the suspicious context.

<h2>Report Prepared by:</h2>

OGUNDOYIN SUNDAY MICHEAL

SECURITY ANALYST
