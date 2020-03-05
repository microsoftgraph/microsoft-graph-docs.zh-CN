---
title: Yammer 活动报表
description: 您可以通过在组织中生成多少活动以及在 Yammer 上进行 post （如和阅读邮件）的唯一用户的数量来了解您的组织对 Yammer 的服务级别。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 8f1358c188b06953d7af180c2b7ad83b6183af35
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519055"
---
# <a name="yammer-activity-reports"></a>Yammer 活动报表

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

您可以通过在组织中生成多少活动以及在 Yammer 上进行 post （如和阅读邮件）的唯一用户的数量来了解您的组织对 Yammer 的服务级别。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 活动](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)。

## <a name="reports"></a>报表

| 函数                                 | CSV 返回类型 | JSON 返回类型                         | 说明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [获取用户详细信息](../api/reportroot-getyammeractivityuserdetail.md) | Stream          | [yammerActivityUserDetail](../resources/yammeractivityuserdetail.md) | 获取用户执行的 Yammer 活动的详细信息。 |
| [获取活动数](../api/reportroot-getyammeractivitycounts.md) | Stream          | [yammerActivitySummary](../resources/yammeractivitysummary.md) | 获取组织中的 Yammer 活动数趋势，具体是以已发布、已阅读和已赞的消息数为依据。 |
| [获取用户数](../api/reportroot-getyammeractivityusercounts.md) | Stream          | [yammerActivitySummary](../resources/yammeractivitysummary.md) | 获取已发布、已阅读和已赞 Yammer 消息的唯一用户数趋势。 |
