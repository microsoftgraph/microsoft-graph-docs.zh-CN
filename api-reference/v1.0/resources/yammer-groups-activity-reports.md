---
title: Yammer 组活动报表
description: Yammer 组活动报表可用于深入了解组织中的 Yammer 组活动，并了解正在创建和使用多少个 Yammer 组。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 961072e088d36748d51a4a6081f0ee06c47b6e20
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534265"
---
# <a name="yammer-groups-activity-reports"></a>Yammer 组活动报表

命名空间：microsoft.graph

Yammer 组活动报表可用于深入了解组织中的 Yammer 组活动，并了解正在创建和使用多少个 Yammer 组。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 组活动](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)。

## <a name="reports"></a>报表

| 函数                                 | 返回类型 | 说明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [获取组详细信息](../api/reportroot-getyammergroupsactivitydetail.md) | Stream      | 获取组执行的 Yammer 组活动的详细信息。 |
| [获取组数](../api/reportroot-getyammergroupsactivitygroupcounts.md) | Stream      | 获取存在的总组数，以及有多少组包含组对话活动。 |
| [获取活动计数](../api/reportroot-getyammergroupsactivitycounts.md) | Stream      | 获取组中已发布、已阅读和已赞的 Yammer 消息数。 |
