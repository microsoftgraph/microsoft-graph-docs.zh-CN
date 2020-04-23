---
title: 通用打印云打印 API 概述
description: 通用打印是一种新式打印解决方案，组织可以使用它通过 Microsoft 云服务来管理自己的打印基础设施。
author: braedenp-msft
localization_priority: Priority
ms.prod: universal-print
ms.custom: scenarios:getting-started
ms.openlocfilehash: 84a8a97315bb8ca62afb22f76db06fa67fb4e307
ms.sourcegitcommit: 9c16d84eac9c34134864ad63a9bb95c309218a44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/18/2020
ms.locfileid: "43557862"
---
# <a name="universal-print-cloud-printing-api-overview"></a>通用打印云打印 API 概述

通用打印是一种新式打印解决方案，组织可以使用它通过 Microsoft 云服务来管理自己的打印基础设施。

![通用打印 Azure 门户主页的屏幕截图](images/universal-print-portal-homepage.png)

## <a name="why-use-universal-print"></a>为什么要使用通用打印？

通用打印将关键的 Windows Server 打印功能迁移到 Microsoft 365 云中，这样组织就不再需要本地打印服务器，也不需要在设备上安装打印机驱动程序。 此外，通用打印还带来了一些关键功能，如用于授予打印机访问权限的安全组、基于位置的打印机发现和丰富的管理员体验。

随着组织采用通用打印，组织和独立软件供应商 (ISV) 可使用 Microsoft Graph 中的通用打印 API 来生成和扩展应用程序，从而支持新方案。

### <a name="print-documents-from-web-and-mobile-applications"></a>从 Web 和移动应用打印文档

将打印基础设施迁移到云中，可直接从 Web 和移动应用打印文档。

若要开始使用通用打印 API，请执行以下操作：

1. [创建打印作业](/graph/api/printer-post-jobs?view=graph-rest-beta)，并存储生成的文档 ID。
2. [将文档数据上传](/graph/api/printdocument-uploaddata?view=graph-rest-beta)到文档。
3. [启动打印作业](/graph/api/printjob-startprintjob?view=graph-rest-beta)。

### <a name="manage-printers"></a>管理打印机

跟踪组织的打印机、打印机配置和打印机使用情况是一项很复杂的任务。 通用打印 API 可以在所有三个方面实现集成。

* 使用[列出打印机](/graph/api/print-list-printers?view=graph-rest-beta)和 [printerStatus](/graph/api/resources/printerstatus?view=graph-rest-beta)，**监视打印机状态、配置和可用性**。

* 使用报告 API，**了解谁在使用打印机以及打印进度**：
  * [列出 dailyPrintUsageSummariesByUser](/graph/api/reportroot-list-dailyprintusagesummariesbyuser?view=graph-rest-beta)
  * [列出 monthlyPrintUsageSummariesByUser](/graph/api/reportroot-list-monthlyprintusagesummariesbyuser?view=graph-rest-beta)
  * [列出 dailyPrintUsageSummariesByPrinter](/graph/api/reportroot-list-dailyprintusagesummariesbyprinter?view=graph-rest-beta)
  * [列出 monthlyPrintUsageSummariesByPrinter](/graph/api/reportroot-list-monthlyprintusagesummariesbyprinter?view=graph-rest-beta)

* 通过修改打印机上的用户和组成员资格，**配置用户权限**：
  * [列出 allowedUsers](/graph/api/printer-list-allowedusers?view=graph-rest-beta)
  * [添加 allowedUser](/graph/api/printer-post-allowedusers?view=graph-rest-beta)
  * [删除 allowedUser](/graph/api/printer-delete-alloweduser?view=graph-rest-beta)
  * [列出 allowedGroups](/graph/api/printer-list-allowedgroups?view=graph-rest-beta)
  * [添加 allowedGroup](/graph/api/printer-post-allowedgroups?view=graph-rest-beta)
  * [删除 allowedGroup](/graph/api/printer-delete-allowedgroup?view=graph-rest-beta)

### <a name="seamlessly-replace-or-update-printer-hardware"></a>无缝更换或更新打印机硬件

用户只能看到[共享](/graph/api/print-post-printershares?view=graph-rest-beta)的打印机，这样管理员可以精细地控制哪个打印机硬件在给定时间可用。

共享打印机会创建 [printerShare](/graph/api/resources/printershare?view=graph-rest-beta) 资源，它可随时更新为指向其他打印机，这样就能轻松更换损坏的打印机硬件，或让打印机脱机接受维护。

若要在应用程序中使用此功能，请使用[更新 printerShare](/graph/api/printershare-update?view=graph-rest-beta) 来更新 printerShare 的 `printer` 引用。

## <a name="api-reference"></a>API 参考
在查找此服务的 API 参考？

- [Microsoft Graph Beta 中的通用打印 API](/graph/api/resources/print?view=graph-rest-beta)

## <a name="see-also"></a>另请参阅

- [什么是通用打印](https://docs.microsoft.com/universal-print/fundamentals/universal-print-whatis)
- 欢迎在 [UserVoice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) 上提供有关通用打印 API 的反馈！
