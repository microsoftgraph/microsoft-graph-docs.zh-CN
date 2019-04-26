---
title: Office 365 组活动报表
description: 您可以深入了解组织中的 office 365 组的活动, 并查看创建和使用了多少个 office 365 组。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: a46e1823acd63616f10ce2569a72a0099e390f93
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342007"
---
# <a name="office-365-groups-activity-reports"></a>Office 365 组活动报表

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

您可以深入了解组织中的 office 365 组的活动, 并查看创建和使用了多少个 office 365 组。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Office 365 组](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)。

## <a name="reports"></a>报表

| 函数                                 | CSV 返回类型 | JSON 返回类型                         | 说明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [获取组详细信息](../api/reportroot-getoffice365groupsactivitydetail.md) | Stream          | [office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md) | 获取组执行的 Office 365 组活动的详细信息。 |
| [获取活动数](../api/reportroot-getoffice365groupsactivitycounts.md) | Stream          | [office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md) | 获取跨组工作负载的组活动数。 |
| [获取组数](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | Stream          | [office365GroupsActivityGroupCounts](../resources/office365groupsactivitygroupcounts.md) | 获取每日总组数和活跃组数（以电子邮件对话、Yammer 帖子和 SharePoint 文件活动为依据）。 |
| [获取存储](../api/reportroot-getoffice365groupsactivitystorage.md) | Stream          | [office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md) | 获取跨所有组邮箱和组网站使用的总存储。 |
| [获取文件数](../api/reportroot-getoffice365groupsactivityfilecounts.md) | Stream          | [office365GroupsActivityFileCounts](../resources/office365groupsactivityfilecounts.md) | 获取跨与 Office 365 组相关联的所有组网站的文件总数和活跃文件数。 |
