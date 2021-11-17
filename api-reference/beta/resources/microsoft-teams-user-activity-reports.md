---
title: Microsoft Teams 用户活动报告
description: 使用Microsoft Teams活动报告可深入了解Microsoft Teams活动的用户活动。
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 46ab4747f5ce4e38ab57a56e54528f4c3dfb9360
ms.sourcegitcommit: 42e0e15ff90815e0126c34b928405486cfb1ed86
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/17/2021
ms.locfileid: "61044678"
---
# <a name="microsoft-teams-user-activity-reports"></a>Microsoft Teams 用户活动报告

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用Microsoft Teams活动报告可深入了解Microsoft Teams活动的用户活动。

## <a name="methods"></a>方法

| 方法                                                       | 返回类型 | 说明                                                  |
| :----------------------------------------------------------- | :---------- | :----------------------------------------------------------- |
| [获取用户详细信息](../api/reportroot-getteamsuseractivityuserdetail.md) | Stream      | 按用户获取有关 Microsoft Teams 用户活动的详细信息。     |
| [获取活动计数](../api/reportroot-getteamsuseractivitycounts.md) | Stream      | 获取按活动类型的 Microsoft Teams 活动的数量。 活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。 活动由许可Microsoft Teams执行。 |
| [获取活动总数](../api/reportroot-getteamsuseractivitytotalcounts.md) | Stream      | 获取按活动类型的 Microsoft Teams 活动的数量。 活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。 这些活动由Microsoft Teams或非许可用户执行。 |
| [获取用户数](../api/reportroot-getteamsuseractivityusercounts.md) | Stream      | 按活动类型Microsoft Teams许可用户数。 活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。 |
| [获取用户总数](../api/reportroot-getteamsuseractivitytotalusercounts.md) | Stream      | 按活动类型Microsoft Teams授权或非许可用户的数量。 活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。 |
| [获取分发用户数](../api/reportroot-getteamsuseractivitydistributionusercounts.md) | Stream      | 按活动类型Microsoft Teams许可证用户数。 活动类型包括团队聊天消息、私人聊天消息、通话和会议的数量。 |
| [获取分发用户总数](../api/reportroot-getteamsuseractivitydistributiontotalusercounts.md) | Stream      | 按活动类型Microsoft Teams许可证或非许可用户数。 活动类型包括团队聊天消息、私人聊天消息、通话和会议的数量。 |


