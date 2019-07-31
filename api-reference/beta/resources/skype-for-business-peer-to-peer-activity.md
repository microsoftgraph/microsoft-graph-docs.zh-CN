---
title: Skype for Business 对等活动报表
description: 你可以在组织中获取对等活动的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 60f8e5c5878822eaae64d5f10d0ff52dd4bc004f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964985"
---
# <a name="skype-for-business-peer-to-peer-activity-reports"></a>Skype for Business 对等活动报表

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

你可以在组织中获取对等活动的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 对等活动](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713)。

## <a name="reports"></a>报表

| 函数                                 | CSV 返回类型 | JSON 返回类型                         | 说明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [获取活动数](../api/reportroot-getskypeforbusinesspeertopeeractivitycounts.md) | 流          | [skypeForBusinessPeerToPeerActivityCounts](../resources/skypeforbusinesspeertopeeractivitycounts.md) | 获取使用情况趋势，即组织中召开的会话的次数和类型。 会话类型包括 IM、音频、视频、应用共享和文件传输。 |
| [获取用户数](../api/reportroot-getskypeforbusinesspeertopeeractivityusercounts.md) | Stream          | [skypeForBusinessPeerToPeerActivityUserCounts](../resources/skypeforbusinesspeertopeeractivityusercounts.md) | 获取使用情况趋势，即组织中召开的对等会话的唯一用户数和类型。 对等会话类型包括 IM、音频、视频、应用共享和文件传输。 |
| [获取分钟数](../api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts.md) | Stream          | [skypeForBusinessPeerToPeerActivityMinuteCounts](../resources/skypeforbusinesspeertopeeractivityminutecounts.md) | 获取使用情况趋势，即组织中召开的对等会话的时长（以分钟为单位）和类型。 会话类型包括音频和视频。 |
