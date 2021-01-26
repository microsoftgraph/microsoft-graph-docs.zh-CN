---
title: Microsoft 365 组活动报告
description: 可以使用组活动报告深入了解组织中 Microsoft 365 组的活动，并查看正在创建和使用多少个 Microsoft 365 组。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 7470eff43c2c77a63206cf24e0484360bf3371b6
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980995"
---
# <a name="microsoft-365-groups-activity-reports"></a>Microsoft 365 组活动报告

命名空间：microsoft.graph

可以使用组活动报告深入了解组织中 Microsoft 365 组的活动，并查看正在创建和使用多少个 Microsoft 365 组。

> **注意：** 有关不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报表 - Microsoft 365 组](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)。

## <a name="reports"></a>报告

| 函数                                 | 返回类型 | 说明                              |
| :--------------------------------------- | :-------------- |  ---------------------------------------- |
| [获取组详细信息](../api/reportroot-getoffice365groupsactivitydetail.md) | Stream          | 按组获取有关 Microsoft 365 组活动的详细信息。 |
| [获取活动计数](../api/reportroot-getoffice365groupsactivitycounts.md) | Stream          | 获取跨组工作负载的组活动数。 |
| [获取组数](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | Stream          | 获取每日总组数和活跃组数（以电子邮件对话、Yammer 帖子和 SharePoint 文件活动为依据）。 |
| [获取存储](../api/reportroot-getoffice365groupsactivitystorage.md) | Stream          | 获取跨所有组邮箱和组网站使用的总存储。 |
| [获取文件数](../api/reportroot-getoffice365groupsactivityfilecounts.md) | Stream          | 获取与 Microsoft 365 组关联的所有组网站中的文件总数及其活跃文件数。 |

