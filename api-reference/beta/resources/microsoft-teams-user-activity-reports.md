---
title: Microsoft Teams 用户活动报告
description: 使用 Microsoft 团队用户活动报告您的组织中获取的 Microsoft 团队用户活动见解。
ms.openlocfilehash: 26af58ad88541fb4e9e0f64159505846bfe90bb5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042383"
---
# <a name="microsoft-teams-user-activity-reports"></a>Microsoft Teams 用户活动报告

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。 在 Microsoft Graph 中国由 21Vianet 不支持这些 Api。

使用 Microsoft 团队用户活动报告您的组织中获取的 Microsoft 团队用户活动见解。

## <a name="methods"></a>方法

| 方法                                   | 返回类型                              | 说明                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [获取用户详细信息](../api/reportroot-getteamsuseractivityuserdetail.md) | [teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md) | 按用户获取有关 Microsoft Teams 用户活动的详细信息。 |
| [获取活动计数](../api/reportroot-getteamsuseractivitycounts.md) | [teamsUserActivityCounts](../resources/teamsuseractivitycounts.md) | 获取按活动类型的 Microsoft Teams 活动的数量。 活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。 |
| [获取用户计数](../api/reportroot-getteamsuseractivityusercounts.md) | [teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md) | 按活动类型获取用户数。 活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。 |
