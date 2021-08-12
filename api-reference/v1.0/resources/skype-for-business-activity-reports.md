---
title: Skype for Business 活动报表
description: Skype for Business 活动报表可用于获取整个组织中活动的详细信息。 这些详细信息有助于为组织调查、计划和制定其他业务决策。
localization_priority: Priority
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 4b7f5c244fec894feb0cb7708e5b373019b1d7e90daadf4e46b899f61ed09848
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54202124"
---
# <a name="skype-for-business-activity-reports"></a>Skype for Business 活动报告

命名空间：microsoft.graph

Skype for Business 活动报表可用于获取整个组织中活动的详细信息。 这些详细信息有助于为组织调查、计划和制定其他业务决策。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅 [Microsoft 365 报表 - Skype for Business 活动](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)。

## <a name="reports"></a>报告

| 函数                                 | 返回类型 | 说明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [获取用户详细信息](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | Stream      | 获取用户执行的 Skype for Business 活动的详细信息。 |
| [获取活动数](../api/reportroot-getskypeforbusinessactivitycounts.md) | Stream      | 获取通过 Skype for Business 组织并参与在组织中召开的会议会话的用户数趋势。报表还包含对等会话数。 |
| [获取用户数](../api/reportroot-getskypeforbusinessactivityusercounts.md) | Stream      | 获取通过 Skype for Business 组织并参与在组织中召开的会议会话的唯一用户数趋势。报表还包含对等会话数。 |

