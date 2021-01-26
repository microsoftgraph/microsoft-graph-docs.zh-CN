---
title: Microsoft 365 组活动报告
description: 你可以深入了解组织中 Microsoft 365 组的活动，并查看创建和使用的 Microsoft 365 组数。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 0b2f38512ed41fea65f363c8e7ddbef156794fc3
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980764"
---
# <a name="microsoft-365-groups-activity-reports"></a>Microsoft 365 组活动报告

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

你可以深入了解组织中 Microsoft 365 组的活动，并查看创建和使用的 Microsoft 365 组数。

> **注意：** 有关不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报表 - Microsoft 365 组](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)。

## <a name="reports"></a>报告

| 函数                                 | CSV 返回类型 | JSON 返回类型                         | 说明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [获取组详细信息](../api/reportroot-getoffice365groupsactivitydetail.md) | Stream          | [office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md) | 按组获取有关 Microsoft 365 组活动的详细信息。 |
| [获取活动计数](../api/reportroot-getoffice365groupsactivitycounts.md) | Stream          | [office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md) | 获取跨组工作负载的组活动数。 |
| [获取组数](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | Stream          | [office365GroupsActivityGroupCounts](../resources/office365groupsactivitygroupcounts.md) | 获取每日总组数和活跃组数（以电子邮件对话、Yammer 帖子和 SharePoint 文件活动为依据）。 |
| [获取存储](../api/reportroot-getoffice365groupsactivitystorage.md) | Stream          | [office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md) | 获取跨所有组邮箱和组网站使用的总存储。 |
| [获取文件数](../api/reportroot-getoffice365groupsactivityfilecounts.md) | Stream          | [office365GroupsActivityFileCounts](../resources/office365groupsactivityfilecounts.md) | 获取与 Microsoft 365 组关联的所有组网站中的文件总数及其活跃文件数。 |


