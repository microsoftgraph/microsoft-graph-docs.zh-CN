---
title: Microsoft Teams 用户活动报告
description: 使用 Microsoft Teams 用户活动报告深入了解您组织的 Microsoft Teams 用户活动。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: e249998d8c4481c7e3ef0b2fe31072fe59c84378
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980787"
---
# <a name="microsoft-teams-user-activity-reports"></a>Microsoft Teams 用户活动报告

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用 Microsoft Teams 用户活动报告深入了解您组织的 Microsoft Teams 用户活动。

## <a name="methods"></a>方法

| 方法                                   | 返回类型                              | 说明                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [获取用户详细信息](../api/reportroot-getteamsuseractivityuserdetail.md) | [teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md) | 按用户获取有关 Microsoft Teams 用户活动的详细信息。 |
| [获取活动计数](../api/reportroot-getteamsuseractivitycounts.md) | [teamsUserActivityCounts](../resources/teamsuseractivitycounts.md) | 获取按活动类型的 Microsoft Teams 活动的数量。 活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。 |
| [获取用户计数](../api/reportroot-getteamsuseractivityusercounts.md) | [teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md) | 按活动类型获取用户数。 活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。 |


