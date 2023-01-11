# MS-Audit-Log-Configure
PowerShell Script for Local Log Policy Audit Management

<b>Script ps-audit.ps1</b><br>
Usage:<br>
 -h  ->  Get This Help<br>
 -l  ->  Load and Save in CSV (ActualSetting_ComputerName.csv) Actual Audit Settings<br>
 -p AuditTemplate.csv  ->  Print Audit Settings from AuditTemplate.csv file<br>
 -c AuditTemplate.csv  ->  Compare Audit Settings with Desired AuditTemplate.csv file<br>
 -s AuditTemplate.csv  ->  Sync Audit Settings with Desired AuditTemplate.csv file<br>
 <br>
 <b>Included CSV files</b><br>
 Are Best Practice policies from MS<br>
 Link: https://learn.microsoft.com/en-us/windows-server/identity/ad-ds/plan/security-best-practices/audit-policy-recommendations<br>
 * system-audit-settings-stronger-recommendation-server-DC.csv<br>
 * system-audit-settings-stronger-recommendation-server.csv<br>
 * system-audit-settings-stronger-recommendation-workstation.csv<br>
 <br>
 
 # Screenshots
 <br><b>Script help</b><br>
 ![2](https://user-images.githubusercontent.com/39199196/211798460-880b01ed-1d24-4c38-81d7-fbb5286b0aae.png)<br>
 <br>
 <br><b>Load Current Local Policy</b><br>
 ![3](https://user-images.githubusercontent.com/39199196/211798695-557fc40b-b5f7-4300-b509-03fde5472959.png)<br>
 ![4](https://user-images.githubusercontent.com/39199196/211798733-23d3d56f-824a-4880-aa29-7696bf8604fc.png)<br>
 <br><b>Compare Current Local Policy with Desired</b><br>
 ![5](https://user-images.githubusercontent.com/39199196/211798931-289cafe8-a96d-42d8-8b28-633ad55adf03.png)<br>
 <b>-</b> means no matching policies (D - Desired Policy Setting has logging of [S - IsSuccessEnabled] and [F - IsFailureEnabled] or [(Empty or -) means no policy]. A - Actual   Policy Setting)<br>
 <b>+</b> means that policies are the same<br>
 <b>?</b> means that no such audit policy on machine<br>
 <br><b>Sync Current Local Policy with Desired</b><br>
 ![6](https://user-images.githubusercontent.com/39199196/211799043-d9a0ae50-b727-45af-8cb7-0a629ea8a204.png)
