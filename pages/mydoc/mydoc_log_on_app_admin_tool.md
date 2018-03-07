---
title: Logging on to the Application Administrator tool
keywords: logging on, logging on application administrator tool
last_updated: July 3, 2018
summary: "The administrator procedures described in this guide are performed using the Application Administrator tool. The default path of the Application Server is http://localhost/Server/default.aspx. When you log on to the Application Administrator tool for the first time, the login service uses localhost as the server by default. In case you enter a server name other than localhost, the Application Administrator tool uses this server name when you log on to the server the next time. You must enter a database name if you have entered a server name. If you do not enter a value in the Server Name box, the Server uses localhost as the default server and MASMetadata as the default database. "
sidebar: mydoc_sidebar
permalink: mydoc_log_on_app_admin_tool.html
---

## Log on to the Application Administrator tool

1.  Navigate to the default page of the Application Administrator tool: <http://localhost/Conductor/Login.aspx>, where localhost is the name of the server on which the Application Server is installed. The Application Administrator tool Login page appears as shown in the following figure.
<img src="images/application-administrator-tool-login-page.png">

2.  In the **Username** box, enter an administrator user name. The installer     creates a default user that is part of the Administrators group. That     default user name is **admin**.

3.  In the **Password** box, enter the password for the account. The default     password is **password123**.

## Change the Default Administrator Account Credentials

Until changed, the default administrator account credentials are:

-   username: **admin**

-   password: **password123**

To ensure the security of your server, change the credentials for this account as soon as possible.

## Change the administrator account credentials

  1.  Log on to Application Administrator tool as a member of the administrators group.
  2.  Under the Security heading in the left pane, select **Users**.    
  3.  In the User ID column, click the **admin** user.
  4.  If necessary, change the user name of the admin account by modifying the name in the **User ID** box.
  5.  Click the **Change** button to change the admin password.
  6.  In the **Old Password** box, enter the default password as **password123**.
  7.  In the **New Password** box, enter the new password.
       {% include note.html content="The password is composed of letters and digits and cannot contain more than 25 characters. Passwords cannot be left blank." %}
  8.  Click the **Submit** button to save the changes. The password is changed, and you are returned to the User form.
  9.  Be sure to add the user to the Administrator group.

{% include links.html %}
