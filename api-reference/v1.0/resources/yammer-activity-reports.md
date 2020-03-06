---
title: Yammer 活动报表
description: Yammer 活动报表可用于了解组织的 Yammer 交互级别，具体是以整个组织中生成的活动数以及在 Yammer 上发布、赞和阅读消息的唯一用户数为依据。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: b6f92ba4745d69cf2ce341412eee88403218414c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533357"
---
# <a name="yammer-activity-reports"></a>Yammer 活动报表

命名空间：microsoft.graph

Yammer 活动报表可用于了解组织的 Yammer 交互级别，具体是以整个组织中生成的活动数以及在 Yammer 上发布、赞和阅读消息的唯一用户数为依据。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 活动](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)。

## <a name="reports"></a>报表

| 函数                                 | 返回类型 | 说明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [获取用户详细信息](../api/reportroot-getyammeractivityuserdetail.md) | Stream      | 获取用户执行的 Yammer 活动的详细信息。 |
| [获取活动计数](../api/reportroot-getyammeractivitycounts.md) | Stream      | 获取组织中的 Yammer 活动数趋势，具体是以已发布、已阅读和已赞的消息数为依据。 |
| [获取用户计数](../api/reportroot-getyammeractivityusercounts.md) | Stream      | 获取已发布、已阅读和已赞 Yammer 消息的唯一用户数趋势。 |
