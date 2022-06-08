---
title: Microsoft Teams 用户活动报告
description: 使用 Microsoft Teams 活动报告了解组织中的 Microsoft Teams 用户活动。
ms.localizationpriority: high
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: a2c61edbc5e8df05fb47eca2f34dfb2b84606c9b
ms.sourcegitcommit: 69b150e408c0b9a0705bf33229269f6e5371bc6c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/07/2022
ms.locfileid: "65923965"
---
# <a name="microsoft-teams-user-activity-reports"></a>Microsoft Teams 用户活动报告

命名空间：microsoft.graph

使用 Microsoft Teams 活动报告了解组织中的 Microsoft Teams 用户活动。

## <a name="methods"></a>方法

| 方法                                   | 返回类型 | 说明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [获取用户详细信息](../api/reportroot-getteamsuseractivityuserdetail.md) | Stream      | 按用户获取有关 Microsoft Teams 用户活动的详细信息。 |
| [获取活动计数](../api/reportroot-getteamsuseractivitycounts.md) | Stream      | 获取按活动类型的 Microsoft Teams 活动的数量。 这些活动由 Microsoft Teams 许可的用户执行。 |
| [获取用户数](../api/reportroot-getteamsuseractivityusercounts.md) | Stream      | 按活动类型获取用户数。 活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。 |

