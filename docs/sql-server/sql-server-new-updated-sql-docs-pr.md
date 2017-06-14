---
title: Updated - SQL Server docs | Microsoft Docs
description: Display snippets of updated content for recently changed in documentation, for SQL Server.
services: na
documentationcenter: ''
author: MightyPen
manager: jhubbard
editor: BYHAM
ms.service: na
ms.topic: updart-autogen
ms.technology: database-engine
ms.custom: UpdArt.exe
ms.workload: sql-server
ms.tgt_pltfrm: na
ms.devlang: na
ms.topic: updart-autogen
ms.date: 05/23/2017
ms.author: genemi
---
# New and Recently Updated: SQL Server docs



Nearly every day Microsoft updates some of its existing articles on its [Docs.Microsoft.com](http://docs.microsoft.com/) documentation website. This article displays excerpts from recently updated articles. Links to new articles might also be listed.

This article is generated by a program that is rerun periodically. Occasionally an excerpt can appear with imperfect formatting, or as markdown from the source article. Images are never displayed here.

Recent updates are reported for the following date range and subject:



- *Date range of updates:* &nbsp; **2017-05-01** &nbsp; -to- &nbsp; **2017-05-23**
- *Subject area:* &nbsp; **SQL Server**.




&nbsp;

## Updated Articles with Excerpts

This section displays the excerpts of updates gathered from articles which have recently experienced a large update.

The excerpts displayed here appear separated from their proper semantic context. Also, sometimes an excerpt is separated from important markdown syntax that surrounds it in the actual article. Therefore these excerpts are for general guidance only. The excerpts only enable you to know whether your interests warrant taking the time to click and visit the actual article.

For these and other reasons, do not copy code from these excerpts, and do not take as exact truth any text excerpt. Instead, visit the actual article.



&nbsp;

&nbsp;

<a name="TitleNum_1"/>

### 1. &nbsp; [SQL Server 2017 Release Notes](sql-server-2017-release-notes.md)

*Updated: 2017-05-17* &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;  ([Next](#TitleNum_2))

<!-- Source markdown line 28.  ms.author= "craigg".  -->

&nbsp;


<!-- git diff --ignore-all-space --unified=0 84e7a2a49f2893d49380db1ad75695d9a4fd59b2 27a145ad30c10fd667f926d2e092b88c0ba586c5 -->



**SQL Server 2017 CTP 2.1 (May  2017)**

**Documentation (CTP 2.1)**

- **Issue and customer impact:** Documentation for [!INCLUDE[ssSQLv14_md--../includes/sssqlv14-md.md)] is limited and content is included with the [!INCLUDE[ssSQL15_md--../includes/sssql15-md.md)] documentation set.  Content in articles that is specific to [!INCLUDE[ssSQLv14_md--../includes/sssqlv14-md.md)] will be noted with **Applies To**. 
- **Issue and customer impact:** No offline content is available for [!INCLUDE[ssSQLv14_md--../includes/sssqlv14-md.md)].

**SQL Server Reporting Services (CTP 2.1)**


- **Issue and customer impact:** If you have both SQL Server Reporting Services and Power BI Report Server on the same machine and uninstall one of them, you will no longer be able to connect to the remaining report server with Report Server Configuration Manager.
- **Workaround** To work around this issue, you must perform the following operations after uninstalling one of the servers.

    1. Launch a command prompt in Administrator mode.
    2. Go to the directory where the remaining report server is installed.

        *Default location for Power BI Report Server: C:\Program Files\Microsoft Power BI Report Server*

        *Default location for SQL Server Reporting Services: C:\Program Files\Microsoft SQL Server Reporting Services*

    3. Then go to the next folder. This will either be *SSRS* or *PBIRS* depending on what is remaining.
    4. Go to the WMI folder.
    5. Run the following command:

        ```
        regsvr32 /i ReportingServicesWMIProvider.dll
        ```

        You can ignore the following error, if you see it.

        ```
        The module "ReportingServicesWMIProvider.dll" was loaded but the entry-point DLLInstall was not found. Make sure that "ReportingServicesWMIProvider.dll" is a valid DLL or OCX file and then try again.
        ```

**TSqlLanguageService.msi (CTP 2.1)**


- **Issue and customer impact:** After installing on a machine that has a 2016 version of *TSqlLanguageService.msi* installed (either through SQL Setup or as a standalone redistributable) the v13.* (SQL 2016) versions of *Microsoft.SqlServer.Management.SqlParser.dll* and *Microsoft.SqlServer.Management.SystemMetadataProvider.dll* are removed. Any applications that have a dependency on the 2016 versions of those assemblies will then cease to function, giving an error similar to: *error : Could not load file or assembly 'Microsoft.SqlServer.Management.SqlParser, Version=13.0.0.0, Culture=neutral, PublicKeyToken=89845dcd8080cc91' or one of its dependencies. The system cannot find the file specified.*




&nbsp;

&nbsp;

---

<a name="TitleNum_2"/>

### 2. &nbsp; [What&#39;s New in SQL Server 2017](what-s-new-in-sql-server-2017.md)

*Updated: 2017-05-22* &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;  ([Previous](#TitleNum_1))

<!-- Source markdown line 31.  ms.author= "craigg".  -->

&nbsp;


<!-- git diff --ignore-all-space --unified=0 b3e965f62414af06d42f88497958a4bca67befce 82ad09ae9a917f26db3e2210b5cf89585e0e4c4e -->



**What's New in SQL Server 2017 CTP 2.1 (May 2017)**

**SQL Server Database Engine  **

- A new DMF, [sys.dm_db_log_stats--../relational-databases/system-dynamic-management-views/sys-dm-db-log-stats-transact-sql.md), is introduced to expose summary level attributes and information on transaction log files; useful for monitoring the health of the transaction log.  
- This CTP contains bug fixes and performance improvements for the Database Engine.
- For a detailed list of 2017 CTP enhancements in previous CTP releases, see [What's New in SQL Server 2017 (Database Engine)--../database-engine/configure-windows/what-s-new-in-sql-server-2017-database-engine.md).

**SQL Server Reporting Services (SSRS)**

- SQL Server Reporting Services is no longer available to install through SQL Server's setup as of CTP 2.1.
- Comments are now available for reports. Comments allow you to add perspective to what is in a report and collaborate with others in your organization. You can also include attachments with your comment.
- For more detailed SSRS what's new information, including details from previous releases, see [What's new in Reporting Services--../reporting-services/what-s-new-in-sql-server-reporting-services-ssrs.md). 
- For information about Power BI Report Server, see [Get started with Power BI Report Server](https://powerbi.microsoft.com/documentation/reportserver-get-started/).

**SQL Server Machine Learning Services**

- There are no new Machine Learning Services features in this CTP.
- For more detailed Machine Learning Services what's new information, including details from previous CTPs, see [What's New in SQL Server Machine Learning Services--../advanced-analytics/what-s-new-in-sql-server-machine-learning-services.md).  

**SQL Server Analysis Services (SSAS)**

- There are no new SSAS features in this CTP.  
- For more details about improvements and bug fixes in this release, see [What's New in SQL Server 2017 Analysis Services--../analysis-services/what-s-new-in-sql-server-analysis-services-2017.md).  





&nbsp;

<a name="compactupdatedlist"/>

## Compact List of Articles Updated Recently

This compact list provides links to all the updated articles which are listed in the preceding section.

1. [SQL Server 2017 Release Notes](#TitleNum_1)
2. [What&#39;s New in SQL Server 2017](#TitleNum_2)


<a name="sisters2"/>

&nbsp;

## Sister Articles

This section lists very similar articles for recently updated articles in other subject areas, within the same GitHub repository.


&nbsp;

[Microsoft/**sql-docs-pr**](https://github.com/microsoftdocs/sql-docs-pr/) repository on GitHub.com:

- [Updated recently: **Relational Databases and Microsoft SQL Server** docs](/sql/relational-databases/relational-databases-new-updated-sql-docs-pr)
- [Updated recently: **Microsoft SQL Server** docs](/sql/sql-server/sql-server-new-updated-sql-docs-pr)
- [Updated recently: **Transact-SQL in SQL Server** docs](/sql/t-sql/t-sql-new-updated-sql-docs-pr)


&nbsp;

<!--
[Microsoft/**azure-docs**](https://github.com/microsoft/azure-docs/) repository on GitHub.com:

- [Sisters list for **azure-docs** repo](https://docs.microsoft.com/azure/sql-server-new-updated-azure-docs/#sisters2)
-->

&nbsp;

