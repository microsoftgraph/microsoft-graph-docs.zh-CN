---
title: SharePoint 网站使用情况报表
description: SharePoint 网站使用情况报表可用于大致了解 SharePoint 带来的价值，具体是以用户在 SharePoint 网站中存储的文件总数、使用的活跃文件数以及跨所有这些网站使用的存储为依据。 然后，可以向下钻取这些报表，了解所有网站的趋势以及每网站级别详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 08de7aff6f96a30632c9b639c7021414f7853663
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034305"
---
# <a name="sharepoint-site-usage-reports"></a>SharePoint 网站使用情况报表

SharePoint 网站使用情况报表可用于大致了解 SharePoint 带来的价值，具体是以用户在 SharePoint 网站中存储的文件总数、使用的活跃文件数以及跨所有这些网站使用的存储为依据。 然后，可以向下钻取这些报表，了解所有网站的趋势以及每网站级别详细信息。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - SharePoint 网站使用情况](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)。

## <a name="reports"></a>报表

| 函数                                 | 返回类型 | 说明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [获取网站详细信息](../api/reportroot-getsharepointsiteusagedetail.md) | 流      | 获取 SharePoint 网站使用情况的详细信息。 |
| [获取文件数](../api/reportroot-getsharepointsiteusagefilecounts.md) | 流      | 获取跨所有网站的文件总数和活跃文件数。 如果文件（用户或系统）在指定时间段内被保存、同步、修改或共享，则视为活跃文件（用户或系统）。 |
| [获取网站数](../api/reportroot-getsharepointsiteusagesitecounts.md) | Stream      | 获取跨所有网站的文件总数和活跃文件数。 如果文件（用户或系统）在指定时间段内被保存、同步、修改或共享，则视为活跃文件（用户或系统）。 |
| [获取存储](../api/reportroot-getsharepointsiteusagestorage.md) | Stream      | 获取报表周期内分配和使用的存储趋势。 |
| [获取页面数](../api/reportroot-getsharepointsiteusagepages.md) | Stream      | 获取跨所有网站浏览的页面数。 |
