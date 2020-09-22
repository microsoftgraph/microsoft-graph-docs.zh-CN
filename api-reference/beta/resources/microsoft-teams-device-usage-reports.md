---
title: Microsoft Teams 设备使用情况报告
description: '使用 Microsoft 团队设备使用情况报告可深入了解组织中的 Microsoft 团队设备使用情况。 '
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 991e29ada91b943428d9d3acf3523fb7e65d26b6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021355"
---
# <a name="microsoft-teams-device-usage-reports"></a>Microsoft Teams 设备使用情况报告

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用 Microsoft 团队设备使用情况报告可深入了解组织中的 Microsoft 团队设备使用情况。 

## <a name="methods"></a>方法

| 方法                                   | 返回类型                              | 说明                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [获取用户详细信息](../api/reportroot-getteamsdeviceusageuserdetail.md) | [teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md) | 按用户获取有关 Microsoft Teams 设备使用情况的详细信息。 |
| [获取用户计数](../api/reportroot-getteamsdeviceusageusercounts.md) | [teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md) | 按设备类型获取每日唯一用户数。 |
| [获取分发用户计数](../api/reportroot-getteamsdeviceusagedistributionusercounts.md) | [teamsDeviceUsagedistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md) | 在选定的时间段内按设备类型获取唯一用户数。 |


