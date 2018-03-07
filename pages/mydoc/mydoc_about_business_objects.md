---
title: About business objects
keywords: business objects, object, objects
last_updated: July 3, 2018
tags: [business_objects]
summary: "Business objects are a very prominent part of the Application Designer and its components. To develop flawless applications, one must have an exhaustive knowledge of business objects, creating it, and understanding the various events associated with it."
sidebar: mydoc_sidebar
permalink: mydoc_about_business_objects.html
folder: mydoc
---

## Understanding Business Objects

A business object represents a specific type of data used by the application. Examples include product, product number, appointment, and so forth. Business objects defined and modified using Application Administrator tool are physically stored in the metadata repository.

This version of a business object packages data source metadata that is passed to the device and then manipulated by your small factor application's public class BusinessObject statement(s). Unlike the BusinessObject class, however, a business object does not contain any business logic. The business logic is completely contained in your Visual Basic code.

The metadata repository contains the schema for the business objects, business rules, business constants, views, and columns used by the Application Server. The metadata repository is stored in a SQL Server database. When the Pocket PC user selects the Settings, Subscribe tab, and Get Customer Data Definition option, the metadata b_mac database is created and populated with data from the metadata repository. Any defined business objects are used to create the b_mac table definitions. 
The following figure illustrates the relationship between business objects and views, and between business object properties and view columns.
<a data-fancybox="gallery" href="images/app-server-and-views.png" title="click to enlarge" alt="application server and view">
<img src="images/app-server-and-views.png" style="width: 300;"/>
</a>
