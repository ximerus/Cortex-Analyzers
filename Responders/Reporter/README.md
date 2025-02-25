# Reporter

A Cortex Responder for TheHive Project that creates a Markdown report for a given case.  This is a Work in Progress.

# Installation

See `requirements.txt` for dependencies.

# ToDo

- Automatically close the task that is generated for the report
- Include the Observable description (just has the tag)

# Sample Report

![TLP:WHITE](<https://www.us-cert.gov/sites/default/files/tlp/tlp_icons_small/TLP-ICONS_RGB_WHITE_sm.png>) Case #11: Introducing the Reporter responder
===============================================================================================================================================================================

Table of Contents
=================

* [Case Summary](#case-summary)
* [Case Description](#case-description)
* [Task Log Entries](#task-log-entries)
	* [Task Group \: Task Title](#task-group-\:-task-title)
	* [default \: Where does the report go?](#default-\:-where-does-the-report-go?)
	* [default \: This is a closed task](#default-\:-this-is-a-closed-task)
* [Case Observables](#case-observables)
* [Traffic Light Protocol (TLP) Definitions and Usage](#traffic-light-protocol-(tlp)-definitions-and-usage)

# Case Summary
  
**TLP:WHITE - Disclosure is not limited.**  

|  |  |
| :--- | :--- |
|**Severity** |Medium|
|**Created By** |admin|
|**Assignee** |admin|
|**Tags** |responder|
|**Case status:** |Open|
|**Start Date**|2019-11-17T05:36:00Z|
  
<div style="page-break-after: always;"></div>  
 
# Case Description
  
This is a test case for the Reporter responder  
 
# Task Log Entries

## Task Group \: Task Title
  
**Created At:** 2019-11-17T05:39:52Z  
**Created By:** admin  
**Assigned To:** admin  
**Case Status:** InProgress  
   
**Description:**   
This is the task description.  If there is no description present, then "No description specified" is put into the report in its place   
   
2019-11-17T05:40:56Z : This is a task log entry  
2019-11-17T05:41:08Z : This is another task log entry  
2019-11-17T05:41:23Z : Any attachments are not included in the report at this time
## default \: Where does the report go?
  
**Created At:** 2019-11-17T05:41:47Z  
**Created By:** admin  
**Assigned To:** admin  
**Case Status:** InProgress  
   
**Description:**   
After running the responder, the report is attached to a new task named "Autogenerated Report".

It is also available on the main case page under "Attachments" to download  
   
2019-11-17T05:44:03Z : The report is generated in Markdown format, so you can use other applications to convert it to another format.
## default \: This is a closed task
  
**Created At:** 2019-11-17T05:50:52Z  
**Created By:** admin  
**Assigned To:** admin  
**Case Status:** Completed  
   
**Description:**   
No description specified  
 
# Case Observables

|Created At|Data Type|Data|Sighted|IOC|Tags|
| :--- | :--- | :--- | :--- | :--- | :--- |
|2019-11-17T05:44:31Z|autonomous-system|AS0000|False|False|asn|
|2019-11-17T05:44:50Z|domain|www[.]google[.]com|True|False|domain|
|2019-11-17T05:45:02Z|file|TLP-ICONS_RGB_WHITE_sm.png|False|False|file|
|2019-11-17T05:45:19Z|filename|path/to/file[.]txt|False|False|file|
|2019-11-17T05:45:38Z|fqdn|fqdn[.]example[.]com|True|True|fqdn|
|2019-11-17T05:47:38Z|hash|B00D9D41F6558B315E8E1934D9FB5CF31C4F465443CE45D55F52AEEF6FF5CEFD|False|False|sha256|
|2019-11-17T05:48:03Z|ip|8[.]8[.]8[.]8|False|False||
|2019-11-17T05:48:03Z|ip|8[.]8[.]4[.]4|False|False||
|2019-11-17T05:48:33Z|mail|person@example[.]com|False|False|email|
|2019-11-17T05:49:00Z|mail_subject|FW: Hello!|True|True|email-subject|
|2019-11-17T05:49:09Z|other|"other"|False|False|other|
|2019-11-17T05:49:28Z|registry|HKLM\System|False|False|registry|
|2019-11-17T05:49:49Z|url|hxxps://blog[.]agood[.]cloud|False|False|url|
|2019-11-17T05:50:38Z|user-agent|Mozilla/5[.]0 (Windows NT 10[.]0; Win64; x64) AppleWebKit/537[.]36 (KHTML, like Gecko) Chrome/78[.]0[.]3904[.]97 Safari/537[.]36|False|False|UA, normal user agent|
  
<div style="page-break-after: always;"></div>  
 
# Traffic Light Protocol (TLP) Definitions and Usage

|Color|When should it be used?|How may it be shared|
| :--- | :--- | :--- |
|TLP:RED   <br> ![TLP:RED](<https://www.us-cert.gov/sites/default/files/tlp/tlp_icons_small/TLP-ICONS_RGB_RED_sm.png>)|Sources may use TLP\:RED when information cannot be effectively acted upon by additional parties, and could lead to impacts on a party's privacy, reputation, or operations if misused.|Recipients may not share TLP\:RED information with any parties outside of the specific exchange, meeting, or conversation in which it was originally disclosed. In the context of a meeting, for example, TLP\:RED information is limited to those present at the meeting. In most circumstances, TLP\:RED should be exchanged verbally or in person.|
|TLP:AMBER <br> ![TLP:AMBER](<https://www.us-cert.gov/sites/default/files/tlp/tlp_icons_small/TLP-ICONS_RGB_AMBER_sm.png>)|Sources may use TLP\:AMBER when information requires support to be effectively acted upon, yet carries risks to privacy, reputation, or operations if shared outside of the organizations involved.|Recipients may only share TLP\:AMBER information with members of their own organization, and with clients or customers who need to know the information to protect themselves or prevent further harm. **Sources are at liberty to specify additional intended limits of the sharing\: these must be adhered to.**|
|TLP:GREEN <br> ![TLP:GREEN](<https://www.us-cert.gov/sites/default/files/tlp/tlp_icons_small/TLP-ICONS_RGB_GREEN_sm.png>)|Sources may use TLP\:GREEN when information is useful for the awareness of all participating organizations as well as with peers within the broader community or sector.|Recipients may share TLP\:GREEN information with peers and partner organizations within their sector or community, but not via publicly accessible channels. Information in this category can be circulated widely within a particular community. TLP\:GREEN information may not be released outside of the community.|
|TLP:WHITE <br> ![TLP:WHITE](<https://www.us-cert.gov/sites/default/files/tlp/tlp_icons_small/TLP-ICONS_RGB_WHITE_sm.png>) |Sources may use TLP\:WHITE when information carries minimal or no foreseeable risk of misuse, in accordance with applicable rules and procedures for public release.|Subject to standard copyright rules, TLP\:WHITE information may be distributed without restriction.|
