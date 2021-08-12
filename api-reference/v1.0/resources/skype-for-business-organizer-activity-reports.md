---
title: Skype for Business 组织者活动报表
description: Skype for Business 组织者活动报表可用于获取整个组织中组织会议活动的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: c458d6b720e92473841edc54a2c2ca5cca028e6ba62b30756885a3cdca8e06f8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54235252"
---
# <a name="skype-for-business-organizer-activity-reports"></a>Skype for Business 组织者活动报表

命名空间：microsoft.graph

Skype for Business 组织者活动报表可用于获取整个组织中组织会议活动的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。

> **注意：** 有关不同报告视图和名称的详细信息，请参阅Microsoft 365 [报告 - Skype for Business会议组织者活动](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254)。

## <a name="reports"></a>报表

| 函数                                 | 返回类型 | 说明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [获取活动数](../api/reportroot-getskypeforbusinessorganizeractivitycounts.md) | Stream      | 获取使用情况趋势，即组织中用户召开和组织的会议会话的次数和类型。 会议会话类型包括 IM、音频/视频、应用共享、Web、第三方拨入/拨出和 Microsoft 拨入/拨出。 |
| [获取用户数](../api/reportroot-getskypeforbusinessorganizeractivityusercounts.md) | Stream      | 获取使用情况趋势，即组织中用户召开和组织的会议会话的唯一用户数和类型。 会议会话类型包括 IM、音频/视频、应用共享、Web、第三方拨入/拨出和 Microsoft 拨入/拨出。 |
| [获取分钟数](../api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md) | Stream      | 获取使用情况趋势，即组织中用户召开和组织的会议会话的时长（以分钟为单位）和类型。 会议会话类型包括音频/视频和 Microsoft 拨入/拨出。 |

