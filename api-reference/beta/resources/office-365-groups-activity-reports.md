---
title: Microsoft 365 组活动报告
description: 您可以深入了解组织中的 Microsoft 365 组活动，并查看创建和使用了多少个 Microsoft 365 组。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 0b2a4fbb3a95f816ef730bcc16f2742a70160de0
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896810"
---
# <a name="microsoft-365-groups-activity-reports"></a>Microsoft 365 组活动报告

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

您可以深入了解组织中的 Microsoft 365 组活动，并查看创建和使用了多少个 Microsoft 365 组。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅[microsoft 365 报表-microsoft 365 组](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)。

## <a name="reports"></a>报表

| 函数                                 | CSV 返回类型 | JSON 返回类型                         | 说明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [获取组详细信息](../api/reportroot-getoffice365groupsactivitydetail.md) | Stream          | [office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md) | 按组获取有关 Microsoft 365 组活动的详细信息。 |
| [获取活动数](../api/reportroot-getoffice365groupsactivitycounts.md) | Stream          | [office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md) | 获取跨组工作负载的组活动数。 |
| [获取组数](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | Stream          | [office365GroupsActivityGroupCounts](../resources/office365groupsactivitygroupcounts.md) | 获取每日总组数和活跃组数（以电子邮件对话、Yammer 帖子和 SharePoint 文件活动为依据）。 |
| [获取存储](../api/reportroot-getoffice365groupsactivitystorage.md) | Stream          | [office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md) | 获取跨所有组邮箱和组网站使用的总存储。 |
| [获取文件数](../api/reportroot-getoffice365groupsactivityfilecounts.md) | Stream          | [office365GroupsActivityFileCounts](../resources/office365groupsactivityfilecounts.md) | 获取总文件数以及与 Microsoft 365 组关联的所有组网站中有多少个处于活动状态的文件。 |
