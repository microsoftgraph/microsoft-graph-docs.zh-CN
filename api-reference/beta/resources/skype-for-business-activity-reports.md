---
title: Skype for Business 活动报表
description: 你可以获取有关整个组织活动的详细信息。 这些详细信息有助于为组织调查、计划和制定其他业务决策。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 0fe3236fc8c4f29357e2ae3fae45c80969c353db
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980645"
---
# <a name="skype-for-business-activity-reports"></a>Skype for Business 活动报告

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

你可以获取有关整个组织活动的详细信息。 这些详细信息有助于为组织调查、计划和制定其他业务决策。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅 [Microsoft 365 报表 - Skype for Business 活动](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)。

## <a name="reports"></a>报告

| 函数                                 | CSV 返回类型 | JSON 返回类型                         | 说明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [获取用户详细信息](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | Stream          | [skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md) | 获取用户执行的 Skype for Business 活动的详细信息。 |
| [获取活动数](../api/reportroot-getskypeforbusinessactivitycounts.md) | Stream          | [skypeForBusinessActivityCounts](../resources/skypeforbusinessactivitycounts.md) | 获取通过 Skype for Business 组织并参与在组织中召开的会议会话的用户数趋势。 报表还包含对等会话数。 |
| [获取用户数](../api/reportroot-getskypeforbusinessactivityusercounts.md) | Stream          | [skypeForBusinessActivityUserCounts](../resources/skypeforbusinessactivityusercounts.md) | 获取通过 Skype for Business 组织并参与在组织中召开的会议会话的唯一用户数趋势。 报表还包含对等会话数。 |


