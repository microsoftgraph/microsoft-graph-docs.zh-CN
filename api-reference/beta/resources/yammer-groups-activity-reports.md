---
title: Yammer 组活动报表
description: 您可以深入了解组织中的 yammer 组活动, 并查看正在创建和使用的 yammer 组的数量。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 9035984cf33c56811dc411a6c9cc01e6d438d194
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342788"
---
# <a name="yammer-groups-activity-reports"></a>Yammer 组活动报表

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

您可以深入了解组织中的 yammer 组活动, 并查看正在创建和使用的 yammer 组的数量。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 组活动](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)。

## <a name="reports"></a>报表

| 函数                                 | CSV 返回类型 | JSON 返回类型                         | 说明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [获取组详细信息](../api/reportroot-getyammergroupsactivitydetail.md) | Stream          | [yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md) | 获取组执行的 Yammer 组活动的详细信息。 |
| [获取组数](../api/reportroot-getyammergroupsactivitygroupcounts.md) | Stream          | [yammerGroupsActivityGroupCounts](../resources/yammergroupsactivitygroupcounts.md) | 获取存在的总组数，以及有多少组包含组对话活动。 |
| [获取活动数](../api/reportroot-getyammergroupsactivitycounts.md) | Stream          | [yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md) | 获取组中已发布、已阅读和已赞的 Yammer 消息数。 |
