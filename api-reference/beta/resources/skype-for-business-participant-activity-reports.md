---
title: Skype for Business 参与者活动报表
description: 你可以在组织中获取有关会议活动的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 0701a31db5a1c57e67efba477a5f2d0c6d47b5e9
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897986"
---
# <a name="skype-for-business-participant-activity-reports"></a>Skype for Business 参与者活动报表

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

你可以在组织中获取有关会议活动的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅[Microsoft 365 reports-Skype For business 会议参与者活动](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b)。

## <a name="reports"></a>报表

| 函数                                 | CSV 返回类型 | JSON 返回类型                         | 说明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [获取活动数](../api/reportroot-getskypeforbusinessparticipantactivitycounts.md) | Stream          | [skypeForBusinessParticipantActivityCounts](../resources/skypeforbusinessparticipantactivitycounts.md) | 获取使用情况趋势，即组织中用户参与的会议会话的次数和类型。 会议会话类型包括 IM、音频/视频、应用共享、Web 和第三方拨入/拨出。 |
| [获取用户数](../api/reportroot-getskypeforbusinessparticipantactivityusercounts.md) | Stream          | [skypeForBusinessParticipantActivityUserCounts](../resources/skypeforbusinessparticipantactivityusercounts.md) | 获取使用情况趋势，即组织中用户参与的会议会话的唯一用户数和类型。 会议会话类型包括 IM、音频/视频、应用共享、Web 和第三方拨入/拨出。 |
| [获取分钟数](../api/reportroot-getskypeforbusinessparticipantactivityminutecounts.md) | Stream          | [skypeForBusinessParticipantActivityMinuteCounts](../resources/skypeforbusinessparticipantactivityminutecounts.md) | 获取使用情况趋势，即组织中用户参与的会议会话的时长（以分钟为单位）和类型。 会议会话类型包括音频/视频。 |
