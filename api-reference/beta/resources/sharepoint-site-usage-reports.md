---
title: SharePoint 网站使用情况报表
description: 您可以获取从 SharePoint 获取的值的高级别视图，包括用户在 SharePoint 网站中存储的文件总数、当前使用的文件数以及所有这些网站中使用的存储。 然后，你可以向下钻取 SharePoint 网站使用情况报告，了解所有网站的趋势和每个网站级别的详细信息。
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: dd0f57a197981ee41b887c824eddcbcf3a2b3814
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2021
ms.locfileid: "61390785"
---
# <a name="sharepoint-site-usage-reports"></a>SharePoint 网站使用情况报表

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

您可以获取从 SharePoint 获取的值的高级别视图，包括用户在 SharePoint 网站中存储的文件总数、当前使用的文件数以及所有这些网站中使用的存储。 然后，你可以向下钻取 SharePoint 网站使用情况报告，了解所有网站的趋势和每个网站级别的详细信息。

> **注意：** 有关不同报告视图和名称的详细信息，请参阅Microsoft 365 [报告 -](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)SharePoint使用率。

## <a name="reports"></a>报告

| 函数                                                     | CSV 返回类型 | JSON 返回类型 | 说明                                                  |
| :----------------------------------------------------------- | :-------------- | :--------------- | ------------------------------------------------------------ |
| [获取网站详细信息](../api/reportroot-getsharepointsiteusagedetail.md) | Stream          | Stream           | 获取 SharePoint 网站使用情况的详细信息。                     |
| [获取文件数](../api/reportroot-getsharepointsiteusagefilecounts.md) | Stream          | Stream           | 获取跨所有网站的文件总数和活跃文件数。 如果文件（用户或系统）在指定时间段内被保存、同步、修改或共享，则视为活跃文件（用户或系统）。 |
| [获取网站数](../api/reportroot-getsharepointsiteusagesitecounts.md) | Stream          | Stream           | 获取跨所有网站的文件总数和活跃文件数。 如果文件（用户或系统）在指定时间段内被保存、同步、修改或共享，则视为活跃文件（用户或系统）。 |
| [获取存储](../api/reportroot-getsharepointsiteusagestorage.md) | Stream          | Stream           | 获取报表周期内分配和使用的存储趋势。 |
| [获取页面数](../api/reportroot-getsharepointsiteusagepages.md) | Stream          | Stream           | 获取跨所有网站浏览的页面数。             |


