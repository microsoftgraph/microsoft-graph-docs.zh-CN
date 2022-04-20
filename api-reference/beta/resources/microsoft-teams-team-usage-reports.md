---
title: Microsoft Teams团队使用情况报告
description: 使用Microsoft Teams团队使用情况报告来深入了解组织中团队的使用情况。
ms.localizationpriority: medium
ms.prod: reports
author: zhiliqiao
doc_type: conceptualPageType
ms.openlocfilehash: df580adb2234902cf9093714fd4e627f67581491
ms.sourcegitcommit: 9bbcce5784a89768ece55a66e3651080d56e1e92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/19/2022
ms.locfileid: "64917854"
---
# <a name="microsoft-teams-team-usage-reports"></a>Microsoft Teams团队使用情况报告

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用Microsoft Teams团队使用情况报告来深入了解组织中团队的使用情况。

## <a name="reports"></a>报表

| 函数 | CSV 返回类型 | JSON 返回类型 | 说明 |
| :--------------------------------------- | --------------- | ---------------------------------------- | ---------------------------------------- |
| [获取团队详细信息](../api/reportroot-getteamsteamactivitydetail.md) | Stream | Stream | 按团队获取有关Teams活动的详细信息。 这些数字包括许可用户和非许可用户的活动。 |
| [获取团队计数](../api/reportroot-getteamsteamactivitycounts.md) | Stream | Stream | 获取跨Microsoft Teams的团队活动数。 活动类型与会议和消息相关。 |
| [获取分发团队计数](../api/reportroot-getteamsteamactivitydistributioncounts.md) | Stream | Stream | 获取所选时间段内跨Microsoft Teams的团队活动数。 |


