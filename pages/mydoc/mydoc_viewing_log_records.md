---
title: Working with log records
last_updated: July 3, 2018
keywords: sort logs, sort log, export log, view log
summary: "The Application Server automatically collects log history. It can also log Web service metric data if it is configured to do so. This allows you to monitor the transactions that take place and to troubleshoot issues. You can log any of the services that comprise the Application Server and log metrics for the Web methods used by the Web services.<br>
Logging information is stored in the `m_log` table of the `MASMetadata` database. Metrics are stored in the `m_metric` table."
sidebar: mydoc_sidebar
permalink: mydoc_viewing_log_records.html
folder: mydoc
---
The Logs page displays information about all logs currently stored in the log file. The logs can be sorted by log level, category, server name, thread ID, timestamp, or the IP address. To maintain a more meaningful log, you can delete any records containing a specific log level, category, server name, user name, thread ID, or timestamp. 
## To view log information

1.  Start the Application Administrator tool.

2.  Under the Logging category in the left pane, select **Logs**. The Logs page     opens. By default, log records are sorted by timestamp.

## To sort the log 

{% include note.html content="You can sort the log alphabetically (in descending or ascending order). You can also sort by level, category, server, user, thread ID, or timestamp. Click the appropriate column name and then click for a second time to sort the column in the opposite order." %}

## To limit records displayed in the log

1.  Start the Application Administrator tool.

2.  Under the Logging category in the left pane, select **Logs**. The Logs page     opens.

3.  In the **Page Size** textbox, enter the number of log records that will be     recorded to a page, for printing purposes. The minimum size is 100 and the     maximum is 500.

4.  To show only those logs matching a specific level, category, server name,     thread ID, or timestamp, specify the unique search criteria in the text box     above the appropriate column heading. (The format must match the data     format. For example, timestamp must use the format mm-dd hh:mm:ss where the     time portion is in GMT format). In the case of level or category, select     from the drop down. Click the **Find** icon.

5.  To redisplay all log records, set the level and category lists to the blank     selection (at the top of the list selections) and clear the server, message,     thread ID, and timestamp text boxes.

6.  Click the **Find** icon.

## To export the log to a delimited .txt file

1.  Start the Application Administrator tool.

2.  Under the Logging category in the left pane, select **Logs**. The Logs page     opens.

3.  (Optional) To show only those logs matching a specific level, category,     server name, thread ID, or timestamp, specify the unique search criteria in     the text box above the appropriate column heading. (The format must match     the data format. For example, timestamp must use the format mm-dd hh:mm:ss     where the time portion is in GMT format). In the case of level or category,     select from the drop down. Click the **Find** icon.

4.  Click the Export icon.

5.  In the **Export Log by Search Criteria dialog** box, click the **OK**     button.

6.  In the **File Download** dialog box, click **Save**.

7.  In the **Save** dialog box, navigate to the directory to which you want the     log file downloaded, name the log file, and then click the **Save** button.

## To permanently delete records from the log

1.  Start the Application Administrator tool.

2.  Under the Logging category in the left pane, select **Logs**. The Logs page     opens.

3.  To permanently delete log records matching a specific level, category,     server name, thread ID, or timestamp, specify the unique delete criteria in     the text box above the appropriate column heading. (The format must match     the data format. For example, timestamp must use the format mm-dd hh:mm:ss     where the time portion is in GMT format). In the case of level or category,     select from the drop down.

4.  Click the **Delete** icon.
