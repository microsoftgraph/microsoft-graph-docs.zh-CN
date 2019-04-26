---
title: SharePoint 活动报表
description: 您可以通过查看用户与文件的交互来获取使用 SharePoint 的每个用户的活动。 也可以查看以共享文件数为依据的协作级别。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: cfe8c698533b46d4edbbb724dc5fb993cc85cfdb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343162"
---
# <a name="sharepoint-activity-reports"></a>SharePoint 活动报表

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

您可以通过查看用户与文件的交互来获取使用 SharePoint 的每个用户的活动。 也可以查看以共享文件数为依据的协作级别。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - SharePoint 活动](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)。

## <a name="reports"></a>报表

| 函数                                 | CSV 返回类型 | JSON 返回类型                         | 说明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [获取用户详细信息](../api/reportroot-getsharepointactivityuserdetail.md) | Stream          | [sharePointActivityUserDetail](../resources/sharepointactivityuserdetail.md) | 获取用户执行的 SharePoint 活动的详细信息。 |
| [获取文件数](../api/reportroot-getsharepointactivityfilecounts.md) | Stream          | [siteActivitySummary](../resources/siteactivitysummary.md) | 获取与 SharePoint 网站中存储的文件进行交互的唯一许可用户数。 |
| [获取用户数](../api/reportroot-getsharepointactivityusercounts.md) | Stream          | [sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md) | 获取活跃用户数趋势。 如果用户执行了文件活动（保存、同步、修改或共享）或在指定时间内访问了页面，则视为活跃用户。 |
| [获取页面数](../api/reportroot-getsharepointactivitypages.md) | Stream          | [sharePointActivityPages](../resources/sharepointactivitypages.md) | 获取用户访问的唯一页面数。 |
