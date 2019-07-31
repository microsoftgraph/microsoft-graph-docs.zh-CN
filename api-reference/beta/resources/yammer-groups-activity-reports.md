---
title: Yammer 组活动报表
description: 您可以深入了解组织中的 Yammer 组活动, 并查看正在创建和使用的 Yammer 组的数量。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 07a78a4b2047e03beee611443240f56739f76b4f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963836"
---
# <a name="yammer-groups-activity-reports"></a>Yammer 组活动报表

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

您可以深入了解组织中的 Yammer 组活动, 并查看正在创建和使用的 Yammer 组的数量。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 组活动](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)。

## <a name="reports"></a>报表

| 函数                                 | CSV 返回类型 | JSON 返回类型                         | 说明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [获取组详细信息](../api/reportroot-getyammergroupsactivitydetail.md) | 流          | [yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md) | 获取组执行的 Yammer 组活动的详细信息。 |
| [获取组数](../api/reportroot-getyammergroupsactivitygroupcounts.md) | Stream          | [yammerGroupsActivityGroupCounts](../resources/yammergroupsactivitygroupcounts.md) | 获取存在的总组数，以及有多少组包含组对话活动。 |
| [获取活动数](../api/reportroot-getyammergroupsactivitycounts.md) | Stream          | [yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md) | 获取组中已发布、已阅读和已赞的 Yammer 消息数。 |
