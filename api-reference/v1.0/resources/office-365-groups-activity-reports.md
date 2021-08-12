---
title: Microsoft 365组活动报告
description: 可以使用组活动报告深入了解组织中 Microsoft 365 组的活动，并查看创建和使用Microsoft 365组数。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 814b66d419fea4d06cbf16158298fac81c644ba794f3c0f85a8c32e2996d776f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54174918"
---
# <a name="microsoft-365-groups-activity-reports"></a>Microsoft 365组活动报告

命名空间：microsoft.graph

可以使用组活动报告深入了解组织中 Microsoft 365 组的活动，并查看创建和使用Microsoft 365组数。

> **注意：** 有关不同报表视图和名称的详细信息，请参阅Microsoft 365 [报告 -](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)Microsoft 365组。

## <a name="reports"></a>报表

| 函数                                 | 返回类型 | 说明                              |
| :--------------------------------------- | :-------------- |  ---------------------------------------- |
| [获取组详细信息](../api/reportroot-getoffice365groupsactivitydetail.md) | Stream          | 获取有关按组Microsoft 365组活动的详细信息。 |
| [获取活动数](../api/reportroot-getoffice365groupsactivitycounts.md) | Stream          | 获取跨组工作负载的组活动数。 |
| [获取组数](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | Stream          | 获取每日总组数和活跃组数（以电子邮件对话、Yammer 帖子和 SharePoint 文件活动为依据）。 |
| [获取存储](../api/reportroot-getoffice365groupsactivitystorage.md) | Stream          | 获取跨所有组邮箱和组网站使用的总存储。 |
| [获取文件数](../api/reportroot-getoffice365groupsactivityfilecounts.md) | Stream          | 获取与组关联的所有组网站中的文件总数及其Microsoft 365数量。 |

