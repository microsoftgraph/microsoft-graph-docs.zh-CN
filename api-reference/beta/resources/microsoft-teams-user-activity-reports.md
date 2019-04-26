---
title: Microsoft Teams 用户活动报告
description: 使用 Microsoft 团队用户活动报告可深入了解组织中的 microsoft 团队用户活动。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: f88d1c9d568ce3fbbf9bfe19abaf637065d37b8c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342203"
---
# <a name="microsoft-teams-user-activity-reports"></a>Microsoft Teams 用户活动报告

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用 Microsoft 团队用户活动报告可深入了解组织中的 microsoft 团队用户活动。

## <a name="methods"></a>方法

| 方法                                   | 返回类型                              | 说明                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [获取用户详细信息](../api/reportroot-getteamsuseractivityuserdetail.md) | [teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md) | 按用户获取有关 Microsoft Teams 用户活动的详细信息。 |
| [获取活动计数](../api/reportroot-getteamsuseractivitycounts.md) | [teamsUserActivityCounts](../resources/teamsuseractivitycounts.md) | 获取按活动类型的 Microsoft Teams 活动的数量。 活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。 |
| [获取用户计数](../api/reportroot-getteamsuseractivityusercounts.md) | [teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md) | 按活动类型获取用户数。 活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。 |
