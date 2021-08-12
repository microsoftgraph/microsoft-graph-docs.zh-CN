---
title: Microsoft Teams 用户活动报告
description: 使用 Microsoft Teams 活动报告了解组织中的 Microsoft Teams 用户活动。
localization_priority: Priority
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 48091295d428263c21ddcb5deb694a1b447f41359bdceb4a512fb22a52bc1f5d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178155"
---
# <a name="microsoft-teams-user-activity-reports"></a>Microsoft Teams 用户活动报告

命名空间：microsoft.graph

使用 Microsoft Teams 活动报告了解组织中的 Microsoft Teams 用户活动。

## <a name="methods"></a>方法

| 方法                                   | 返回类型 | 说明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [获取用户详细信息](../api/reportroot-getteamsuseractivityuserdetail.md) | Stream      | 按用户获取有关 Microsoft Teams 用户活动的详细信息。 |
| [获取活动计数](../api/reportroot-getteamsuseractivitycounts.md) | Stream      | 获取按活动类型的 Microsoft Teams 活动的数量。 活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。 |
| [获取用户计数](../api/reportroot-getteamsuseractivityusercounts.md) | Stream      | 按活动类型获取用户数。 活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。 |

