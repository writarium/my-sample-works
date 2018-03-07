---
title: Troubleshooting
tags: [troubleshooting]
keywords: trouble, problems, support, error messages, problems, failure, error, #fail
last_updated: July 3, 2018
summary: "This page lists common errors and the steps needed to troubleshoot them."
sidebar: mydoc_sidebar
permalink: mydoc_troubleshooting.html
folder: mydoc
---

## Conflict Resolutions

### Viewing and Resolving Conflicts

As an administrator, you can view a list of conflicts queued for manual resolution. As new conflicts arise, you can also be sent an e-mail notification. To view conflict details and select the object value and perform the following steps.
    
1.	Start the Application Administrator tool.
2. Under the Logging category in the left pane, select Conflicts. The Conflicts page opens. 
3. Click a Resolve link to display details about that conflict. 
4. Click the update in the Current column to highlight it and display additional information about the conflict. Click a username (#) column to the right of the Current column to highlight it. Review the data in the columns to determine which update should prevail.
5. To select the winning update, highlight that column and click the Save icon.
6. Continue the steps above to resolve additional record conflicts.

### Unable to initializing logging on the client application

The client logging feature writes debug information to a log file on the Pocket PC. For details about the code change needed in your Pocket PC application to accommodate this functionality, see [Defining Business Objects.](mydoc_defining_business_objects.html)


## Users and Groups

### I'm cannot change a user's password using the Application Administrator tool

When you import a user, the password is only defined in the LDAP directory or Active directory. To change the password, you muse change it in the LDAP or the Active directory. A user must also be added to a security group before the user can log on to the Application Administrator tool;

### I'm unable to disable  permissions for imported users
You must define a user in the *m_user* table of the *MASMetadata* database to disable the imported user. Importing users from LDAP or Active Directory into the *m_user* table allows you the ability to enable or disable these user accounts. 
{% include note.html content="A disabled user is not authorized to access data on the mobile application, and when a disabled user attempts to access data, an alert message is displayed." %}



{% include links.html %}
