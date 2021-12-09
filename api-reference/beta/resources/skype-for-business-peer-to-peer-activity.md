---
title: Skype for Business 对等活动报表
description: 可以获取整个组织中对等活动的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 2d0ccd9af6989ccb1a14f07818e4647e7cb2366a
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2021
ms.locfileid: "61390025"
---
# <a name="skype-for-business-peer-to-peer-activity-reports"></a>Skype for Business 对等活动报表

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

可以获取整个组织中对等活动的详细信息。 为组织调查、计划和做出其他业务决策时，便会发现这些详细信息非常有用。

> **注意：** 有关不同报表视图和名称的详细信息，请参阅Microsoft 365 [报告 - Skype for Business对等活动](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713)。

## <a name="reports"></a>报告

| 函数                                                     | CSV 返回类型 | JSON 返回类型 | 说明                                                  |
| :----------------------------------------------------------- | :-------------- | :--------------- | ------------------------------------------------------------ |
| [获取活动数](../api/reportroot-getskypeforbusinesspeertopeeractivitycounts.md) | Stream          | Stream           | 获取使用情况趋势，即组织中召开的会话的次数和类型。 会话类型包括 IM、音频、视频、应用共享和文件传输。 |
| [获取用户数](../api/reportroot-getskypeforbusinesspeertopeeractivityusercounts.md) | Stream          | Stream           | 获取使用情况趋势，即组织中召开的对等会话的唯一用户数和类型。 对等会话类型包括 IM、音频、视频、应用共享和文件传输。 |
| [获取分钟数](../api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts.md) | Stream          | Stream           | 获取使用情况趋势，即组织中召开的对等会话的时长（以分钟为单位）和类型。 会话类型包括音频和视频。 |


