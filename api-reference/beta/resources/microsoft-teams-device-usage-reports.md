---
title: Microsoft Teams 设备使用情况报告
description: '使用 Microsoft Teams 设备使用情况报告可深入了解贵组织的 Microsoft Teams 设备使用情况。 '
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: b9a4d2ab3034281970a3e342aa0a2d78e53678e5
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766110"
---
# <a name="microsoft-teams-device-usage-reports"></a>Microsoft Teams 设备使用情况报告

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用 Microsoft Teams 设备使用情况报告可深入了解贵组织的 Microsoft Teams 设备使用情况。 

## <a name="methods"></a>方法

| 方法                                                       | 返回类型                                                  | 说明                                                  |
| :----------------------------------------------------------- | :----------------------------------------------------------- | :----------------------------------------------------------- |
| [获取用户详细信息](../api/reportroot-getteamsdeviceusageuserdetail.md) | [teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md) | 按用户获取有关 Microsoft Teams 设备使用情况的详细信息。      |
| [获取用户计数](../api/reportroot-getteamsdeviceusageusercounts.md) | [teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md) | 按设备类型获取每日唯一 Microsoft Teams 许可用户数。 |
| [获取用户总数](../api/reportroot-getteamsdeviceusagetotalusercounts.md) | [teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md) | 按设备类型获取每日唯一 Microsoft Teams 许可或非许可用户的数量。 |
| [获取分发用户数](../api/reportroot-getteamsdeviceusagedistributionusercounts.md) | [teamsDeviceUsagedistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md) | 按设备类型获取选定时段内唯一 Microsoft Teams 许可用户的数量。 |
| [获取分发用户总数](../api/reportroot-getteamsdeviceusagedistributiontotalusercounts.md) | [teamsDeviceUsagedistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md) | 按设备类型获取选定时段内唯一 Microsoft Teams 许可或非许可用户的数量。 |


