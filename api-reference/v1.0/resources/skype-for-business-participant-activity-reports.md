---
title: Skype for Business 参与者活动报表
description: Skype for Business 参与者活动报表可用于获取整个组织中参与会议活动的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: d1dc12c3c2a83808c4168fa19a413f249ef6ba2e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59014340"
---
# <a name="skype-for-business-participant-activity-reports"></a>Skype for Business 参与者活动报表

命名空间：microsoft.graph

Skype for Business 参与者活动报表可用于获取整个组织中参与会议活动的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。

> **注意：** 有关不同报告视图和名称的详细信息，请参阅Microsoft 365 [报告 - Skype for Business会议参与者活动](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b)。

## <a name="reports"></a>报表

| 函数                                 | 返回类型 | 说明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [获取活动数](../api/reportroot-getskypeforbusinessparticipantactivitycounts.md) | Stream      | 获取使用情况趋势，即组织中用户参与的会议会话的次数和类型。 会议会话类型包括 IM、音频/视频、应用共享、Web 和第三方拨入/拨出。 |
| [获取用户数](../api/reportroot-getskypeforbusinessparticipantactivityusercounts.md) | Stream      | 获取使用情况趋势，即组织中用户参与的会议会话的唯一用户数和类型。 会议会话类型包括 IM、音频/视频、应用共享、Web 和第三方拨入/拨出。 |
| [获取分钟数](../api/reportroot-getskypeforbusinessparticipantactivityminutecounts.md) | Stream      | 获取使用情况趋势，即组织中用户参与的会议会话的时长（以分钟为单位）和类型。 会议会话类型包括音频/视频。 |

