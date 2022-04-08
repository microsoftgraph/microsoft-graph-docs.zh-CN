---
title: Microsoft Teams 用户活动报告
description: 使用Microsoft Teams用户活动报告深入了解组织中的Microsoft Teams用户活动。
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: d49f7c0ebccbc70f10460673d73aab3794283195
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704231"
---
# <a name="microsoft-teams-user-activity-reports"></a>Microsoft Teams 用户活动报告

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用Microsoft Teams用户活动报告深入了解组织中的Microsoft Teams用户活动。

## <a name="methods"></a>Methods

| 方法                                                       | 返回类型 | 说明                                                  |
| :----------------------------------------------------------- | :---------- | :----------------------------------------------------------- |
| [获取用户详细信息](../api/reportroot-getteamsuseractivityuserdetail.md) | Stream      | 按用户获取有关 Microsoft Teams 用户活动的详细信息。     |
| [获取活动计数](../api/reportroot-getteamsuseractivitycounts.md) | Stream      | 获取按活动类型的 Microsoft Teams 活动的数量。 活动由Microsoft Teams许可用户执行。 |
| [获取活动总计计数](../api/reportroot-getteamsuseractivitytotalcounts.md) | Stream      | 获取按活动类型的 Microsoft Teams 活动的数量。 这些活动由Microsoft Teams许可或未经许可的用户执行。 |
| [获取用户数](../api/reportroot-getteamsuseractivityusercounts.md) | Stream      | 按活动类型获取Microsoft Teams许可用户的数量。 活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。 |
| [获取用户总数](../api/reportroot-getteamsuseractivitytotalusercounts.md) | Stream      | 按活动类型获取Microsoft Teams许可或未经许可的用户数。 活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。 |
| [获取分发用户数](../api/reportroot-getteamsuseractivitydistributionusercounts.md) | Stream      | 按活动类型获取所选时间段内Microsoft Teams许可用户的数量。 活动类型为团队聊天消息、私人聊天消息、呼叫和会议的数量。 |
| [获取分发总用户计数](../api/reportroot-getteamsuseractivitydistributiontotalusercounts.md) | Stream      | 按所选时间段内的活动类型获取Microsoft Teams许可或非许可用户的数量。 活动类型为团队聊天消息、私人聊天消息、呼叫和会议的数量。 |
| [获取总分布活动计数](../api/reportroot-getteamsuseractivitytotaldistributioncounts.md) | Stream      | 获取所选时间段内Microsoft Teams用户活动的数量。 活动类型为团队聊天消息、私人聊天消息、呼叫、会议、组织会议、参加会议、音频持续时间、视频持续时间、屏幕共享持续时间、邮件发布和回复消息。 |

