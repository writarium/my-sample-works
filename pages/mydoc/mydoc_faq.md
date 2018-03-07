---
title: Frequently Asked Questions
permalink: mydoc_faq.html
sidebar: mydoc_sidebar
tags: [special_layouts]
keywords: frequently asked questions, FAQ, faqs, question and answer, collapsible sections, expand, collapse
last_updated: November 30, 2015
summary: "Here are some of the most frequently asked questions by our customers. Please contact customer support if you have any, so we can add them here."
toc: false
folder: mydoc
---

<div class="panel-group" id="accordion">
                    <div class="panel panel-default">
                        <div class="panel-heading">
                            <h4 class="panel-title">
                                <a class="noCrossRef accordion-toggle" data-toggle="collapse" data-parent="#accordion" href="#collapseOne">How do I view calls to user table objects?</a>
                            </h4>
                        </div>
                        <div id="collapseOne" class="panel-collapse collapse noCrossRef">
                            <div class="panel-body">
                                1.	Start the Application Administrator tool. <br />
                                2.	Under the Logging category in the left pane, select History. The History page appears.<br />
                                3.	In the Select User list, select a user.<br />
                                4.	In the Select View list, select a client user table object, or select All.<br />
                                5.	Click the Find icon. The History page redisplays with information about the requested client user table objects.<br />
                                For each object, the tables display associated attributes, the date and time when those attributes were updated, and each attribute's new value.<br />
                                6.	To view additional details about a particular object call, click a timestamp hyperlink. The History Record page opens. The History Record page displays the following additional information about the selected object call:<br />
                                o	Client Time: This displays the date and time the object was called from the client.<br />
                                o	Server Time: This displays the date and time the object call reached the server.<br />
                                o	Revision: This displays the number of times this object value has changed.<br />
                                *	Primary Key(s): Lists the attribute(s) used as the object primary key.
                            </div>
                        </div>
                    </div>
                    <!-- /.panel -->
                    <div class="panel panel-default">
                        <div class="panel-heading">
                            <h4 class="panel-title">
                                <a class="noCrossRef accordion-toggle" data-toggle="collapse" data-parent="#accordion" href="#collapseTwo">How do I view conflict details and select the object value that prevail?</a>
                            </h4>
                        </div>
                        <div id="collapseTwo" class="panel-collapse collapse noCrossRef">
                            <div class="panel-body"><br />
                            1.	Start the Application Administrator tool.<br />
							2.	Under the Logging category in the left pane, select Conflicts. The Conflicts page opens. <br />
							3.	Click a Resolve link to display details about that conflict. <br />
							4.	Click the update in the Current column to highlight it and display additional information about the conflict. Click a username (#) column to the right of the Current column to highlight it. Review the data in the columns to determine which update should prevail.<br />
							5.	To select the winning update, highlight that column and click the Save icon.<br />
							6.	Continue the steps above to resolve additional record conflicts.<br />

                            </div>
                        </div>
                    </div>
                    <!-- /.panel -->
                    <div class="panel panel-default">
                        <div class="panel-heading">
                            <h4 class="panel-title">
                                <a class="noCrossRef accordion-toggle" data-toggle="collapse" data-parent="#accordion" href="#collapseThree">How do I export the log to a delimited .txt file?</a>
                            </h4>
                        </div>
                        <div id="collapseThree" class="panel-collapse collapse noCrossRef">
                            <div class="panel-body"><br />
                                1.	Start the Application Administrator tool.<br />
                                2.	Under the Logging category in the left pane, select Logs. The Logs page opens. <br />
                                3.	(Optional) To show only those logs matching a specific level, category, server name, thread ID, or timestamp, specify the unique search criteria in the text box above the appropriate column heading. (The format must match the data format. For example, timestamp must use the format mm-dd hh:mm:ss where the time portion is in GMT format). In the case of level or category, select from the drop down. Click the Find icon.<br />
                                4.	Click the Export icon.<br />
                                5.	In the Export Log by Search Criteria dialog box, click the OK button.<br />
                                6.	In the File Download dialog box, click Save.<br />
                                7.	In the Save dialog box, navigate to the directory to which you want the log file downloaded, name the log file, and then click the Save button.<br />

                            </div>
                        </div>
                    </div>
                    <!-- /.panel -->
                    <div class="panel panel-default">
                        <div class="panel-heading">
                            <h4 class="panel-title">
                                <a class="noCrossRef accordion-toggle" data-toggle="collapse" data-parent="#accordion" href="#collapseFour">How do I permanently delete records from the log?</a>
                            </h4>
                        </div>
                        <div id="collapseFour" class="panel-collapse collapse">
                            <div class="panel-body"><br />
                                1.	Start the Application Administrator tool.<br />
                                2.	Under the Logging category in the left pane, select Logs. The Logs page opens. <br />
                                3.	To permanently delete log records matching a specific level, category, server name, thread ID, or timestamp, specify the unique delete criteria in the text box above the appropriate column heading. (The format must match the data format. For example, timestamp must use the format mm-dd hh:mm:ss where the time portion is in GMT format). In the case of level or category, select from the drop down. <br />
                                4.	Click the Delete icon.<br />

                            </div>
                        </div>
                    </div>
                    <!-- /.panel -->
                    <div class="panel panel-default">
                        <div class="panel-heading">
                            <h4 class="panel-title">
                                <a class="noCrossRef accordion-toggle" data-toggle="collapse" data-parent="#accordion" href="#collapseFive">How do I configure conflict notification for senders and recipients ?</a>
                            </h4>
                        </div>
                        <div id="collapseFive" class="panel-collapse collapse">
                            <div class="panel-body">
							1.	Start the Application Administrator tool.<br />
							2.	Under the Logging category in the left pane, select Settings. The Log Settings page opens. The Conflicts group box is shown.<br />
							3.	In Sender Email, enter the email address of the individual or group from whom the conflict notification will be sent.<br />
							4.	In Recipient Email, enter the names of all individuals who should be sent notification of record conflicts. Separate multiple email addresses with a semicolon (;).<br />
							5.	Check Include User to also send a record conflict notification to the user who introduced the conflict.<br />

                            </div>
                        </div>
                    </div>
                    <!-- /.panel -->
                    <div class="panel panel-default">
                        <div class="panel-heading">
                            <h4 class="panel-title">
                                <a class="noCrossRef accordion-toggle" data-toggle="collapse" data-parent="#accordion" href="#collapseSix">How do I verify the status of a user?</a>
                            </h4>
                        </div>
                        <div id="collapseSix" class="panel-collapse collapse">
                            <div class="panel-body">

                                1.	Start the Settings tool on the mobile client device. <br />
                                2.	Click the Config tab. <br />
                                3.	In the User Name box, enter the name of the user of interest.<br />
                                4.	In the User Password box, enter the user password. <br />
                                5.	Click the status button to check the status of the account. <br />
                                Note: A status message appears notifying you that the account is active or disabled.
                            </div>
                        </div>
                    </div>
                    <!-- /.panel -->
                    <div class="panel panel-default">
                        <div class="panel-heading">
                            <h4 class="panel-title">
                                <a class="noCrossRef accordion-toggle" data-toggle="collapse" data-parent="#accordion" href="#collapseSeven">What is the purpose of creating users?</a>
                            </h4>
                        </div>
                        <div id="collapseSeven" class="panel-collapse collapse">
                            <div class="panel-body">
                                Users are created in the Application Administrator tool for certain reasons. These are:<br />
                                -	To associate the user with security groups, and allow the user to log on to the Application Administrator tool. <br />
                                -	To associate the user with security groups, and allow or prohibit the user to call Web methods. <br />
                                -	To provide you with the ability to enable or disable users. 

                            </div>
                        </div>
                    </div>
                    <!-- /.panel -->
                    <div class="panel panel-default">
                        <div class="panel-heading">
                            <h4 class="panel-title">
                                <a class="noCrossRef accordion-toggle" data-toggle="collapse" data-parent="#accordion" href="#collapseEight">What is the difference between importing versus creating Users?</a>
                            </h4>
                        </div>
                        <div id="collapseEight" class="panel-collapse collapse">
                            <div class="panel-body">
                                Users can be imported into the m_user table from Active Directory or an LDAP directory. When a user has been imported into the metadata database, only the username is imported into the m_user table. The password is not imported into the metadata database. <br />
                                When you create a user in the Application Administrator tool, the user's password is included in the m_user table. This password can be changed using Application Administrator tool.

                            </div>
                        </div>
                    </div>
                    <!-- /.panel -->
                    <div class="panel panel-default">
                        <div class="panel-heading">
                            <h4 class="panel-title">
                                <a class="noCrossRef accordion-toggle" data-toggle="collapse" data-parent="#accordion" href="#collapseNine">What happens when I disable a user?</a>
                            </h4>
                        </div>
                        <div id="collapseNine" class="panel-collapse collapse">
                            <div class="panel-body">
                                Disabling an account prohibits the user from downloading data, uploading data, launching the mobile client application, and logging on to the Application Administrator tool. Users that are defined in the m_user table of the MASMetadata database can be disabled and enabled using the Application Administrator tool. The status of a user can be verified using the Settings page too.
                            </div>
                        </div>
                    </div>
                    <!-- /.panel -->
</div>
<!-- /.panel-group -->

{% include links.html %}