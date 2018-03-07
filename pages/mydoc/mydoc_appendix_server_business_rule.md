---
title: Server side business rule
last_updated: July 3, 2018
keywords: logs, logging, log history, history
summary: "The following business rule monitors the contents of the <b>a_messagequeue</b> table for null <b>d_sent</b> column values. In this example, a null value indicates that a new table record has been added. For each new record row, a custom Web Service Web method takes the s_from, s_to, s_subject, and s_body values, constructs an e-mail message, and sends it to the recipient."
sidebar: mydoc_sidebar
permalink: mydoc_appendix_server_business_rule.html
folder: mydoc
---

```
Imports .Client
Imports .Server
Imports .Server.BusinessRule 'Required to create a business rule.
Imports .Server.Common
Public Const SQL_GET_COUNT = "select count(k_messagequeue) from a_messagequeue where d_sent is null" 

```
