---
title: SharePoint 网站使用情况报表
description: 您可以根据用户在 SharePoint 网站中存储的文件总数、活动使用的文件数以及在所有这些网站中使用的存储，从 SharePoint 中获取要获取的值的高级别视图。 然后，可深入研究 SharePoint 网站使用情况报表，了解所有网站的趋势和其中每个网站的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 86359fd9be572f76d04a188503b217fd892e5d80
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520715"
---
# <a name="sharepoint-site-usage-reports"></a>SharePoint 网站使用情况报表

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

您可以根据用户在 SharePoint 网站中存储的文件总数、活动使用的文件数以及在所有这些网站中使用的存储，从 SharePoint 中获取要获取的值的高级别视图。 然后，可深入研究 SharePoint 网站使用情况报表，了解所有网站的趋势和其中每个网站的详细信息。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - SharePoint 网站使用情况](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)。

## <a name="reports"></a>报表

| 函数                                 | CSV 返回类型 | JSON 返回类型                         | 说明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [获取网站详细信息](../api/reportroot-getsharepointsiteusagedetail.md) | Stream          | [sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md) | 获取 SharePoint 网站使用情况的详细信息。 |
| [获取文件数](../api/reportroot-getsharepointsiteusagefilecounts.md) | Stream          | [sharePointSiteUsageFileCounts](../resources/sharepointsiteusagefilecounts.md) | 获取跨所有网站的文件总数和活跃文件数。 如果文件（用户或系统）在指定时间段内被保存、同步、修改或共享，则视为活跃文件（用户或系统）。 |
| [获取网站数](../api/reportroot-getsharepointsiteusagesitecounts.md) | Stream          | [sharePointSiteUsageSiteCounts](../resources/sharepointsiteusagesitecounts.md) | 获取跨所有网站的文件总数和活跃文件数。 如果文件（用户或系统）在指定时间段内被保存、同步、修改或共享，则视为活跃文件（用户或系统）。 |
| [获取存储](../api/reportroot-getsharepointsiteusagestorage.md) | Stream          | [siteUsageStorage](../resources/siteusagestorage.md) | 获取报表周期内分配和使用的存储趋势。 |
| [获取页面数](../api/reportroot-getsharepointsiteusagepages.md) | Stream          | [sharePointSiteUsagePages](../resources/sharepointsiteusagepages.md) | 获取跨所有网站浏览的页面数。 |
