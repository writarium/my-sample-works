---
title: About logs and log history
last_updated: July 3, 2018
keywords: logs, logging, log history, history
summary: "The Application Server automatically collects log history. It can also log Web service metric data if it is configured to do so. This allows you to monitor the transactions that take place and to troubleshoot issues. You can log any of the services that comprise the Application Server and log metrics for the Web methods used by the Web services.<br>
Logging information is stored in the `m_log` table of the `MASMetadata` database. Metrics are stored in the `m_metric` table."
sidebar: mydoc_sidebar
permalink: mydoc_about_logs_and_log_history.html
folder: mydoc
---
## Configuring Client-Side Log Information

In addition to capturing server log information, client-side log information is also captured saved to a file named log.txt. This file is located on the device in the application folder. If users contact your Support personnel with issues, instruct them to navigate to the log.txt file, and open it. This is the first act of troubleshooting.

## Configuring the Logging Levels, History, and Metrics Collection

The Log Settings page is used to specify that the Application Server collect log history and Web method metric data.

## To configure logging levels and enable history and metrics collection

1.  Start the Application Administrator tool.
2.  Under the Logging category in the left pane, select **Settings**. The Log     Settings page opens. The Log Levels group box is shown. 
3.  For each category, select the level of message description to capture and     display in the Logs screen. By default, the message description level for     all Web services is set to "Error." Choose from:
-   **Error:** This logs only error messages.
-   **Important:** This logs only error and warning messages.
-   **Information:** This logs error, warning, and information messages.
-   **Verbose:** This logs error, warning, information, and verbose messages.
    {% include note.html content="The level of logging may negatively impact server performance depending on the amount of logging that occurs. Log size is limited only by the amount of disk space where the MASMetaData database is located." %}   
	
4.  Do one of the following:

-   To save the log file to the cache, make sure the **Caching** option is     selected. Clear this option if you do not want to save the log file to the     cache.

-   To enable the server to collect measurements (such as bytes received, characters sent, and response time) for all Web service Web methods, click     the **Turn ON all Metrics** button.
    {% include note.html content=" If you choose to use all Metrics, and subsequently turn off metric collection for one or more Web methods, the **Turn On all Metrics** button is toggled off automatically. Similarly, if you choose to turn off all Metrics, and subsequently turn on metric collection for one or more Web methods, the **Turn Off all Metrics** button is toggled off automatically. In these instances, the Status message provides additional information." %}
