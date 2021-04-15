---
title: Microsoft Teams 用户活动报告
description: 使用 Microsoft Teams 用户活动报告可深入了解贵组织的 Microsoft Teams 用户活动。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 97a32ce99eab154a99a97d9c9dab7fc49d4a7a1d
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766117"
---
# <a name="microsoft-teams-user-activity-reports"></a>Microsoft Teams 用户活动报告

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用 Microsoft Teams 用户活动报告可深入了解贵组织的 Microsoft Teams 用户活动。

## <a name="methods"></a>方法

| 方法                                                       | 返回类型                                                  | 说明                                                  |
| :----------------------------------------------------------- | :----------------------------------------------------------- | :----------------------------------------------------------- |
| [获取用户详细信息](../api/reportroot-getteamsuseractivityuserdetail.md) | [teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md) | 按用户获取有关 Microsoft Teams 用户活动的详细信息。     |
| [获取活动计数](../api/reportroot-getteamsuseractivitycounts.md) | [teamsUserActivityCounts](../resources/teamsuseractivitycounts.md) | 获取按活动类型的 Microsoft Teams 活动的数量。 活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。 这些活动由 Microsoft Teams 许可用户执行。 |
| [获取活动总数](../api/reportroot-getteamsuseractivitytotalcounts.md) | [teamsUserActivityCounts](../resources/teamsuseractivitycounts.md) | 获取按活动类型的 Microsoft Teams 活动的数量。 活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。 这些活动由 Microsoft Teams 授权用户或非许可用户执行。 |
| [获取用户数](../api/reportroot-getteamsuseractivityusercounts.md) | [teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md) | 按活动类型获取 Microsoft Teams 许可用户的数量。 活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。 |
| [获取用户总数](../api/reportroot-getteamsuseractivitytotalusercounts.md) | [teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md) | 按活动类型获取 Microsoft Teams 许可或非许可用户的数量。 活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。 |
| [获取分发用户数](../api/reportroot-getteamsuseractivitydistributionusercounts.md) | [teamsUserActivityDistributionUserCounts](../resources/teamsuseractivitydistributionusercounts.md) | 按活动类型获取选定时段内 Microsoft Teams 许可用户的数量。 活动类型包括团队聊天消息、私人聊天消息、通话和会议的数量。 |
| [获取分发用户总数](../api/reportroot-getteamsuseractivitydistributiontotalusercounts.md) | [teamsUserActivityDistributionUserCounts](../resources/teamsuseractivitydistributionusercounts.md) | 按活动类型获取选定时段内 Microsoft Teams 许可或非许可用户的数量。 活动类型包括团队聊天消息、私人聊天消息、通话和会议的数量。 |


