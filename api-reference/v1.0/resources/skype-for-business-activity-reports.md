---
title: Skype for Business 活动报表
description: Skype for Business 活动报表可用于获取整个组织中活动的详细信息。 这些详细信息有助于为组织调查、计划和制定其他业务决策。
ms.localizationpriority: high
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 486acf1c05eaba43c062d1d7d985c6b42f31ee4f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123011"
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

