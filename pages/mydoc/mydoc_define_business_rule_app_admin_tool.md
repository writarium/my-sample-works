---
title: Defining Business Rules in the Application Administrator tool
keywords: logging on, logging on application administrator tool
last_updated: July 3, 2018
summary: "After creating a business rule code in Microsoft Visual Studio, you need to define the business rule in Application Administrator tool."
sidebar: mydoc_sidebar
permalink: mydoc_define_business_rule_app_admin_tool.html
folder: mydoc
---

##  Defining a business rule

1.  Start the Application Administrator tool.

2.  From the Business Rules category in the left pane, select Business Rules.

3.  In the Class Name box, enter a unique class name identifier for this business rule.

4.  Select the assembly from the Assembly list to which you want to link the class you named in step 3.

    {% include note.html content=" Usually, the assembly linked to a business rule contains DLLs that, in turn, contain the actual compiled business rules" %}

5.  Click the Save icon.

    <img src="images/define_business_rule_app_admin_tool.png" alt="Jekyll" caption="This is a sample caption">

6.  To view the event generators using the selected business rule, select the Event Generators tab. The information displayed on the Event Generators tab is read-only. For more information, see Defining Event Generators.

7.  To view any business objects associated with this business rule, select the Business Objects tab. The information displayed on the Business Objects tab is read-only. For more information, see To define a business object event and map it to a business rule.
