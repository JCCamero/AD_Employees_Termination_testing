AD Employees Termination testing
================================

Continuous Auditing testing on timely termination of employees in Active Directory


BUSINESS RISK

In our company, Active Directory allows access not only to the network but also to other corporate systems and tools by using single sign-on feature.

With 70,000 active AD accounts and 150,000 terminations of employees per year (overall) across the globe, the timely deactivation of the accounts becomes a hard duty to prevent unauthorized transactions performed by unauthorized personnel on critical financial systems.

Besides the above, SOX requirement must be met.

CONTROL

Timely deactivation of the AD accounts is a global admin responsibility. Employees’ terminations report is sent by HR department twice a day by an email notification.

TESTING APPROACH

This project intends to be part of our new Continuous Auditing program which leverages the new EXECUTE command in ACL Analytics 10 to assess the timely termination of the AD accounts. The scripts included intend to work as follow:

  1.Generate a current list of AD accounts through the use of ADFind tool (i.e. command line Active Directory LDAP query, it is a free tool).
  
  2.Import and/or update the Employees’ Termination listing.
  
  3.Analyze the imported data by matching termination report against to AD listing to look for exceptions (i.e. enable accounts belonging to term employees, login activity after term date).

THIRD-PARTY REQUIREMENTS and USE OF EXECUTE COMMAND

Please refer to EXECUTE.docx file.
