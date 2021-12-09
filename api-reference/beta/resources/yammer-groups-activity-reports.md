---
title: Yammer 组活动报表
description: 你可以深入了解组织中Yammer组的活动，并查看创建Yammer组数。
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 6afb080020f5a9032f26a34c8b91433db2b8e034
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2021
ms.locfileid: "61390653"
---
# <a name="yammer-groups-activity-reports"></a>Yammer 组活动报表

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

你可以深入了解组织中Yammer组的活动，并查看创建Yammer组数。

> **注意：** 有关不同报表视图和名称的详细信息，请参阅 Microsoft 365 [reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)。

## <a name="reports"></a>报告

| 函数                                                     | CSV 返回类型 | JSON 返回类型 | 说明                                                  |
| :----------------------------------------------------------- | :-------------- | :--------------- | ------------------------------------------------------------ |
| [获取组详细信息](../api/reportroot-getyammergroupsactivitydetail.md) | Stream          | Stream           | 获取组执行的 Yammer 组活动的详细信息。           |
| [获取组数](../api/reportroot-getyammergroupsactivitygroupcounts.md) | Stream          | Stream           | 获取存在的总组数，以及有多少组包含组对话活动。 |
| [获取活动数](../api/reportroot-getyammergroupsactivitycounts.md) | Stream          | Stream           | 获取组中已发布、已阅读和已赞的 Yammer 消息数。 |


