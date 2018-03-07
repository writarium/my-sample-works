---
title: About business Rules and Constants
keywords: logging on, logging on application administrator tool
last_updated: July 3, 2018
summary: "Business rules enable you to apply consistent logic to your business data."
sidebar: mydoc_sidebar
permalink: mydoc_business_rules_constants.html
folder: mydoc
---

 In general, business rules define:

-   **How data is handled when it is manipulated** (inserted, updated, saved,     reverted, located, or deleted)**:** Take, for example, a business rule that,     on a save action, checks a service estimate against the contact of the     customer monetary authorization limit. This type of business rule is     triggered by a business object event that is associated with a     business objects using the Application Administrator tool.

-   **How data is handled when it is validated:** Take, for example, a business     rule that verifies that there are nine digits in a social security number or     that a company has required identification code has been entered.

-   **How data integrity is handled:** For primary keys of type String, for     example, your business rule can ensure that the key remains unique.

Business rules enable the functionality defined in your .NET source code. For example, the JobTitleRequired business constant can be set to True or False. However, the logic that actually checks to verify whether a Job Title must be provided and what happens if the job title is not provided is enabled by a business rule. In this case, an event triggers the business rule, and then business constant, to be evaluated. Use the Application Administrator tool to specify the business rule that would be started either before or after any of the above events.

{% include note.html content="The logic used to enable a business rule is defined in a DLL, which is developed using VB.NET. The Application Administrator tool is used to define the business rule by referencing the business rule DLL." %}

{% include note.html content="Business rule definition information is stored in the metadata database." %}
### Invoking Business Rules

On the device, a business rule is invoked by your custom code or by a business object event. On the server, a business rule is invoked by an event generator.

### Defining Business Rules 

Because business rules use DLLs to enforce rules, business rules are typically created by database administrators or developers using VB.NET.

### Creating Business Rules

There are two general steps to creating a business rule for use by your small factor application. These are:

-   Use Microsoft Visual Studio to create a business rule class. Add Evaluate     and TakeAction code. Compile this into a DLL.

-   Using the Application Administrator tool, name the data manipulation event     that trigger the business rule.

Or you can create an event generator that fires the business rule at a specific time or time interval. For more information, see [Defining Event Generators](##_Defining_Event_Generators).

### Using Microsoft Visual Studio.NET to Create a Business Rule

Before mapping to a business rule using the Application Administrator tool, you must have already created the business rule class in Microsoft Visual Studio. An example of an address validation business rule is illustrated in the following figure.

<img src="images/dot-net-ide.png">

The AddressValidate business rule shown in the above and in the code following, for example, identifies each required input box and the action to take if the user does not enter a value. In each case, a message (a business constant) is displayed.

In the first line, AddressValidate refers to the Business Rule. This is referenced in the Application Administrator tool as Apps.BusinessRules.AddressValidate (the full namespace of the class file). The second line is necessary, as your business rules must always inherit from BusinessModel.BusinessRule.

```
Public Class AddressValidate

Inherits BusinessModel.BusinessRule
```
