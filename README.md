# Unit-18-Homework-Lets-Go-Splunking



**Scenario**
You have just been hired as an SOC Analyst by Vandalay Industries, an importing and exporting company.


Vandalay Industries uses Splunk for their security monitoring and have been experiencing a variety of security issues against their online systems over the past few months.


You are tasked with developing searches, custom reports and alerts to monitor Vandalay's security environment in order to protect them from future attacks.



#### Vandalay Industries Monitoring Activity

**Step 1: The Need for Speed**

- Background: As the worldwide leader of importing and exporting, Vandalay Industries has been the target of many adversaries attempting to disrupt their online business. Recently, Vandaly has been experiencing DDOS attacks against their web servers.

- Not only were web servers taken offline by a DDOS attack, but upload and download speed were also significantly impacted after the outage. Your networking team provided results of a network speed run around the time of the latest DDOS attack.

-  Task: Create a report to determine the impact that the DDOS attack had on download and upload speed. Additionally, create an additional field to calculate the ratio of the upload speed to the download speed.


    -  Using the eval command, create a field called ratio that shows the ratio between the upload and download speeds.
    -  Create a report using the Splunk's table command to display the following fields in a statistics report:

       - _time
       - IP_ADDRESS
       - DOWNLOAD_MEGABITS
       - UPLOAD_MEGABITS
       - ratio


**Eval Command Used to Show Ratio Between Upload and Download Speeds:**

![TODO](https://github.com/Tamie13/Unit-18-Homework-Lets-Go-Splunking/blob/main/Unit%2018%20HW%20screenshots/Upload%20:%20Download%20Field.png)

**Table Showing `TIME` `IP_ADDRESS` `DOWNLOAD_MEGABITS` `UPLOAD_MEGABITS` AND `RATIO`:

![TODO](https://github.com/Tamie13/Unit-18-Homework-Lets-Go-Splunking/blob/main/Unit%2018%20HW%20screenshots/Splunk%20Table%20Command.png)

**Answer the following questions:**

Based on the report created, what is the approximate date and time of the attack?
How long did it take your systems to recover?

Submit a screen shot of your report and the answer to the questions above.

Step 2: Are We Vulnerable?
Background:  Due to the frequency of attacks, your manager needs to be sure that sensitive customer data on their servers is not vulnerable. Since Vandalay uses Nessus vulnerability scanners, you have pulled the last 24 hours of scans to see if there are any critical vulnerabilities.

For more information on Nessus, read the following link: https://www.tenable.com/products/nessus


Task: Create a report determining how many critical vulnerabilities exist on the customer data server. Then, build an alert to notify your team if a critical vulnerability reappears on this server.


Upload the following file from the Nessus vulnerability scan.

Nessus Scan Results



Create a report that shows the count of critical vulnerabilities from the customer database server.

The database server IP is 10.11.36.23.
The field that identifies the level of vulnerabilities is severity.



Build an alert that monitors every day to see if this server has any critical vulnerabilities. If a vulnerability exists, have an alert emailed to soc@vandalay.com.


Submit a screenshot of your report and a screenshot of proof that the alert has been created.

Step 3: Drawing the (base)line
Background:  A Vandaly server is also experiencing brute force attacks into their administrator account. Management would like you to set up monitoring to notify the SOC team if a brute force attack occurs again.
Task: Analyze administrator logs that document a brute force attack. Then, create a baseline of the ordinary amount of administrator bad logins and determine a threshold to indicate if a brute force attack is occurring.


Upload the administrator login logs.

Admin Logins



When did the brute force attack occur?

Hints:

Look for the name field to find failed logins.
Note the attack lasted several hours.





Determine a baseline of normal activity and a threshold that would alert if a brute force attack is occurring.


Design an alert to check the threshold every hour and email the SOC team at SOC@vandalay.com if triggered.


Submit the answers to the questions about the brute force timing, baseline and threshold. Additionally, provide a screenshot as proof that the alert has been created.

Your Submission
In a word document, provide the following:

Answers to all questions where indicated.
Screenshots where indicated.


© 2020 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.
