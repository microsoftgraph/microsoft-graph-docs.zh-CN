---
title: Skype for Business 参与者活动报表
description: Skype for Business 参与者活动报表可用于获取整个组织中参与会议活动的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: bffdfd100ef1b9e8367ace26dff54d2cec20b5ac
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533651"
---
# <a name="skype-for-business-participant-activity-reports"></a>Skype for Business 参与者活动报表

命名空间：microsoft.graph

Skype for Business 参与者活动报表可用于获取整个组织中参与会议活动的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 会议参与者活动](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b)。

## <a name="reports"></a>报表

| 函数                                 | 返回类型 | 说明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [获取活动计数](../api/reportroot-getskypeforbusinessparticipantactivitycounts.md) | Stream      | 获取使用情况趋势，即组织中用户参与的会议会话的次数和类型。 会议会话类型包括 IM、音频/视频、应用共享、Web 和第三方拨入/拨出。 |
| [获取用户计数](../api/reportroot-getskypeforbusinessparticipantactivityusercounts.md) | Stream      | 获取使用情况趋势，即组织中用户参与的会议会话的唯一用户数和类型。 会议会话类型包括 IM、音频/视频、应用共享、Web 和第三方拨入/拨出。 |
| [获取分钟数](../api/reportroot-getskypeforbusinessparticipantactivityminutecounts.md) | Stream      | 获取使用情况趋势，即组织中用户参与的会议会话的时长（以分钟为单位）和类型。 会议会话类型包括音频/视频。 |
