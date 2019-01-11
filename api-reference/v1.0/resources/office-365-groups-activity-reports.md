---
title: Office 365 组活动报表
description: 组活动报表可用于深入了解组织中的 Office 365 组活动，并了解正在创建和使用多少个 Office 365 组。
localization_priority: Normal
ms.openlocfilehash: c9f7ae5517cf38f3e290db214a6b2f285dce86f4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832849"
---
# <a name="office-365-groups-activity-reports"></a>Office 365 组活动报表

组活动报表可用于深入了解组织中的 Office 365 组活动，并了解正在创建和使用多少个 Office 365 组。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Office 365 组](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)。

## <a name="reports"></a>报表

| 函数                                 | 返回类型 | 说明                              |
| :--------------------------------------- | :-------------- |  ---------------------------------------- |
| [获取组详细信息](../api/reportroot-getoffice365groupsactivitydetail.md) | Stream          | 获取组执行的 Office 365 组活动的详细信息。 |
| [获取活动数](../api/reportroot-getoffice365groupsactivitycounts.md) | Stream          | 获取跨组工作负载的组活动数。 |
| [获取组数](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | Stream          | 获取每日总组数和活跃组数（以电子邮件对话、Yammer 帖子和 SharePoint 文件活动为依据）。 |
| [获取存储](../api/reportroot-getoffice365groupsactivitystorage.md) | Stream          | 获取跨所有组邮箱和组网站使用的总存储。 |
| [获取文件数](../api/reportroot-getoffice365groupsactivityfilecounts.md) | Stream          | 获取跨与 Office 365 组相关联的所有组网站的文件总数和活跃文件数。 |
